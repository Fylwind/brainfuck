Shell implementation of Brainfuck
=================================

An implementation of the esoteric programming language
[Brainfuck](https://en.wikipedia.org/wiki/Brainfuck) using shell scripts of
the Bourne variety.  Should be portable on any system with a Bourne-like
shell, even ancient ones like the heirloom shell.

  - `brainfuckc`: A compiler that translates Brainfuck into C code, and then
    (optionally) compiles the C code using a native C compiler.  The
    translation phase is a bit slow, but tolerable.  Execution is fast, but
    beware of undefined behavior if you go outside the bounds of the array.

    Example usage: `./brainfuckc -o myprogram mycode.bf && ./myprogram`

    For more info, run: `./brainfuckc -h`

  - `brainfucki`: An interpreter that reads Brainfuck code character by
    character and executes it via the shell.  Really really slow.

    Example usage: `./brainfucki mycode.bf`

    For more info, run: `./brainfucki -h`

I have no idea why I made this :v
