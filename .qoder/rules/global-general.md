---
trigger: always_on
alwaysApply: true
---
# Global Coding Standards - Apply to all code generation

## Core Principles
- Write clean, readable, efficient code. Prioritize simplicity over cleverness.
- Always provide COMPLETE, compilable/runnable code with all includes/imports/dependencies.
- Handle errors explicitly (no silent fails). Use return codes or exceptions where appropriate.
- Include short explanation of changes + why they improve code.
- Format output as: 1. Brief rationale (2-3 sentences). 2. Full code block. 3. Test instructions if applicable.

## Process
1. Think step-by-step before coding
2. Query rules/knowledge first  
3. Write COMPLETE compilable code
4. Format: Explanation → Code block → Test command

## Quality Checks
- No unused variables/functions.
- Optimize for performance (min allocs, cache-friendly, branch prediction).
- Security: Validate inputs, avoid buffer overflows, SQL injection.
- Standards: Follow language best practices (MISRA for C/C++, PSR-12 for PHP).

## Examples
Good C function:
```c
#include <stdio.h>
#include <stdlib.h>

int safe_add(int a, int b) {
    if (a > INT_MAX - b) return -1;  // Overflow check
    return a + b;
}
