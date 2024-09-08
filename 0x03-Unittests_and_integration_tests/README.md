# Unit and Integration Testing Project

## Description

This project involves understanding and implementing unit tests and integration tests in Python. The focus is on testing functions to ensure they work as expected under various conditions. We will explore concepts such as mocking, parametrization, and fixtures, and use the `unittest` framework to test the functionality of different modules. Unit testing helps ensure individual functions work in isolation, while integration testing ensures the code works end-to-end.

## Concepts Covered

### 1. Unit Testing

- **Unit tests** validate that individual pieces of code (usually functions) behave as expected with different inputs.
- Unit tests are focused on testing a function in isolation, without external dependencies (e.g., network calls, database interactions).
- External dependencies are **mocked** in unit tests to simulate their behavior.
- **Goal**: Verify the correctness of a function in isolation.

### 2. Integration Testing

- **Integration tests** validate that different parts of the codebase work together as expected.
- Integration tests do not mock components like database calls or API requests; instead, they simulate a full code path.
- **Goal**: Test interactions between various components to ensure they work together correctly.

### 3. Mocking

- **Mocking** is a technique used in testing to simulate the behavior of external dependencies (e.g., API calls, databases).
- It allows testing code in isolation by providing controlled responses for external dependencies.
- [unittest.mock — Mock object library](https://docs.python.org/3/library/unittest.mock.html)

### 4. Parametrization

- **Parametrization** allows running the same test with multiple sets of inputs.
- This makes it easier to test a function against a wide variety of data.
- [Parameterized Testing](https://pypi.org/project/parameterized/)

### 5. Fixtures

- **Fixtures** are setup and teardown methods used to prepare the test environment.
- They ensure that tests start with a known state and clean up after themselves.
- [unittest — Fixtures](https://docs.python.org/3/library/unittest.html#unittest.TestCase.setUp)

## Requirements

- All files will be interpreted/compiled on Ubuntu 18.04 LTS using Python3 (version 3.7)
- All files should end with a new line
- The first line of all your files should be exactly `#!/usr/bin/env python3`
- A `README.md` file at the root of the project is mandatory
- Code should use the **pycodestyle** style (version 2.5)
- All files must be executable
- All modules should be documented (use `python3 -c 'print(__import__("module").__doc__)'`)
- All classes should be documented (use `python3 -c 'print(__import__("module").MyClass.__doc__)'`)
- All functions should have proper documentation (use `python3 -c 'print(__import__("module").my_function.__doc__)'`)
- Functions and coroutines must be type-annotated

## How to Execute Tests

To run the tests, use the following command:

```bash
$ python -m unittest path/to/test_file.py
```
