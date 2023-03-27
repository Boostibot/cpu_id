# cpu_id
*A c/c++ header for cpu id related info on x86*

## List of supported compilers/targets:
 - **(w) works**:         properly reports cpu
 - **(c) compiles**:      compiles but all functions return empty (can be stil used for runtime testing of flags which will never pass)
 - **(d) doesnt compile**

### MSVC:
  - x86/x64/x86_64:   w
  - arm64 + C:        w
  - arm64 + C++:      c

### GCC/Clang:
  - x86/x64/x86_64:   w
  - arm32:             c
  - arm64:             c
  - risc:              c
  - mips:              c
  - power:             c
  - clang wasm:        d (missing string.h?)
  - clang armv7:       d (missing string.h?)
  - other:             c

### MinGW GCC/MinGW Clang:
 - x86/x64:          w

see https://en.wikipedia.org/wiki/CPUID for more info

