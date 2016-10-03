# GROMACS-5.1.3
Gromacs with modified kernel

The non-bonded forces can be shifted in this version of GROMACS on machines running AVX 256 / AVX 128 FMA / SSE2 / SSE4.1 processors in single and double precision mode. You will need to pass -DSHIFT_FORCES=value to cmake when compiling Gromacs, with
value being a floating point number that represents the distance (in nm) by which the interatomic distance is shifted. e.g. to compile Gromacs with shifted forces in double precision on an X86 machine, -DSHIFT_FORCES=0.1 must be passed to cmake.
