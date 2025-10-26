# 📚 Trends in Toronto Public Libraries (2012–2022)

This project explores how public engagement with the Toronto Public Library (TPL) evolved between 2012 and 2022, analyzing four core metrics: visits, new registrations, circulation of materials, and computer usage. Using open data from the City of Toronto, the research provides a statistical and qualitative overview of how libraries have adapted—and struggled—through technological change and the COVID-19 pandemic.

#### 🎯 Research Objective

This study aims to:
 - **1.** Examine long-term trends in public library usage across four key performance metrics.
 - **2.** Assess the pandemic’s short- and long-term effects on the TPL system.
 - **3.** Provide insights and data-driven recommendations for future improvements in library accessibility, technology integration, and community engagement.

The motivation behind this project is to understand how libraries can evolve in an era of increasing digital access and declining physical engagement, and to highlight their continued social importance.

#### 📈 Research Design & Methodology

This paper is a descriptive statistical analysis, not a predictive model. The methodology focuses on cleaning, merging, and visualizing publicly available datasets to identify multi-year trends.

 - **Software Used:** R (v4.2.2)
 - **Packages:** `tidyverse`, `ggplot2`, `dplyr`, `patchwork`, `janitor`, `knitr`
 - **Data Source:** Open Data Toronto
 - **Datasets Used:**
   - Library Branch General Information — used to distinguish physical vs. non-physical branches.
   - Library Card Registrations
   - Library Circulation
   - Library Visits
   - Library Workstation Usage

Data was cleaned and merged into a single table aligned by branch code and year (2012–2022), containing the four main variables: vistis, regristrations, circulations, and sessions. Non-physical branches (e.g., Bookmobiles, Virtual Library) were excluded to focus on in-person usage.

## 🧠 Discussion & Insights

 - Library popularity has declined since 2012, driven by increasing digital access to information and media.
 - New registrations stand out as a bright spot, suggesting ongoing community engagement and onboarding despite lower physical attendance.
 - Computer usage dropped sharply post-2015, indicating improving personal internet access but also reduced reliance on library technology.
 - COVID-19 caused massive short-term declines, but 2021–2022 data show partial recovery across all variables.

#### 🔍 Key Takeaways

 - Libraries continue to serve as digital access points for those without home internet.
 - COVID-19 accelerated pre-existing declines in physical engagement.
 - Data transparency through open portals like Open Data Toronto enables community-driven research.
 - The recovery trajectory post-2020 highlights the resilience of the TPL system and underscores the need for digital modernization.


## File Structure

The repo is structured as:

-   `input/data` contains the data sources used in analysis including the raw data.
-   `outputs/data` contains the cleaned dataset that was constructed.
-   `outputs/paper` contains the files used to generate the paper, including the Quarto document and reference bibliography file, as well as the PDF of the paper. 
-   `scripts` contains the R scripts used to simulate, download and clean data.
