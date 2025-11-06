# qmlformat-hook

The only standalone, multiplatform pre-commit hook for formatting QML files using the `qmlformat` tool with no Qt prerequisites required.

## Installation

1. Add this repository to your `.pre-commit-config.yaml`:

   ```yaml
   - repo: https://github.com/tomas-krupa/qmlformat-hook.git
     rev: 1.2.0
     hooks:
       - id: qmlformat
         #args: ["--check"]
         #additional_dependencies:
         #  - PySide6-Essentials==6.8.3 # override version of Qt Python metapackage
   ```
* By default, all `*.qml` files will be matched

2. Install the pre-commit hooks:

   ```bash
   pre-commit install
   ```

3. Make a commit with QML files to see the hook in action.
