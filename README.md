# CanCOTS 2025 - Interactive Tutorials Working Sub-Group

This repository contains WebR templates and instructions from CanCOTS 2025 in Montreal (10-12 June 2025).

---
## Team Members

### Core Team

| Role | Name | GitHub | Contributions |
|----|----|----|---|
| Team Leader | [Dave Riegert](https://github.com/driegert) | [![GitHub: driegert](https://img.shields.io/badge/GitHub-driegert-lightgrey?logo=github)](https://github.com/driegert) | Provided training, led group and wrote instructions in the README file. |
| Contributor | [Kyran Cupido](https://github.com/cupidok) | [![GitHub: cupidok](https://img.shields.io/badge/GitHub-cupidok-lightgrey?logo=github)](https://github.com/cupidok) | Added sample activities and simulations. |
| Contributor | [Nishan Mudalige](https://github.com/nishanmudalige) | [![GitHub: nishanmudalige](https://img.shields.io/badge/GitHub-nishanmudalige-lightgrey?logo=github)](https://github.com/nishanmudalige) | Added sample tutorials, merged contributions, partially updated README. |
| Contributor | [Irene Vrbik](https://github.com/vrbiki) | [![GitHub: vrbiki](https://img.shields.io/badge/GitHub-vrbiki-lightgrey?logo=github)](https://github.com/vrbiki) | Created the skeleton course with sample slides. |
| Participant | [Allan Majdanac](https://github.com/majdanaca) | [![GitHub: majdanaca](https://img.shields.io/badge/GitHub-majdanaca-lightgrey?logo=github)](https://github.com/majdanaca) | Testing. |

### Additional Support

| Role | Name | GitHub | Contributions |
|----|----|----|---|
| Organizing Committee | [Léo Raymond-Belzile](https://github.com/lbelzile) | [![GitHub: lbelzile](https://img.shields.io/badge/GitHub-lbelzile-lightgrey?logo=github)](https://github.com/lbelzile) | Provided additional training and guidance, helped with troubleshooting. |
| Technical support | [Aarushi Alreja](https://github.com/aarushi-codes) | [![GitHub: aarushi-codes](https://img.shields.io/badge/GitHub-aarushi--codes-lightgrey?logo=github)](https://github.com/aarushi-codes) | Technical assistance with GitHub. |
| Technical support | [Kabir Bhatia](https://github.com/kabir-codes) | [![GitHub: kabir-codes](https://img.shields.io/badge/GitHub-kabir--codes-lightgrey?logo=github)](https://github.com/kabir-codes) | Technical assistance with GitHub. |

---

## Deliverable: Sample Course (Slides, Activities, Tutorials)

The deliverable for the sub-group is a skeleton of a course consisting of

- A sample course landing page
- Sample slides made in `quarto`
- Sample interactive activities made with `learnr` and `webr`
- Sample interactive tutorials made with `learnr`, `webr` and `gradethis`

<br>

A template for a sample course can be viewed by [**clicking here**](https://nishanmudalige.github.io/CanCOTS_2025_Interactive_R_Tutorials/).

---

## Additional Resources

| Resource | Description | Link |
|---|---|---|
| **Quarto Slides** | Quarto and Reveal.js slide for statistics and data science courses created by [Irene Vrbik](https://github.com/vrbiki). | [View slides](https://irene.vrbik.ok.ubc.ca/courses/) |
| **Activities and Simulations** | Interactive `webR` activities and simulations created by [Kyran Cupido](https://cupidok.github.io/). | [View activities](https://cupidok.github.io/stats/) |
| **Tutorials** | STA258 interactive tutorials created by [Nishan Mudalige](https://github.com/nishanmudalige) using `webR` and `learnr`. | [View tutorials](https://nishanmudalige.github.io/STA258_Tutorials/) |


---
# Prerequisites

The steps below are from [https://quarto-webr.thecoatlessprofessor.com/](https://quarto-webr.thecoatlessprofessor.com/).

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
    - Mac: Open the Terminal (can be found in Launchpad) and run:
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

## Fork the `CanCOTS_2025_Interactive_R_Tutorials` Repository

Next, fork the repository to your own GitHub account by clicking the "Fork" button in the top right corner of this page. This will create a copy of the repository in your account.

## Making the Document Available

1. Go to your forked repository on Github.
2. Replace the contents of `README.md` (THIS FILE, maybe!) with your own content.
3. Click on the repository settings (next to "Insights")
4. Click on "Pages" on the left menu.
5. Ensure you have "Deploy from a branch" selected and then under "Branch", select "main". Click "Save".



# Steps
To use this template you should:

1. Download R
2. Download RStudio
3. Install Quarto: [https://quarto.org/docs/get-started/](https://quarto.org/docs/get-started/)
4. Make sure you do not already have a version of TinyTex installed:
In the command line, run:
```bash
quarto uninstall tinytex
```
5. Install the latest version of TinyTex:
```bash
quarto install tinytex
```
6. Install `rwasm` (Build R Packages for WebAssembly)
```bash
# install.packages("pak")
pak::pak("r-wasm/rwasm")
```

7. Create a new directory for your Web-R files (file explorer, terminal, etc.).
8. From the command line, navigate to the direcotry you created in the last step and run:
```bash
quarto add coatless/quarto-webr
```
1. Download the template to the directory that you created (the .qmd file should be in the same directory as the `_extensions` directory.)
   - html (recommended)
   1. revealjs (for slides; there are vertical space issues, however!)
9. Open the .qmd file in RStudio.
10. Press the "Render" button (top of the script pane).
