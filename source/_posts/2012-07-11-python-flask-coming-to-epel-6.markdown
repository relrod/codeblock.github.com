---
layout: post
title: "python-flask coming to EPEL 6 soon-ish"
date: 2012-07-11 18:20
comments: true
categories: ['fedora', 'python', 'programming']
---

For those not aware, I recently picked up the python-flask and python-werkzeug
packages, which were going to be orphaned.

I've spent the majority of today working on getting python-flask and its
dependencies working on EPEL 6, with Ian Weller.

The current plan is to get Flask 0.9 in EPEL right from the get-go.

There are two small patches we need to apply to the package to make using it
as painless as possible on RHEL environments. They both relate to telling
Flask to use the right Jinja2 package.

RHEL6-optional has Jinja 2.2.1. Flask requires 2.4 or greater. So we use the
EPEL version of Jinja2, `python-jinja2-26` which gives us Jinja 2.6. But we
need to tell Flask that it should import the 2.6 version, not the 2.2 version.

The other blocker is `python2-werkzeug` -- the current EPEL 6 version of
werkzeug is 0.6.2. The plan there is to update that to 0.8.3, pending an
exemption of the Incompatible Upgrades Policy, at the EPEL meeting on Monday.

In any case, I just wanted to throw it out there that we are working on this
and we plan on having these pushed to EPEL soon. We're starting to develop
some custom apps with Flask, for use in the Fedora Infrastructure, so
this had to be done sooner or later.

Stay tuned.
