---
title: Porting
redirect_from:
  - /Porting/
  - /Mint/
  - /Porting_and_Hardware_Architecture/
---

Mono has been ported to a number of architectures already, and today it is made up of about 200,000 lines of code and only a small fraction is required for porting it to a new architecture (about 5,000 lines of C code, with a little bit of assembler code)

Porting the VM to a new architecture
====================================

There are a number of documents in the wiki under [Runtime documentation](/docs/advanced/runtime/docs/), in particular read the document [Porting the engine](/docs/advanced/runtime/docs/mini-porting/)

Endian, 64 bits and unaligned access issues
-------------------------------------------

Mono has been ported to little-endian, big-endian, 32 and 64 bit architectures, so it should just be a matter of configuring properly your target, in particular make sure to set ACCESS_UNALIGNED="yes" if your architecture doesn't support accessing ints from unaligned memory locations.

Generating assembly bytecodes for the target processor
------------------------------------------------------

Next, you need to provide the support code for generating machine code for your target platform (in mono/arch/{ppc,sparc,alpha,\*}).

The code should be more or less like the code in x86-codegen.h: macros that produce in-line code for each instruction that you need. For example the 80x86 instruction "ret" has a macro called "x86_ret" that will generate the machine code for the ret instruction in a buffer provided to it.

You do not need to provide code to create every possible opcode. Initially, you just need the code to create trampolines and execute them (you'll need to research how the call convention works on your platform): that would be, for example, the prolog and epilog code in a function, code to pass function parameters and deal with the return value and so on.

You need to learn the calling convention used in your architecture: if you can not find a specification, or you have doubts, you can look at libffi in gcc or the xptcall sources in mozilla. You can also write functions in C and compile them for your architecture: examining the generated assembly code you can see the calling convention being used (if arguments are passed on the stack or in registers, alignment constraints and so on).

You will also need a processor manual to know how to create the assembly binary data. This requires a lot of reading if you're not familiar with the assembly for your target platform. Manuals for many processors are available as PDF files on the web site of the respective vendors. Note that some processors require you to flush the I-cache before executing the code: have a look at how the same thing is done in GNU lightning.

Getting the interpreter to work
-------------------------------

We used to sugget porting the interpreter first, but since we no longer maintain the interpreter code, you should skip this step, the interpreter is most likely not compilable anymore, so go to the JIT porting section.

Once you can generate binary code, you can start working on a mono_create_trampoline() function for your platform: this function will receive a MonoMethod that describes the arguments and the return type of a C function and will create the code to call such function. When this function is complete you'll be able to run more sample programs, that use System.IO and P/Invoke functions.

To support delegates you'll need to write a mono_create_method_pointer() function that creates a native function: this can be used to call the method using the runtime's calling convention (it's basically the reverse of mono_create_trampoline()).

The final step: porting the JIT
-------------------------------

At this point you'd need to have a more complete code generation header file and you can start porting the JIT code. This process is documented in [Mono:Runtime:Documentation:MiniPorting](/docs/advanced/runtime/docs/mini-porting/).

Operating System Ports
======================

Most of the operating system specific bits live in the mono/io-layer directory in the Mono module.

When porting mono, two things are important:

-   if the jit has been ported to the wanted cpu
-   if the os supports a correct implementation of POSIX/pthreads

If both conditions are true, you'll likely need only small tweaks to the configure files and maybe the signal handling mechanism, this means just a few days of work.

If the OS doesn't support pthreads, you will need to implement the io-layer interfaces (basically the small thread-related subset of the win32 API).

If the OS doesn't support POSIX and the standard libc calls, you'll likely have to make changes in many places.


