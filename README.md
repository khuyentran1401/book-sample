# Production Ready Data Science

## Repository Structure

The sample chapter is written in Quarto (`.qmd`) format and is located in [chapters/version_control.qmd](chapters/version_control.qmd).

## Setting Up Your Environment

1. Download and install Quarto from [https://quarto.org/docs/get-started/](https://quarto.org/docs/get-started/).

2. Clone the repository:

   ```bash
   # Fork the repository
   # 1. Go to https://github.com/khuyentran1401/book-sample
   # 2. Click the "Fork" button in the top-right corner
   # 3. Select your GitHub account as the destination

   # Clone the repository
   git clone https://github.com/khuyentran1401/book-sample.git
   cd book-sample
   ```

3. Install uv by following the instructions [here](https://docs.astral.sh/uv/getting-started/installation/).

4. Create and activate virtual environment with uv:

   ```bash
   uv venv

   # Activate the virtual environment
   source .venv/bin/activate  # On Unix/macOS
   # or
   .venv\Scripts\activate  # On Windows
   ```

5. Install dependencies:

   ```bash
   uv sync
   ```

## Contributing to the Book

To contribute to the book, you can follow the steps below:

1. Set up the environment by following the [Setting Up Your Environment](#setting-up-your-environment) section.

2. Create and switch to a new branch:

   ```bash
   git checkout -b your-branch-name
   ```

3. Edit the chapter in [chapters/version_control.qmd](chapters/version_control.qmd) using your favorite text editor. Please refer to the [Quarto Markdown Basics Guide](https://quarto.org/docs/authoring/markdown-basics.html) to learn how to write Quarto markdown.

4. Preview the book to see your changes:

   ```bash
   cd chapters
   quarto preview --no-navigate
   ```

   The sample chapter will be available at [http://localhost:6289/version_control.html](http://localhost:6289/version_control.html).

   You can also render the book to PDF to see your changes:

   ```bash
   quarto render --to pdf
   ```

   The rendered PDF will be available in the `_book` directory.

5. Stage, commit, and push your changes:

   ```bash
   # Stage all changes
   git add .

   # Or stage specific files
   git add path/to/file

   # Commit your changes with a descriptive message
   git commit -m "Your commit message"

   # Push your changes to the remote repository
   git push origin your-branch-name
   ```

6. Create a Pull Request (PR):

   - Go to the repository on GitHub
   - Click on "Pull requests"
   - Click on "New pull request"
   - Select your branch as the compare branch
   - Fill in the PR title and description, explaining your changes
   - Click "Create pull request"