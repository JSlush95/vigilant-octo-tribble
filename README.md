# Word Counter - Enhanced
This project is a web-based visualization tool that allows users to input text and see a graphical representation of the character distribution. It uses D3.js for generating interactive pie and bar charts and Bootstrap for styling.

## Features 
- Text Input: Users can input any text they wish to analyze.
- Character Distribution Visualization: A pie chart displays the distribution of user-defined consonants, vowels, and punctuation marks.
- Detailed Character Count: A bar chart shows the count of each character within the selected category (consonants, vowels, or punctuation).

### Installation
``git clone https://github.com/JSlush95/vigilant-octo-tribble``<br>
### Usage
Open the ``index.html`` file in your preferred browser.

## Technologies Used
- [D3.js](https://d3js.org/) - To create dynamic and interactive data visualizations.
- [Bootstrap](https://getbootstrap.com/) - To design responsive and modern UI.
- JavaScript - To handle the logic and data processing.

## Code Overview
<strong>The main structure of the application is defined in the ``index.html`` file. Key elements include:</strong>
- A text area for user input.
- Two div elements for pie and bar chart visualizations.
- Bootstrap and D3.js integrations for styling and functionality.

<strong>CSS used to make the layout visually appealing and responsive:</strong>
- Styling for ``svg`` elements to set dimensions and background color.
- Tooltip styling for interactivity.
- Text styles.

## JavaScript Logic
<strong>The JavaScript logic handles the text input processing and chart rendering. Key functions include:</strong>

``submitText()``<br>
- Processes the text input and prepares data for visualization.

``processCountData(data)``
- Counts characters, categorizes them into user-defined consonants, vowels, and punctuation, and formats the data for D3.js to use.

``drawDonutChart(donutData, totalData)``<br>
- Draws a pie chart using D3 to visualize the distribution of the defined consonants, vowels, and punctuation.

``drawBarChart(targetSvg, dataType, color, totalData)``<br>
- Draws a bar chart using D3 to show counts of individual characters based on the selected category.

## Tooltips Functionality
<strong>Tooltips provide additional, responsive information when hovering over chart elements. Key aspects include:</strong>
- Contextual displayed tooltip data based on which chart is selected.
- Tooltips follow the mouse cursor for better visibility.
- Tooltip content updates based on the hovered element's data.
