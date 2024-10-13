# Linier Regression Dashboard

## Overview

This Shiny dashboard application provides an interactive interface for exploring data, building linear regression models, and visualizing results. It's designed to be user-friendly and informative, allowing users to upload their own datasets and perform basic machine learning tasks without writing code.

## Features

- Data upload (CSV and XLSX formats supported)
- Data preview and summary statistics
- Correlation analysis with visualizations
- Linear regression modeling
- Variable importance analysis
- Model performance visualization
- Diagnostic plots

## Installation

### Prerequisites

- R (version 4.0.0 or higher recommended)
- RStudio (for easy project management and Shiny app launching)

### Required R Packages

Install the following R packages before running the application:

```r
install.packages(c("shiny", "shinydashboard", "dplyr", "ggplot2", "DT", "plotly", "corrplot", "caret", "stargazer", "readxl", "shinycssloaders"))
```

### Setup

1. Clone this repository or download the source code.
2. Open the project in RStudio.
3. Ensure all required packages are installed.

## Usage

1. In RStudio, open either `ui.R` or `server.R`.
2. Click the "Run App" button in the top-right corner of the script editor.
3. The Shiny dashboard will launch in a new window.

### Data Upload

- Use the "Upload Data" button in the sidebar to upload your CSV or XLSX file.
- If no file is uploaded, the app will use the built-in `mtcars` dataset as an example.

### Data Exploration

- The "Data" tab shows a preview of your dataset and summary statistics.
- The "Analysis" tab allows you to select variables and view correlation plots.

### Modeling

- In the "Analysis" tab, select your predictor variables (X) and target variable (Y).
- Adjust the train/test split percentage in the sidebar if desired.
- The "Model" tab will display the linear regression results, variable importance, and diagnostic plots.

## Customization

You can easily extend this dashboard by modifying the `ui.R` and `server.R` files:

- Add new visualizations in `server.R` and create corresponding outputs in `ui.R`.
- Implement additional modeling techniques by adding new reactive functions in `server.R`.
- Customize the UI layout and styling in `ui.R`.

## Contributing

Contributions to improve the dashboard are welcome. Please feel free to submit pull requests or open issues to suggest improvements or report bugs.

## License

This project is open source and available under the [MIT License](LICENSE).

## Contact

For any questions or feedback, please open an issue in the GitHub repository.

Happy analyzing!
