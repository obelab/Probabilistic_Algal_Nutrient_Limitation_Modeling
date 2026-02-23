<h1 align="center">Probabilistic assessment of algal nutrient limitation across lakes, leveraging trends with temperature and depth</h1>

<p align="center">
  <strong>Brian  W. Baird<sup>1,§</sup>, Smitom S. Borah<sup>1</sup>, James J. Elser<sup>2</sup></strong> , Daniel R. Obenour<sup>1,3</sup></strong>
</p>

<p align="center">
  <sup>1</sup>Department of Civil, Construction, and Environmental Engineering, North Carolina State University, Raleigh, NC, 27606, USA<br>
  <sup>2</sup>2Division of Biological Sciences and Flathead Lake Biological Station, University of Montana, Polson, Montana 59860, USA <br>
  <sup>3</sup>3Center for Geospatial Analytics, North Carolina State University, Raleigh, North Carolina 27695, USA <br>
  <sup>§</sup>Kimley-Horn and Associates, Inc., Dallas, Texas, 75240, USA
</p>


## Table of Contents

- [About the Project](#about-the-project)
- [Getting Started](#getting-started)
- [Running Codes](#Running-Codes)

## About The Project

**Abstract**

Lake eutrophication remains a significant challenge for water-quality management across the world. Many management strategies focus on reducing nutrient inputs, but other environmental factors can substantially influence the yield of algal biomass for a given level of nutrients. While various large-scale studies have explored how different lake characteristics impact eutrophication, there remains a need to integrate these factors into a comprehensive model capable of assessing nitrogen versus phosphorus limitation. In this study, we refine chlorophyll-nutrient relationships across the conterminous United States by considering auxiliary variables (e.g., temperature, lake depth, nutrient enrichment) within a Bayesian hierarchical framework. We leverage over 4000 sampling events of 2755 different lakes from the National Lakes Assessments (2007-2022) to inform model development. We first consider auxiliary variables independently, exploring how they influence the intercept, slope, and critical nutrient ratio (nitrogen:phosphorus) in a regression to predict chlorophyll based on the limiting nutrient. Next, we integrate significant auxiliary variables into a comprehensive model for chlorophyll prediction. Results indicate that the critical nutrient ratio increases in relation to increased lake depth, and the slope of the nutrient-chlorophyll relationship increases with increasing temperature. We apply the model to map mean summer conditions across United States lakes and find that 23% and 16% of lakes are strongly limited by phosphorus and nitrogen, respectively (i.e., at > 90% probability). These proportions, however, vary substantially across different subregions. Overall, the probabilistic modeling approach and results can serve as an effective tool to inform water resources management, especially at large spatial scales.

In this repository, we provide the data and models developed as a part of our study. The data needed to run the codes are stored in *data* folder, the model codes are stored in *codes* folder, and the nutrient limitation data are stored in the *outputs* folder. The details of the files in these folders are provided in the corresponding ReadMe files.

## Getting Started

The codes in this project are developed in R environment. To install and run R and RStudio on your computer, follow these steps:

### Installing R

1. **Download R:**
   - Visit the [CRAN website](https://cran.r-project.org/).
   - Select your operating system: Windows, macOS, or Linux.
   - Click on the appropriate link to download the R installer.

2. **Install R on Windows:**
   - Click on "Download R for Windows" and then on "base."
   - Download the latest version of R by clicking the link at the top of the new page.
   - Run the downloaded `.exe` file and follow the installation wizard steps.

3. **Install R on macOS:**
   - Click on "Download R for macOS."
   - Download the `.pkg` file for the latest version of R.
   - Run the `.pkg` file and follow the installation instructions.

### Installing RStudio

1. **Download RStudio:**
   - Go to the [RStudio website](https://www.rstudio.com/products/rstudio/download/).
   - Click on "DOWNLOAD" under the RStudio Desktop section.

2. **Install RStudio:**
   - Download the installer for your operating system (Windows `.exe` or macOS `.dmg`).
   - Run the installer and follow the installation prompts.

### Running R and RStudio

1. **Open RStudio:**
   - After installation, open RStudio from your Start menu (Windows) or Applications folder (macOS).

2. **Set Up RStudio:**
   - The RStudio interface consists of multiple panes: Source, Console, Environment, and Files/Plots/Packages/Help.
   - You can write R scripts in the Source pane and execute them in the Console.

3. **Install and Load Packages:**
   - Install packages using `install.packages("packageName")`.
   - Load packages using `library(packageName)`.

### Additional Resources

For detailed guides and additional resources on installing and using R and RStudio, you can refer to these tutorials:

- [Dataquest: Downloading and Installing R](https://www.dataquest.io/blog/installing-r-on-your-computer/)
- [Stats and R: How to install R and RStudio](https://statsandr.com/blog/how-to-install-r-and-rstudio/)
- [Hands-On Programming with R: Installing R and RStudio](https://rstudio-education.github.io/hopr/a-intro.html)

These guides provide comprehensive instructions and helpful visuals to ensure a smooth installation process.

## Running Codes
Here's a step-by-step guide to how to the codes given here in RStudio:

### Forking a GitHub Repository

1. **Log in to GitHub:**
   - Go to [GitHub](https://github.com) and log in to your account.

2. **Find the Repository:**
   - Navigate to the repository you want to fork. You can use the search bar at the top of the GitHub page.

3. **Fork the Repository:**
   - In the upper right-hand corner of the repository page, click the `Fork` button. This will create a copy of the repository under your GitHub account.

4. **Clone the Forked Repository:**
   - Go to your GitHub profile and find the forked repository.
   - Click on the `Code` button and copy the URL (HTTPS, SSH, or GitHub CLI) of the repository.

### Cloning the Repository in RStudio

1. **Open RStudio:**
   - Launch RStudio on your computer.

2. **Create a New Project:**
   - Go to the `File` menu, select `New Project`, then choose `Version Control`, and then `Git`.

3. **Clone the Repository:**
   - In the `Repository URL` field, paste the URL you copied from GitHub.
   - Choose a directory where you want to store the project locally.
   - Click `Create Project`. RStudio will clone the repository and open it as a new project.

### Running the Code in RStudio

1. **Explore the Project:**
   - In the `Files` pane of RStudio, you can see all the files in the cloned repository.

2. **Open Scripts:**
   - Double-click on any R notebook (`.RMD` file) to open it in the `Source` pane.

3. **Install Required Packages:**
   - If the project depends on specific R packages, install them using `install.packages("packageName")`.
   - You can find a list of required packages within the script itself (usually at the top in the form of `my_packages <- c(packageName,...)`).

4. **To run code chunks interactively:**
   - Click the green play button (▶) at the top right of each code chunk.
   - Or press Ctrl+Shift+Enter (Windows/Linux) or Cmd+Shift+Enter (Mac) to run the current code chunk.
   - You can also run entire codes with Ctrl+Alt+R (Windows) or Cmd+Option+R (Mac).

### Additional Resources
For further details, refer to these resources:
- [GitHub Docs: Fork a repo](https://docs.github.com/en/get-started/quickstart/fork-a-repo)
- [RStudio Support: Version Control with Git and SVN](https://support.rstudio.com/hc/en-us/articles/200532077-Version-Control-with-Git-and-SVN)
- [Happy Git and GitHub for the useR](https://happygitwithr.com/) - A comprehensive guide on using Git with R.



