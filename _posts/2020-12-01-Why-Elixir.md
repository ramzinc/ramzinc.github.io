---
title: "Why-Elixir"
date:  2020-12-01
layout: post
---

# Table of Contents

1.  [History and Definitions](#org1d094f4)
2.  [Elixir as my language of choice.](#orgb1a687a)
3.  [Why shouldn&rsquo;t my next &ldquo;side&rdquo; project be out of elixir?](#orgb77fe8b)


<a id="org1d094f4"></a>

# History and Definitions

The elixir language is a scripting language built ontop of the BEAM Virtual Machine.
Think of this Virtual Machine in the same terms as you would do the Java Virtual Machine i.e.
these are abstract machines that accept bytecode which they inturn translate to the host machine code.
The core language BEAM was built for was Erlang but its obtuse syntax and lack of a large community
make it hard to swallow.
Like all mainstream languages, Erlang has a standard library that comes with the language and runtime(BEAM).
The standard library is normally referred to as OTP (Open Telecom Platform).
Given the name of the standard library you can guess that this language has its roots in the telecom industry but
due to slow adoption was never seriously marketed by Ericsson.
Elixir, a brainchild of Jose Valim is to the Erlang as Kotlin is to Java. Terse syntax and more approachable defaults
and tools make Elixir stand out. A slight syntactical resemblance with Ruby has led to an influx of
ruby engineers into the elixir community and ofcourse there is me. A resident nomad with programming languages, the only thing I&rsquo;ve stuck to is my text editor: Emacs. Which i&rsquo;ve used for close to 4 years and still barely scratch its full potential as an OS.


<a id="orgb1a687a"></a>

# Elixir as my language of choice.

Most innovations are either basically unifying or decomposition techniques. Neftlix decomposed satelite tv from channel providers to content providers, Docker decomposed VM&rsquo;s to libraries and run time environments. Elixir decomposed building software to its basic unit: processes. This I must admit is also happening with the JVM with [continuations.](https://cr.openjdk.java.net/~rpressler/loom/Loom-Proposal.html) To understand the complexity that can arise from having to deal with distributed state as an ad hoc issue look at Josh Evan&rsquo;s [talk](https://www.youtube.com/watch?v=CZ3wIuvmHeM) on Mastering Chaos at Netflix. Dealing with failure as a feature not as a surprise should be a feature of most languages otherwise then you have to build a whole system to check for failed state and it&rsquo;s after effects.
My education in elixir begyn with Sasa Juric&rsquo;s [Elixir in Action](https://www.manning.com/books/elixir-in-action-second-edition) whose clarity and succinct exposition on the core of elixir is heaven sent. Topics like gen<sub>servers</sub> have to be understood inside out and Juric&rsquo;s book does a great job on teasing this concept out. Starting out by using processes and messaging as computational primitives one gets a small feel for what I hope Alan Kay&rsquo;s(ofcourse am fan) smalltalk might have been.
You graduate slowly building amazing stuff like Process registries, cache servers, your own crude persistence solution using the filesystem and an erlang function `:erlang.term_to_binary` till you finally build a distributed todo list and throw a web interface on it just for the lulz.
Finishing this book left me with a feeling of amazement and change of perspective on the possibilities of my programming career despite its still rather low popularity, Elixir has a rather highly dedicated community that has built great open source software around it not to mention the not so Free software that has been built using Erlang and Elixir e.g: Whatsapp, Riak, RabbitMQ etc.


<a id="orgb77fe8b"></a>

# Why shouldn&rsquo;t my next &ldquo;side&rdquo; project be out of elixir?

-   Low popularity means support comes down to the slack and IRC channels you&rsquo;re on but like I said the individuals involved are somewhat friendly and always ready to help.
-   Syntax can be obtuse and pattern matching is so foreign a concept you&rsquo;ll always get bitten by it but if like me you&rsquo;ve tried though never finished SICP(hopefully I die after finishing it), you&rsquo;ll get accustomed to it quiet quickly.

In conclusion I do believe I have found my favourite language thus far. Please do try it out and do read Elixir In Action it&rsquo;s a great read.
