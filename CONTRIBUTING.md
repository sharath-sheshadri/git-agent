# Contributing to Hello World Python Project

We love your input! By participating in this project, you agree to abide by the following guidelines:

## How to Contribute

1. **Fork the repository**
   - Click the "Fork" button at the top right of the repository page.
2. **Clone your fork**
   ```bash
   git clone https://github.com/<your-username>/git-agent.git
   cd git-agent
   ```
3. **Create a new branch** for your work:
   ```bash
   git checkout -b <feature-or-bugfix-name>
   ```
4. **Make your changes**
   - Follow the coding style used in the project (PEP 8).
   - Add or update tests if applicable.
5. **Commit your changes**
   ```bash
   git add .
   git commit -m "Brief description of the change"
   ```
6. **Push to your fork**
   ```bash
   git push origin <feature-or-bugfix-name>
   ```
7. **Open a Pull Request**
   - Navigate to the original repository and click "New pull request".
   - Provide a clear description of what you changed and why.
   - Reference any related issues using `closes #<issue-number>`.

## Code Style

- Use **PEP 8** formatting. You can run `ruff` or `flake8` to check style.
- Keep lines under 88 characters where possible.
- Use type hints for public functions.

## Testing

- Add unit tests in the `tests/` directory.
- Run tests with `pytest`.
- Ensure all existing tests pass before submitting a PR.

## Documentation

- Update the `README.md` or relevant docs if your change affects usage.
- Keep documentation clear, concise, and up‑to‑date.

## License

By contributing, you agree that your contributions will be licensed under the same MIT License as the project.
