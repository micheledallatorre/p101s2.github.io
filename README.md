# Info #

DEMO: [https://micheledallatorre.github.io/p101s2/](https://micheledallatorre.github.io/p101s2/)

This project is a D3.js interactive ranking chart based on [Produce 101 Season 2 Rankings](https://p101s2.github.io/).

I extended the original project by loading data dynamically from a shared (and published to the web) Google Sheet file (see details below and in commit [https://github.com/micheledallatorre/p101s2/commit/971314ce06698de25cd805ddb5da1199477f7c17](https://github.com/micheledallatorre/p101s2/commit/971314ce06698de25cd805ddb5da1199477f7c17 "https://github.com/micheledallatorre/p101s2/commit/971314ce06698de25cd805ddb5da1199477f7c17")). 

> An interactive ranking chart for MNet's Produce 101 Season 2 made with d3.js. I began this project around Episode 4 in order to better keep track of the numerous contestants and also in hopes of being able to better predict the final 11 winners. I updated this website after each episode as the season progressed. This site now displays the full rankings and final results for each contestant.
> 
![alt text](screenshot.png "Screenshot")

## How to load chart data from Google Sheets rather than from a local CSV file ##

I used tabletop ([https://github.com/jsoma/tabletop](https://github.com/jsoma/tabletop "https://github.com/jsoma/tabletop")).

Tutorial: [http://blog.vida.io/2015/11/02/using-google-spreadsheet-data-in-d3-dot-js-visualizations/](http://blog.vida.io/2015/11/02/using-google-spreadsheet-data-in-d3-dot-js-visualizations/ "http://blog.vida.io/2015/11/02/using-google-spreadsheet-data-in-d3-dot-js-visualizations/")

1. Create a Google Sheet file and publish the spreadsheet to the web.
2. Copy published spreadsheet URL and paste it into the code (`var public_spreadsheet_url`).
3. Load `tabletop.js` library
4. Move d3 visualization code into a function, e.g. `draw`
5. Use tabletop to get data and render the visualization.





### How to deploy locally ###

1. To run as a local server, open a console as administrator, install [https://www.npmjs.com/package/http-server](https://www.npmjs.com/package/http-server "http-server") and run it:



    	npm install -g http-server
    	http-server &


2. Aaccess the website at [http://localhost:8080/](http://localhost:8080/ "http://localhost:8080/")
