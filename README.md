
# L2T - TextToolkit Test Suite

## Assignment L2 in 1DV610

**Version:** 1.0.0
**Author:** Dan-Håkan Davall  
**Email:** [dd222mk@student.lnu.se](mailto:dd222mk@student.lnu.se)

## 🗂️ Project Description

This project is a **comprehensive test suite** for the `texttoolkit` npm package - a modular JavaScript toolkit for advanced text analysis, formatting, search, and transformation with support for Swedish (including å/ä/ö) and English.

This repository contains only the test files that verify the functionality of the `texttoolkit` package, which is included as a dependency.The `texttoolkit` package provides all public APIs and functionality.

***

## 🧪 Test Structure Overview

This repository contains comprehensive test suites for the following components:

- **TextDocument**: Tests for the main wrapper class that aggregates all text operations
- **TextAnalyzer**: Tests for word, character, and sentence analysis, frequency and palindrome detection
- **TextFormatter**: Tests for uppercase/lowercase, capitalization, camelCase, snake_case and trim operations
- **TextSearcher**: Tests for substring search, regex search and position services
- **TextTransformer**: Tests for text transformations and replacement operations
- **TextReverser**: Tests for various text reversal functions
- **HelpFunctions**: Tests for utility functions and input validation

***

### Test Files Overview

This repository contains test suites organized by component:

```text
test/
├── TextDocument.test.js          # Tests for main wrapper class
├── analyzers/
│   └── TextAnalyzer.test.js      # Text analysis functionality tests
├── formatters/
│   └── TextFormatter.test.js     # Text formatting tests
├── searchers/
│   └── TextSearcher.test.js      # Search functionality tests  
├── transformers/
│   ├── TextTransformer.test.js   # Text transformation tests
│   └── TextReverser.test.js      # Text reversal tests
└── helpfunctions/
    └── helpFunctions.test.js     # Utility functions tests
```

Each test file comprehensively covers:

- **Functionality testing**: Core features and methods
- **Edge cases**: Boundary conditions and error handling  
- **Input validation**: Type checking and error responses
- **Swedish language support**: åäö character handling

***

## 🚀 Running Tests

To run the complete test suite:

```bash
npm test
```

This will execute all test files using Jest and provide a comprehensive report of the `texttoolkit` package functionality.

## 📋 Test Coverage

The test suite covers:

```javascript
// Example of what the tests verify:
import { TextDocument } from 'texttoolkit';
const doc = new TextDocument("Hello world! This is a test document.");
// Tests verify: word counting, formatting, searching, transforming
```

***

## 🦾 Developer Workflows

- **Testing:**  
  `npm test` (Jest, with tests in the `test/` directory)
- **Module imports:**  
  ES modules – use `import/export`
- **Test structure:**  
  Follow existing patterns for new test files***

## ⚙️ Test Conventions

- **Language support:** Tests verify Swedish/English functionality including åäö
- **Input validation:** Tests verify error handling for invalid inputs  
- **Edge cases:** Comprehensive testing of boundary conditions
- **Jest patterns:** Follow established Jest testing conventions

***

## 🛠️ Adding New Tests

- Add new test files in the appropriate subdirectory under `test/`
- Follow existing naming conventions: `ComponentName.test.js`
- Test both success cases and error conditions
- Ensure tests cover Swedish character support (åäö)

***

## 📄 Test Information

- See `test/` directory for comprehensive test coverage
- All tests verify expected behaviors and edge cases
- Tests ensure proper error handling and validation

***

## 💻 Installation Instructions

```bash
git clone https://github.com/egsdandd/L2T.git
cd L2T
npm install
```

***

## 📦 Dependencies \& Requirements

- Node.js **v14 or later**
- Jest for testing (v29.7.0)
- `texttoolkit` package (v1.0.1) - the package being tested
- ES Modules support (`"type": "module"` in package.json)

***

## 🧪 Test Execution

- Comprehensive test coverage for all `texttoolkit` components
- Run `npm test` to execute all tests with Jest
- Tests use ES modules with `--experimental-vm-modules` flag

***

## 🤝 Contributing to Tests

1. Fork and create a feature branch
2. Add comprehensive test cases for new functionality
3. Ensure all existing tests continue to pass
4. Write clear commit messages describing test additions/changes

***

## 🐞 Bug Reports / Issues

_Detected a bug?_
Create an issue on GitHub with as much information as possible: steps to reproduce, expected and actual behavior.

***

## ⚖️ License

MIT License

***

## 💬 Communication & Questions

For questions or suggestions about the tests, create an issue on GitHub or contact the repository owner.
