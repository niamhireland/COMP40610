# Data Visualisation with Vega-Lite

<img width="852" alt="Screenshot 2025-01-16 at 10 22 29" src="https://github.com/user-attachments/assets/632c67a8-3d6d-4c23-9892-4663b2f6e28c" />

## About the project 
This project explores the distribution of global independence days by season and how they relate to colonising nations. 

It includes the following features: 
* A bar chart to show the most prolific colonising nations in the world, sorted in descending order. 
* A choropleth map to display the geographic distribution of countries celebrating independence, along with the season they celebrate in.
* A line chart to visualise the spread of independence days across the calendar year, grouped by month.

This project is interactive and focuses on cross-filtering. The user can select a bar in the bar chart, which will cause the countries associated with this colonising nation to be highlighted on the choropleth map. The line chart will also update, now only showing trends of independence days associated with that coloniser. 

Additionally, a tooltip is active on the choropleth map. The user can hover over a country to ascertain details, such as the name of their independence day, the specific country they are celebrating independence from and the exact date of the holiday.

## Running the project 
To explore the project, copy the 'json_file' from the repository. Then, go to https://vega.github.io/editor/ . 
Once you paste the 'json_file' contents into the configuration window there, the project will appear. 

## Technologies used
This project was built using the following technologies:

* [![JSON][JSON]][JSON-url]
* [![Vega-Lite][Vega-Lite]][Vega-Lite-url]
* [![Jupyter Notebook][Jupyter]][Jupyter-url]

## Visualisation decisions made 

I opted to use aggregate groupings when creating the bar chart. This was done because many countries have only colonised one or two other countries, which made the bar chart very long and difficult to understand. These countries have been grouped together under the "Other" label. Additionally, some nations celebrate independence but are not actually celebrating being independent from another country. These celebrations have been grouped under the "None" label. You can see an example of this in the screenshot above, as Australia celebrates Australia Day but does not actually celebrate independence from the United Kingdom. 

The above does cause users to lose some depth of insight. Offering the tooltip is a means of compensating for this. The user can select the Other or None bar and then, guided by the highlighting on the map, hover over the country to ascertain exactly which coloniser is being referred to. 

## Acknowledgements

The dataset behind this project was provided by the Tidy Tuesdays project on GitHub. I performed additional cleaning and infilling on the dataset, in order to meet my project needs. The original can be viewed at: https://github.com/rfordatascience/tidytuesday/blob/main/data/2021/2021-07-06/readme.md

In conjunction with the Tidy Tuesdays project, I utilised a GeoJSON file to render the world map. The original of this was provided by GitHub user alexabruck.
The original can be viewed at: https://github.com/alexabruck

This project was originally completed for UCD's COMP40610: Information Visualisation module. Many thanks to my lecturer Dr. Hamda Ajmal for her support during this time.

<!-- MARKDOWN LINKS & IMAGES -->
[JSON]: https://img.shields.io/badge/JSON-000000?style=for-the-badge&logo=json&logoColor=white
[JSON-url]: https://www.json.org/

[Vega-Lite]: https://img.shields.io/badge/Vega--Lite-1A9CC5?style=for-the-badge&logo=vega-lite&logoColor=white
[Vega-Lite-url]: https://vega.github.io/vega-lite/

[Jupyter]: https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white
[Jupyter-url]: https://jupyter.org/
