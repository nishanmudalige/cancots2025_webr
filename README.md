# Your WebR Project Setup Guide

This guide provides instructions for setting up and deploying your WebR project using GitHub Pages.

---

## Option 1: Forking and Hosting an Existing Repository

This is the quickest way for your colleagues to get started with a pre-existing WebR project.

1.  **Create a GitHub Account**: If you don't already have one, create a GitHub account by visiting <https://github.com/> and clicking "Sign up".
2.  **Fork the WebR Repository**:
    * Navigate to the WebR project repository on GitHub.
    * Click the "**Fork**" button in the top right corner of the page. This creates a copy of the repository in your personal GitHub account.
3.  **Enable GitHub Pages**:
    * Go to your forked repository on GitHub.
    * Click on "**Settings**" (usually found near "Insights").
    * In the left-hand menu, click on "**Pages**".
    * Under "Source", ensure "**Deploy from a branch**" is selected.
    * Under "Branch", select `main` (or `master` if your default branch is named `master`) and click "**Save**".

    GitHub Pages will then build and deploy your WebR HTML file. This process may take a few minutes. Once deployed, a link to your live site will appear on the same "Pages" settings page.

---

## Option 2: Creating a New Repository from Scratch

This option is for colleagues who prefer to set up their WebR project from the ground up and then incorporate the template's content.

### Prerequisites

You will need the following software installed on your computer:

* **R**: Download from <https://cran.r-project.org/>
* **RStudio**: Download from <https://posit.co/download/rstudio-desktop/>
* **Quarto**: Install from <https://quarto.org/docs/get-started/>
* **TinyTex**:
    * **Windows**: Open Command Prompt (Windows Key + R, type `cmd`, press Enter) and run:
        ```bash
        quarto uninstall tinytex
        quarto install tinytex
        ```
    * **Mac**: Open Terminal (found in Launchpad) and run:
        ```bash
        quarto uninstall tinytex
        quarto install tinytex
        ```

### Steps to Create a New Repository and Use the Template

1.  **Create a New Directory**: Create a new directory on your computer where you will store your WebR files (e.g., using your file explorer or terminal).
2.  **Add Quarto WebR Extension**: From your command line, navigate to the directory you just created and run:
    ```bash
    quarto add coatless/quarto-webr
    ```
    This command will create an `_extensions` directory within your project, which is necessary for WebR functionality.
3.  **Copy Template Contents**: Copy the content from your provided `webr-html_template.html` file into a new `.qmd` file (e.g., `my_webr_project.qmd`) in the same directory as the `_extensions` folder. You will also need to ensure the `webr-html_template_files` folder is copied alongside it.
4.  **Render in RStudio**: Open the newly created `.qmd` file in RStudio. Press the "**Render**" button (located at the top of the script pane). This will generate the WebR HTML output.
5.  **Create a New GitHub Repository**:
    * Go to <https://github.com/new> to create a new, empty repository. Give it a meaningful name (e.g., `my-webr-project`).
    * Do not initialize it with a `README`, `.gitignore`, or license, as you will push your local files.
6.  **Push Your Project to GitHub**:
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
7.  **Enable GitHub Pages**: Follow steps 3-6 from "Option 1: Forking and Hosting an Existing Repository" above.





# OLD OLD OLD DO NOT USE

# cancots2025_webr
WebR templates and instructions from CanCOTS 2025 in Montreal (June 10-12).

You can view the template, rendered to HTML, by [clicking here](https://driegert.github.io/cancots2025_webr/webr-html_template.html)

The steps below are from [https://quarto-webr.thecoatlessprofessor.com/](https://quarto-webr.thecoatlessprofessor.com/).

# Prerequisites

## Software

You will need the following:

- R, RStudio, Quarto, and TinyTex installed on your computer:
  - R: [https://cran.r-project.org/](https://cran.r-project.org/)
  - RStudio: [https://posit.co/download/rstudio-desktop/](https://posit.co/download/rstudio-desktop/)
  - Quarto: [https://quarto.org/docs/get-started/](https://quarto.org/docs/get-started/)
  - TinyTex:
    - Windows: Windows Key + R, then type `cmd` and press Enter to open the command line. Run:
        ```bash
        quarto uninstall tinytex
        ```
        and then
        ```bash
        quarto install tinytex
        ```
    - Mac: Open the Terminal (can be found in Launchpad and run:
        ```bash
        quarto uninstall tinytex
        ```
        and then
        ```bash
        quarto install tinytex
        ```

## Github Account

If you don't have a Github account, create one by going to [https://github.com/](https://github.com/)
  - go to "Sign up" in the top right corner

## Fork the `cancots2025_webr` Repository

Next, fork the repository to your own GitHub account by clicking the "Fork" button in the top right corner of this page. This will create a copy of the repository in your account.

## Making the Document Available

1. Go to your forked repository on Github.
2. Replace the contents of README.md (THIS FILE, maybe!) with your own content.
3. Click on the repository settings (next to "Insights")
4. Click on "Pages" on the left menu.
5. Ensure you have "Deploy from a branch" selected and then under "Branch", select "main". Click "Save".










# Steps
To use this template you can:

1. Download R
2. Download RStudio
3. Install Quarto: [https://quarto.org/docs/get-started/](https://quarto.org/docs/get-started/)
4. Make sure you do not already have a version of TinyTex installed:
In the command line, run:
```bash
quarto uninstall tinytex
```
5. Install the latest versino of TinyTex:
```bash
quarto install tinytex
```
6. Create a new directory for your Web-R files (file explorer, terminal, etc.).
7. From the command line, navigate to the direcotry you created in the last step and run:
```bash
quarto add coatless/quarto-webr
```
1. Download the template to the directory that you created (the .qmd file should be in the same directory as the `_extensions` directory.)
   - html (recommended)
   1. revealjs (for slides; there are vertical space issues, however!)
9. Open the .qmd file in RStudio.
10. Press the "Render" button (top of the script pane).
