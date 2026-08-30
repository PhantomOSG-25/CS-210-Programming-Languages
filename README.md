# CS 210 — C++ Programming Fundamentals

A small, portable C++17 example that demonstrates program structure, standard output, and a reproducible build. The project preserves the original introductory programming objective while removing IDE-specific and generated files.

## What this demonstrates

- A minimal C++ entry point and return-value convention
- Standard-library console output with `iostream`
- Portable CMake configuration instead of a machine-specific IDE project
- A smoke test that confirms the executable launches successfully

## Build and run

```powershell
cmake -S . -B build -DBUILD_TESTING=ON
cmake --build build --config Release
ctest --test-dir build -C Release --output-on-failure
```

Run the executable from `build/` after compilation.

## Scope

This is an introductory CS 210 artifact, not a large application. It is included to show foundational C++ fluency and disciplined project packaging alongside the more advanced C++ work in the CS 300 Course Planner repository.
