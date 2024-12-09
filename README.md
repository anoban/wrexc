Pronounced `"I'll see" (isle c)` is a C23 compiler for Windows implemented in Python referencing Nora Sandler's book `"Writng A C Compiler" No Starch Press. 2024`.

#### Goals   
- Porting the reference implementation (provided as pseudo code for `Linux system V ABI` in the reference) to `Win64`.
- Switching to `Intel` assembly syntax instead of the `AT&T` syntax used by the reference.
- Supporting most `C23` features including attribute syntax `[[attribute]]` and `#embed`.
- Less permissive compile time type checks (compiler by default behaves as if other C compilers with `-Wall` and `-Werr` switches turned on)

#### Non-goals    
- Support for other operating system ABIs.
- Support for processor architectures other than AMD64.
- Full compliance with ISO C23 standard.
- Generating assembly code that's on par with production ready compilers in terms of optimizations.
- Performance, I wouldn't have chosen Python if this was a goal.
