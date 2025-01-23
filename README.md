# Belly Button Biodiversity Dashboard

This project is an interactive dashboard designed to explore the Belly Button Biodiversity dataset. The dataset provides information about bacterial species found in human navels. The dashboard enables users to interact with charts and demographic metadata for various test subjects.

## Features

- **Dropdown Menu**: Select a test subject ID to dynamically update charts and metadata.
- **Demographic Information Panel**: Displays detailed demographic data for the selected test subject.
- **Interactive Charts**:
  - **Horizontal Bar Chart**: Shows the top 10 bacterial species (OTUs) for the selected sample.
  - **Bubble Chart**: Visualizes the distribution of all OTUs for the selected sample.
- **Responsive Design**: Built using Bootstrap for a clean and responsive layout.

## Project Files

- `index.html`: The main HTML file containing the dashboard structure and references to external libraries.
- `app.js`: JavaScript code that handles data loading, chart creation, and interactivity.
- `samples.json`: Hosted dataset providing metadata and bacterial sample data.

## Technologies Used

- **HTML/CSS**: For the layout and styling of the dashboard.
- **JavaScript**: For interactivity and dynamic data handling.
- **D3.js**: To fetch and manipulate data.
- **Plotly.js**: To create interactive charts.
- **Bootstrap**: For responsive design and styling.

## How to Use

1. Clone the repository to your local machine.
   ```bash
   git clone https://github.com/your-username/belly-button-biodiversity.git
   ```

2. Navigate to the project directory.
   ```bash
   cd belly-button-biodiversity
   ```

3. Open `index.html` in a web browser.

4. Use the dropdown menu to select a test subject ID and explore the charts and metadata.

## Code Structure

### `app.js`

- **`buildMetadata(sample)`**:
  - Fetches and displays demographic metadata for the selected sample.

- **`buildCharts(sample)`**:
  - Generates the bubble chart and horizontal bar chart for the selected sample.

- **`init()`**:
  - Initializes the dashboard by populating the dropdown menu and displaying data for the first sample.

- **`optionChanged(newSample)`**:
  - Updates the metadata and charts when a new sample is selected from the dropdown.

### `index.html`

- Defines the layout and structure of the dashboard.
- Includes sections for the dropdown menu, demographic panel, and charts.
- References external libraries and `app.js`.

## Deployment

To deploy this project:

1. Push the project to a GitHub repository.
2. Use GitHub Pages to host the dashboard:
   - Go to the repository's settings.
   - Enable GitHub Pages in the "Pages" section.
3. Share the deployment link.

## Dataset

The dataset is hosted at:
```
https://static.bc-edx.com/data/dl-1-2/m14/lms/starter/samples.json
```

It includes:
- **Metadata**: Demographic info for each test subject.
- **Sample Data**: OTU IDs, labels, and values for each sample.

## Acknowledgments

This project was developed as part of a data visualization challenge. Special thanks to the Bootcamp team for providing the dataset and guidelines.



