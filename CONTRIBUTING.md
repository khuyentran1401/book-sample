# Contributing to Production Ready Data Science

## Development Setup

1. **Fork and Clone the Repository**

   ```bash
   # Fork the repository through GitHub's web interface, then:
   git clone https://github.com/YOUR-USERNAME/production-ready-data-science.git
   cd production-ready-data-science
   git remote add upstream https://github.com/khuyentran1401/production-ready-data-science.git
   ```

2. **Install Development Dependencies**

   ```bash
   # Install Poetry
   curl -sSL https://install.python-poetry.org | python3 -

   # Install dependencies
   poetry install --with dev

   # Activate the virtual environment
   poetry shell
   ```

3. **Install Quarto**

   Install Quarto from [https://quarto.org/docs/get-started/](https://quarto.org/docs/get-started/)

4. **Install Pre-commit Hooks**

   ```bash
   pre-commit install
   ```

### Project Structure

- `/chapters` - Quarto book chapters (`.qmd` files)