# Schema Store Repository

Welcome to the **Schema Store Repository**, a collection of JSON and YAML schemas designed to provide validation and standardization for various configuration files. This repository simplifies the development process by offering schemas for configurations that are often missing from popular schema repositories like [SchemaStore.org](https://www.schemastore.org/).

---

## 🚀 Features

- A curated collection of JSON and YAML schemas for popular configuration files.
- Validation and linting support for multiple tools and environments.
- Easily integrable into CI/CD pipelines.
- Includes schemas not available in popular schema repositories like [SchemaStore.org](https://www.schemastore.org/).

---

## 📂 Included Schemas

This repository includes the following schemas:

### JSON Schemas

#### `package-lock.json`
- **Description**: Validates the structure of `package-lock.json` files used by Node.js projects.
- **Location**: `json/package-lock-schema.json`
- **Usage**: Ensures the integrity and consistency of your package dependencies.

#### `.vscode/settings.json`
- **Description**: Validates the structure of `.vscode/settings.json` files used by Visual Studio Code.
- **Location**: `json/vscode-settings-schema.json`
- **Usage**: Ensures correct configurations for your VSCode workspace settings.

### YAML Schemas

#### `compose.yaml`
- **Description**: Validates the structure of Docker Compose configuration files.
- **Location**: `yaml/compose-schema.yaml`
- **Usage**: Ensures your Docker Compose files are properly configured for multi-container applications.

#### `mega-linter.yaml`
- **Description**: Validates MegaLinter configuration files.
- **Location**: `yaml/mega-linter-schema.yaml`
- **Usage**: Ensures your MegaLinter setup adheres to expected standards and structure.

---

## 🛠️ Usage

To use these schemas in your project:

1. Clone this repository:
   ```bash
   git clone https://github.com/adanmauri/schemastore.git
   ```

2. Include the schema in your project configuration. For example, in a VSCode workspace:
   ```json
   {
     "$schema": "https://raw.githubusercontent.com/adanmauri/schemastore/main/json/package-lock.json"
   }
   ```

3. Validate your configuration files using tools like:
   - VSCode's built-in JSON and YAML validation.
   - [AJV JSON Schema Validator](https://ajv.js.org/) for JSON files.
   - [YAML Lint](https://yaml-lint.com/) for YAML files.
   - [v8r](https://chris48s.github.io/v8r/) for JSON and YAML files.

---

## 🤝 Contributing

We welcome contributions! To contribute:

1. Fork this repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/new-schema
   ```
3. Add your changes.
4. Submit a pull request.

For detailed guidelines, see the `CONTRIBUTING.md` file.

---

## 📜 License

This repository is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 💡 About

This repository was created to centralize and simplify schema validation for common configuration files. It is a part of ongoing efforts to streamline development workflows and promote best practices.

---

Feel free to reach out or open an issue for questions, suggestions, or to report bugs. Happy coding! 🎉
