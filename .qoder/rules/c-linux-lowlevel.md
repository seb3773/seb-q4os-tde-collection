---
trigger: glob
glob: *.c,*.h,*.asm
---
C/Linux Low-Level Standards
Target
Linux userland, POSIX, libc only. GCC/Clang. No Windows APIs.

Optimize: Minimize branches, align data (16/32-byte for SIMD), cache-friendly loops.

No dynamic allocs unless necessary; prefer stack/static.

Error handling: errno + perror style.

Code Style
Functions < 50 lines. Single responsibility.

Explicit types (size_t for sizes). Const where possible.

Inline assembly only if justified (measure perf gain).

Example Optimized Loop
c
// Cache-friendly, unrolled, aligned
#define ALIGN16 __attribute__((aligned(16)))
static ALIGN16 int data;

void process_data(int *src, size_t n) {
    for (size_t i = 0; i < n; i += 4) {  // Unroll x4
        data[i] = src[i] * 2;
        data[i+1] = src[i+1] * 2;
        // ... check bounds inline
    }
}