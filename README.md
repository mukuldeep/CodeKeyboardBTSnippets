# CodeKeyboardBTSnippets
This repository serves as a centralized Snippet Store for the app. It contains structured JSON files that define reusable code snippets which can be imported directly into the application.

Each snippet file follows a standardized format, allowing the app to validate, store, and trigger snippets efficiently. The purpose of this repository is to provide a clean, organized collection of ready-to-use code templates that improve typing speed, reduce repetition, and enhance developer productivity—especially when coding wsing the app from mobile devices.

Snippets in this repository are:
  - Structured in a strict JSON format
  - Organized for easy import
  - Validated by the app before storage
  - Designed to be lightweight and extensible

This repository acts purely as a storage and distribution layer for snippets, making it easy to maintain, share, and expand reusable code templates over time.




## Code Snippet JSON Format
The snippet file must follow a strict object-based structure similar to VS Code snippet format.

The root of the JSON file must be a single JSON object. Each key inside the root represents a  **snippet name**.

```
{
  "Snippet Name": {
    "prefix": "trigger",
    "body": ["code line 1", "code line 2"],
    "description": "Short description"
  }
}
```

### Rules

  1. Root must be a JSON object.
  2. Each snippet must contain:
  3. prefix (string)
  4. body (non-empty string array)
  5. description (string)
  6. body must contain only strings.
  7. No trailing commas allowed.
  8. JSON must be valid UTF-8.

### Body Field Details

  - Body Field Details
  - Each array element represents a single line.
  - Indentation should be included as spaces inside the string.
  - Placeholders are not supported.
  - Escape quotes properly (\").

### File Naming Recommendation

File name is considered as default group name while importing in the Code Keyboard BT App. Recommended file name format is `language-name-snippets-category.json` for example `java-basic-algorithms.json`, `cpp-search-algo.json`.

# Contributing

Contributions are welcome from everyone!

If you'd like to add new snippets, improve existing ones, or organize snippet collections, feel free to submit a pull request. This repository is community-driven and aims to grow into a rich, well-structured snippet library for developers.

### How to Contribute

  - Fork the repository
  - Add or modify snippet JSON files following the required format
  - Ensure the JSON is valid and properly structured
  - Submit a pull request with a clear description of your changes

### Contribution Guidelines

  - Follow the defined snippet JSON format
  - Keep snippet names unique and descriptive
  - Use meaningful prefix values
  - Write clear description text
  - Ensure proper indentation inside body strings
  - Avoid duplicate or redundant snippets

All valid and useful contributions are appreciated.


