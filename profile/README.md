# Respect your tools.

The GNU Compiler Collection has a command, `gcc`, that is *not* the C
compiler. It is a command for calling *all* of the compilers.

In fact, when you compile the GNU Compiler Collection itself, from its
own source code, the `gcc` command is used to compile *Ada* code.

One is supposed to compile the Collection as a unitary whole, with all
the languages enabled that one is going to use. Then the `gcc` command
will know it recognizes those languages. This is how the tool was
designed. This is how it has been for a long time.

*Respect your tool.*

NixOS has not respected this tool. It has compiled the languages’
compilers in isolation from the others. It does not matter *why* this
was done. It was done in disrespect of the tool.

Furthermore, NixOS does not compile the GNU Compiler Collection three
times, as is the upstream default for a native build. Why is this the
default? It makes the Collection *self-hosting*. The C/C++ and Ada
compilers, at least, are then *compiled with themselves*. Furthermore,
they are compiled with themselves *twice*, and it is verified that
that *the same result is obtained both times*.

This is how the GNU C compiler has been built since version 1. It is a
good system. You are preparing your tool for honest work.

❦ ❦ ❦

This organization seeks to respect the tools.

We will try to restore the GNU Compiler Collection to its intended
form. We may or may not succeed, but we will try.

We will try to make development environments more closely resemble
those of ordinary POSIX systems. We may or may not succeed, but we
will try.

What good is purity and reproducibility if the tools—and thus the
products of those tools—are not of the same quality as found
elsewhere?

The GNU Compiler Collection on a Linux From Scratch is better than
that on a NixOS system. We have no hesitation in saying so. The
compilers are thrice compiled on the very machine they are to be used
on.

❦ ❦ ❦

We will also put any and sundry here.

❦ ❦ ❦

The proprietor of the organization is an aging person who has been
disabled for many years. Please do not overtax them. Also please
respect that they may have learnt something over the years that they
did not always know, and which they do not expect to be understood
universally.

That one must respect the tool—rather than demand of the tool that *it*
respect *you*—is a hard lesson to learn.

It is a cause, for instance, of people using inferior programming
languages. They are demanding of the language that it respect them.
Really good programming languages are designed by people who know much
more about it than you do. An example is Ada. It is not the simplest
language to use, but that is because you must respect it. The people
who designed it took into account matters you did not even know about.

Do not worry. We also use Scheme, for instance. We use Icon. But we
furthermore use ATS, which embeds static proofs.
