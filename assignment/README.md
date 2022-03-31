# Assignment 03: Sequencing a Choropleth Map Through Temporal Data

## Table of Contents

<!-- TOC -->

- [Assignment 03: Sequencing a Choropleth Map Through Temporal Data](#assignment-03-sequencing-a-choropleth-map-through-temporal-data)
    - [Table of Contents](#table-of-contents)
    - [Part I. Completing the lesson (5 pts)](#part-i-completing-the-lesson-5-pts)
    - [Part II. Building an interactive map (5 pts)](#part-ii-building-an-interactive-map-5-pts)

<!-- /TOC -->

## Part I. Completing the lesson (5 pts)

Save and commit your work to complete the Oregon Map of Unemployment Rates as outlined within [lesson 03](./README.md). Then use this as a basis for completing Part II of this assignment.

## Part II. Building an interactive map (5 pts)

Create an interactive web map of US unemployment rates by county. Use the map created within Lesson 03 as a guide.

Within the *assignment/data/* directory, examine the *us-counties.json* file. Like the GeoJSON used in the lesson, it contains no quantitative attribute data, but merely a "GEOID" attribute, which is each state and county FIPS code, concatenated together. You'll need to modify the script to bind the data to these geometries.

Also within the *assignment/data/* directory is a data file, *us-unemployment-counties.csv*.

Begin by creating a new *index.html* file within the *assignment/* directory.

Your map should fulfill the following requirements:

* Load two external files, a GeoJSON, and a CSV, at runtime.
* Process these data, binding attribute data to geometries.
* Draw a classed choropleth map of unemployment rates for US counties using an appropriate classification method, e.g., k-means or quantile, or quartile and a sequential color scheme. Consult the [Chroma.js](https://gka.github.io/chroma.js/#chroma-limits) for options.
* Draw an accompanying legend with an appropriate legend title and class break labels.
* Display the map at 100% width and height of the browser window's viewport.
* Allow the user to zoom and pan.
* Provide a meaningful title for the map, placed upon the map.

In addition to these requirements, your map should also provide the following UI enhancements for the user:

* A visual affordance when the user hovers over specific counties (e.g., making the stroke of the county yellow).
* A tooltip triggered when the user clicks on a particular county, which provides the name of the county and the specific unemployment rate for the currently displayed year.

Finally:

* Thoroughly comment your code and commit your progress with meaningful commit messages as you work.

Your final map should look and behave like this:

![Final map for assignment 03](graphics/assignment-final.gif)  
*Final map for Assignment 03.*

