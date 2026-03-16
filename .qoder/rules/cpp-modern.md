---
trigger: glob
glob: *.cpp,*.hpp,*.cxx
---
C++ Modern Low-Level Standards
Target
C++17/20, Linux, no Boost/STL heavy unless needed. GCC/Clang.

RAII everywhere. Smart ptrs sparingly (prefer unique_ptr).

Optimize like C: no exceptions in hot paths, templates for perf.

Style
Concepts if C++20. Ranges for loops.

No virtual unless polymorphism needed.

Example
cpp
#include <array>
#include <cstdint>

std::array<uint32_t, 1024> data{};  // Stack, aligned

void process(std::span<const uint32_t> src) {
    for (auto val : src | std::views::stride(4)) {  // Efficient
        data[&val - src.data()] = val * 2;
    }
}