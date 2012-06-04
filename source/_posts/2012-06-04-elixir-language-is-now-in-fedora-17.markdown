---
layout: post
title: "Elixir Language is now in Fedora 17"
date: 2012-06-04 11:24
comments: true
categories: fedora elixir programming
---

Well it's been a week since my 
[Elixir language](http://elixir-lang.org/) package got
[approved](https://bugzilla.redhat.com/show_bug.cgi?id=825418#c4) and I am
happy to announce that it has been pushed to stable, and now appears in the
Fedora 17 updates repository.

Anyone who uses Fedora 17 or Fedora Rawhide, and wants to try out the new
programming language by José Valim (which runs on the Erlang VM), can simply:
`sudo yum install elixir`

I might later on introduce an `elixir-git` subpackage for rawhide that tracks
Elixir's git repository more closely, but for now the `elixir` package tracks
the stable, currently 0.5.0 release, of Elixir.

```elixir
iex> IO.puts "Happy hacking!"
Happy hacking!
:ok
```
