## Intel HDA Device Driver

As part of a larger project to create an accessible UEFI environment for the visually impaired,
I've adapted a driver from RedoxOS to a standalone driver that can run on bare hardware in a UEFI environment: all written in pure Rust.

However, I'm catching a couple snags, and would like to at least be stuck on some other issue than this one (this issue is about 4 months old at this point).

When running on real hardware: "Intel 11th Generation Framework laptop 13", it seems that the program reliably crashes when returning from the initialize() method.
My best guess is that the `Drop` implementation of one of the structures allocated during the running of the function is causing this, but there's all sorts of stuff it could be.

Looking for specific help with:

* Intel HDA Specification
* Additional accessibility input

But general help with:

* cleanup
* refactoring
* correctness
* more compile-time checks

...would also be helpful.
