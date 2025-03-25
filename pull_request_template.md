---
name: "Valormill Firmware Pull Request Template"
about: "A standardized PR template implementing Valormill code review and checklist processes. Implements SOPXX.XX"
---

# Valormill Firmware Pull Request

## Resolved Issues
<!-- Include any relevant issues closed by this pull request. Use the form "Closes <task>" -->
...

## Description
<!-- Provide a clear and concise description of the changes included in this pull request. -->
...

## Files Modified
<!-- List the major files that were added or modified -->
- src/moduleName.c
- include/moduleName.h

## Valormill Code Review Checklist

### Process
- [ ] All comments use `//` style (no `/* */` blocks).
- [ ] Comments are limited to 80 characters per line.
- [ ] Function definitions are preceded by a line of `//-------------` (80 characters wide).
- [ ] Each function has a descriptive comment block

- [ ] Code builds successfully without errors or warnings.
- [ ] The code has been run through `clang-format` for automated formatting.
- [ ] Auto-generated files are excluded.

### Variables and Data Types
- [ ] Variable names are clear, concise, and context-appropriate (e.g., int numPeople, not float NumPeople).
- [ ] Overly long or confusing variable names have been avoided.
- [ ] Data types are consistent with each variable’s context (e.g., float costInUSD).

### Functions
- [ ] Function names use camelCase (e.g., initModule, processData).
- [ ] Function names clearly describe their purpose.
- [ ] Helper functions are documented and appropriately placed.

### File Structure
- [ ] Header and source files follow Valormill’s standardized templates.
- [ ] Header files include:
- [ ] Description
- [ ] Test Plan
- [ ] Test Results
- [ ] Source files only contain the implementation of declared functions.

### Formatting
- [ ] Indentation uses 2 spaces (no tabs).
- [ ] No trailing whitespace or unnecessary blank lines.
- [ ] Line lengths do not exceed 80 characters.
- [ ] Proper spacing is maintained around operators (e.g., x + y, not x+y).

### General Checks
- [ ] Auto-generated files are excluded.
- [ ] Code builds successfully and passes all tests.
- [ ] `clang-format` has been run on all files.
- [ ] No dynamic memory allocation is used.

## Summary Checklist
- [ ] All comments follow Valormill standards.
- [ ] Variable names are clear and context-appropriate.
- [ ] Functions follow camelCase and include descriptive comment blocks.
- [ ] File structure adheres to Valormill templates.
- [ ] Code formatting follows Valormill guidelines.
- [ ] Auto-generated files are excluded.
- [ ] Code builds and tests pass successfully.
- [ ] All modified code has been formatted with `clang-format`.

## References
- Valormill Best Practices – https://docs.google.com/document/d/1Ggo4Ehwjj8n_0gmsaDJAtWLA2fcyl5kjRNULTfklryw/edit?tab=t.0#heading=h.u4mj2ifxx4fq
- Generic Code Review Checklist: https://docs.google.com/document/d/1VenPGzfMm0HoLB1_8-w5PMExpdjibc2o1RiMtGw6_kg/edit?tab=t.0
