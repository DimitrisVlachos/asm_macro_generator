# asm_macro_generator
An old assembly pre-processor i wrote back in 2010-2011 to allow function blocks/nested function calls &amp; loops through assembly code.
I used it mostly for mips32/z80/M68K back then but works with any arch...
Recursion is also supported along with loop unrolling & generated hints for debugging

#build
g++ asm_mac_gen.cpp -O2 -std=c++11 -o macgen

#Usage
./macgen source.S dest.S

#Optional aguments
-ident  (fixes identantion) 
-tab2ws (converts hard tabs to whitespace)
 -wsdepth depth (number of whitespaces in a tab (defaults to 4))
 -nohints (disables comments/hints in the generated file)
 
