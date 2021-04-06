# predictive_testing_overview

## BYU-I Office of Teacher Preparation

**There are four repositories associated with this project.** Check out their individual READMEs for more details.

### [SP_praxis](https://github.com/byuiR/SP_praxis)

Contains the raw student data and the tidy version of said data used for training models. Also contains all of the necessary scripts for cleaning and tidying the data, as well as scripts for EDA and creating the final model. **Because this repo contains sensitive personal data, it should remain private.**

### [byui_praxis_predictor](https://github.com/byuiR/byui_praxis_predictor)

The website that acts as the user interface for the predictive model. Made with vanilla HTML, CSS, and JavaScript. The website makes a POST request to the [plumber](https://www.rplumber.io/) API stored in *plamodel*. Students upload a PDF transcript that is scraped by functions from the *tidytranscript* R pacakge.

### [tidytranscript](https://github.com/byuiR/tidytranscript)

An R package used to scrape PDF transcripts of BYUI students. These functions are used in the API in *plamodel*.

### [plamodel](https://github.com/byuiR/plamodel/tree/master/plumber-api)

Contains the plumber API. Focus on the *plumber-api* directory, which contains the scripts that create the API endpoints, predicts on new data, and help pre-process the new data that is used for prediction.
