# Contributing to UUID to Picture

Thank you for your interest in contributing! This document provides guidelines for contributing to the project.

## Getting Started

1. Fork the repository
2. Clone your fork:
   ```bash
   git clone https://github.com/your-username/uuid-to-picture.git
   cd uuid-to-picture
   ```
3. Open `index.html` in your browser — no build step required

For a local development server:
```bash
npx serve .
# or
python3 -m http.server 8000
```

## Development Guidelines

### Code Style

- **No frameworks or dependencies** — this project is intentionally vanilla JS
- Use ES6+ features (const/let, arrow functions, template literals)
- Follow existing code patterns and naming conventions
- Keep functions small and focused

### Project Structure

```
js/
├── uuid.js             — UUID validation, parsing, generation
├── encoder.js          — UUID to GridModel (logical dot matrix)
├── canvas-renderer.js  — GridModel to Canvas (display + PNG export)
├── svg-renderer.js     — GridModel to SVG string (SVG export)
├── decoder.js          — PNG image to UUID (pixel sampling)
└── app.js              — Entry point, UI event handlers
```

### Testing

Before submitting a PR, verify the encoding/decoding roundtrip:

1. Generate or enter a UUID
2. Click **Generate Picture**
3. Download as PNG
4. Upload the PNG in the **Picture to UUID** section
5. Confirm the decoded UUID matches the original

### Submitting Changes

1. Create a feature branch: `git checkout -b feature/your-feature`
2. Make your changes
3. Test the roundtrip verification
4. Commit with a descriptive message
5. Push and open a Pull Request

## Reporting Bugs

Use the [Bug Report](https://github.com/dykyi-roman/uuid-to-picture/issues/new?template=bug_report.md) issue template.

## Requesting Features

Use the [Feature Request](https://github.com/dykyi-roman/uuid-to-picture/issues/new?template=feature_request.md) issue template.

## License

By contributing, you agree that your contributions will be licensed under the MIT License.
