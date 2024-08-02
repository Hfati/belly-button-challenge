# belly-button-challenge
This project visualizes the biodiversity of bacterial species found in human navels using interactive charts and demographic information.
The dataset reveals that a small handful of microbial species (also called operational taxonomic units, or OTUs) were present in more than 70% of people, while the rest were relatively rare.

## Table of Contents

- [Belly Button Biodiversity Dashboard](#belly-button-biodiversity-dashboard)
  - [Overview](#overview)
  - [Table of Contents](#table-of-contents)
  - [Files in the Repository](#files-in-the-repository)
  - [Instructions](#instructions)
    - [Horizontal Bar Chart](#horizontal-bar-chart)
    - [Bubble Chart](#bubble-chart)
    - [Demographic Info](#demographic-info)
    - [Updating Charts](#updating-charts)
  - [Deployment](#deployment)
  - [Technologies Used](#technologies-used)
  - [Credits](#credits)
  - [License](#license)

## Files in the Repository

- `index.html`: The main HTML file that contains the structure of the dashboard.
- `static/js/app.js`: The JavaScript file containing the logic for fetching data and rendering charts.
- `static/css/style.css`: The CSS file for styling the dashboard.
- `samples.json`: The dataset containing the OTU and demographic information.

## Instructions

1. Use the D3 library to read in `samples.json` from the URL provided.
2. Create interactive charts using Plotly.js to visualize the data.

### Horizontal Bar Chart

- Displays the top 10 OTUs found in each individual.
- Uses `sample_values` as the values for the bar chart.
- Uses `otu_ids` as the labels for the bar chart.
- Uses `otu_labels` as the hovertext for the chart.

### Bubble Chart

- Displays each sample.
- Uses `otu_ids` for the x values.
- Uses `sample_values` for the y values.
- Uses `sample_values` for the marker size.
- Uses `otu_ids` for the marker colors.
- Uses `otu_labels` for the text values.

### Demographic Info

- Displays an individual's demographic information.
- Loops through each key-value pair from the metadata JSON object and appends it to the `#sample-metadata` panel.

### Updating Charts

- Updates all plots when a new sample is selected.
- Creates a dropdown menu for selecting different individuals.

## Deployment

1. Create a new repository for this project called `belly-button-challenge`.
2. Clone the new repository to your computer.
3. Copy the files from the `StarterCode` folder contained within the Module 14 Challenge zip file to your local repository.
4. Push the changes to GitHub.
5. Deploy the new repository to GitHub Pages.

## Technologies Used

- HTML
- CSS (Bootstrap)
- JavaScript
- D3.js
- Plotly.js
- GitHub Pages

## Credits

Data for this project was provided by the U.S. 2020 Decennial Census and retrieved from [https://data.census.gov/cedsci/](https://data.census.gov/cedsci/).

## License

This project is licensed under the MIT License.
