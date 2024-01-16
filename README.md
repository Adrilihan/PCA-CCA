The code in this repository is an implementation of the methodology developed by
[Samadi et al. (2017)](https://link.springer.com/article/10.1007/s00180-016-0667-1) 
that combines Principal Component Analysis (PCA) and Canonical Correlation 
Analysis (CCA) methods to incorporate the time dependencies of time-series data.
This implementation was developed as a project for the curriculum unit 
"Estatística Multivariada" given by [Adelaide Freitas](https://www.ua.pt/pt/p/10310341) 
at the University of Aveiro. 

The implementation uses the [NCAR Research Data Archive](https://rda.ucar.edu/) 
dataset ([ds578.1](https://rda.ucar.edu/datasets/ds578.1/)), which contains 
monthly mean surface temperature (degrees C) and monthly accumulated 
precipitation (millimetres) from 160 land stations in China from 1951 to 2000. 
Only the temperature data was used for this project and it's located in the 
files `ch160sta.txt` and `ch160temp.txt`.

The code was featured on a poster via a QR code for the 
[One Day Meeting CIDMA conference](https://sites.google.com/view/one-daymeeting-cidma).

# Installation

1. **Download the repository**: You can download this repository to your local 
machine either by cloning it or by downloading it as a zip file.

   - To clone the repository, use the following command in your terminal:

    ```bash
    git clone https://github.com/Adrilihan/PCA-CCA.git
    ```

   - To download the repository as a zip file, click on the `Code` button on the
   repository page and then click `Download ZIP`. Extract the zip file to your 
   desired location.

2. **Open the R project**: Navigate to the directory where you downloaded the 
repository and open the `PCA-CCA.Rproj` file. This will start the R environment 
with the correct working directory.

3. **Install the required packages**: This project uses the `renv` package for 
dependency management. If you don't have `renv` installed, you can install it 
using the following command in the R console:

    ```r
    install.packages("renv")
    ```

    Then, to install the project dependencies, use the following command:

    ```r
    renv::restore()
    ```

4. **Run the R Markdown file**: Finally, you can run the `PCA.Rmd` file to 
execute the code and generate the report.

Please note that this project was developed in R, so you need to have R 
installed on your machine. If you don't have R installed, you can download it 
from [The Comprehensive R Archive Network (CRAN)](https://cran.r-project.org/mirrors.html).

# Usage

Currently, this repository contains an R Markdown file, `PCA.Rmd`, which 
provides a detailed walkthrough of the steps taken to format the data and apply 
the PCA-CCA methodology. Users can refer to this file to understand the process 
and use the code provided.

In the future, we aim to develop a function that can perform the analysis given formatted data. Please stay tuned for updates.

# License

This project is licensed under the MIT License. See the LICENSE file for 
details.


# References

Data: https://rda.ucar.edu/datasets/ds578.1/

Paper: https://link.springer.com/article/10.1007/s00180-016-0667-1

PCA wiki: https://en.wikipedia.org/wiki/Principal_component_analysis

CCA wiki: https://en.wikipedia.org/wiki/Canonical_correlation

R plotly package documentation: https://plotly.com/r/

CCA R implementation: https://cmdlinetips.com/2020/12/canonical-correlation-analysis-in-r/
