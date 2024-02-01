
# USClinicalTrialsDashboard

This R Shiny app displays a live map of the current active clinical trials in the United States with information on their phase and lifecycle.

1. Running Locally

- To run this app locally, ensure you have R and the Shiny package installed. Clone this repository, open `app.R` in RStudio or VS Code, and click 'Run App'.

 ```R
install.packages("shiny")

- Clone this repository to your local machine and open your IDE. Set your directory to the cloned repository if you are using RStudio or another R environment.

- Run the app

shiny::runApp()


2. Testing and deployment

- Test your modified app thoroughly in your local development environment prior to deploying to shinnyapps.io to ensure all features work correctly. Then install and load the 'rsconnect' package:

install.packages("rsconnect")
library(rsconnect)

- Set up your shinyapps.io account information.

rsconnect::setAccountInfo(name='YOUR_ACCOUNT_NAME', token='YOUR_TOKEN', secret='YOUR_SECRET')

- Complete the deployment of your new app with the following, and update 'path/to/your/app' with the actual path to your shinny application directory.

rsconnect::deployApp('path/to/your/app')

3. Data Source

Data is dynamically fetched from ClinicalTrials.gov.

4. License

This project is licensed under the BSD 2-Clause "Simplified" License. For more information, please see the 'LICENSE' file.
