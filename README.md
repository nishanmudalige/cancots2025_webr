# Your WebR Project Setup Guide

This guide provides instructions for setting up and deploying your WebR project using GitHub Pages.

---

## Option 1: Forking and Hosting an Existing Repository

This is the quickest way for your colleagues to get started with a pre-existing WebR project.

1.  **Create a GitHub Account**: If you don't already have one, create a GitHub account by visiting <https://github.com/> and clicking "Sign up".
2.  **Fork the WebR Repository**:
    * Navigate to the WebR project repository on GitHub.
    * Click the "**Fork**" button in the top right corner of the page. This creates a copy of the repository in your personal GitHub account.  
    You will use this repository to create and modify your WebR Quarto (.qmd) files. You may want to make this repository private if you do not want to share the content with others (e.g., students).
3. Create a lesson in RStudio based on the Quarto (.qmd) templates provided and that you want to share with students.  
Render the lesson to HTML. You will create a .html file and a `<your_file_name>_files/` directory.
4. Create a new directory on your computer and copy over:
    - `_extensions/` folder
    - `<your_file_name>_files/`
    - `<your_file_name>.html`
    - `CHANGEMYNAME.md` - change this to `README.md` and ensure that you have edited the links appropriately to match your filenames.  
    Your directory structure should look like:
    ```
    <directory name you just created>
    ├── _extensions
    ├── <your_filename>_files
    ├── <your_filename>.html
    └── README.md
    ```
5.  **Create a New GitHub Repository**:
> [!NOTE]
> This will be the repository you will use for the course for the semester.
    - Go to <https://github.com/new> to create a new, empty repository. Give it a meaningful name (e.g., `math200-fall2025`).
    - Do **NOT** initialize it with a `README`, `.gitignore`, or license, as you will push your local files.
4.  **Push Your Project to GitHub**:
    * Open your terminal or Git Bash.
    * Navigate to your project directory.
    * Initialize a Git repository: `git init`
    * Add your files: `git add .`
    * Commit your changes: `git commit -m "Initial WebR project"`
    * Add the remote origin (replace `YOUR_USERNAME` and `YOUR_REPOSITORY_NAME` with your actual GitHub username and repository name):
        ```bash
        git remote add origin [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)
        ```
    * Push your local project to GitHub: `git push -u origin main` (or `master` if that's your default branch name).
5.  **Enable GitHub Pages**:
    * Go to your forked repository on GitHub.
    * Click on "**Settings**" (usually found near "Insights").
    * In the left-hand menu, click on "**Pages**".
    * Under "Source", ensure "**Deploy from a branch**" is selected.
    * Under "Branch", select `main` (or `master` if your default branch is named `master`) and click "**Save**".

    GitHub Pages will then build and deploy your WebR HTML file. This process may take a few minutes. Once deployed, a link to your live site will appear on the same "Pages" settings page.
    
The README.md file should contain links to your lesson `.html` files.

```markdown
[The text that will be displayed](https://your_username.github.io/your_file.html)
```