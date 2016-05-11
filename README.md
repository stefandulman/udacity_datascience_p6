# Project 6 - complete a data visualization using d3

## Summary 

For this project I focused on a data set showing the net overseas migration pattern for Australia for a period of 11 years. The data contains information about how many people settled in or left the country and which types of visas they used. Additionally, the dataset contains information about which particular state they settled in or left.

## Design 

Initially I wanted to make a design showing the evolution of data over time. After discussing with my friends and also looking at the data patterns, it turned out that this kind of animation offered little insight for the data set. Hence, I decided to focus the animation/exploration on the types of visas instead.

Visualizing the data posed the problem of multidimensionality and also huge difference in scale for data for various states. The first step to reduce the dimensionality was to condense the many types of visas under only five categories. Secondly, I decided to show the trends of coming to/leaving Australia for various types of visa holders. For example, the story line should show that there is a general trend of immigration, using permanent and temporary visas. 

I chose to use a line chart to show the overall trend - it should convey the ideas that immigration dominates emigration. I wanted to show how this trend was computed, so I overimposed two sets of bar charts showing the arrivals and departures. Even so, there was a huge difference across regions and I chose to add a map in which to show using pie charts the immigration/emigration. The pie charts use colors for the two categories. Their surfaces reflect the size of the phenomena for each state.

A few unexpected facts were observed:
- roughly half of the temporary visa holder immigrants actually decided to leave the country
- overall, more australian citizens choose to leave the country than to move back to their home country
- although the overall trend for australian citizens is close to 0, it is the result of large numbers of incoming/outgoing persons
- there is a clear influx of New Zealand citizens and very few choose to leave
- the economical crises from 2006-2008 triggered a large amount of immigrants, as expected. A new immigration policy was adopted and the effects were quite effective, bringing the numbers down and stabilizing the influx.

The second kind of observations relates to the geography of the country. The South-East part of the continent attracts most of the immigrants, with The North-East and Western part following closely. The other regions are less favorite destinations, maybe because geographical conditions make them significantly less populated.

Back to the design choices, as can be observed from the previous versions of the index.html file, I intended to include a general graph with the overall data by default. This would have changed when the user moved the mouse over the lines in the graph or legend, then go back to the original display. The feedback was that the general overview contained basically no information, scaled the graph in an awkward manner, and it was difficult to "chase" with the mouse a line and stop on it to see the change. So, the overall view got dropped in the last version.

## Feedback 

The major points of feedback received were:
- choose an animation for the visa types instead of an animation over time
- express the huge difference between various territories using a map and an overimposed graph
- clearly show the trends in/out over time
- drop the overall view to which the graph should have returned after the mouse has moved

Minor feedback points refered to the design aspect, colors, fonts placement, the overall placement of map/graph, etc. Below is a list of changes I performed across versions, which includes also many of the minor comments:

### index.thml versions:

v1 

  - basic graph reading the data from the tsv

v2 

  - added interactivity - selected/unselected lines change shape
  - lines interact also with legend lines/text

v3

  - added bar charts

v4

  - added map and circle graphs
  - move circles to the middle of the regions

v5 

  - link bubbles to the interactive graph
  - add scaling to the circles

v6 

  - add a default value for the bubbles (the overall total)
  - add interaction to the legend line and textas well
  - add legend for the circles on the map

v7

  - beautify axes of graph
  - remove x axis; add a background set of bars with years written on top
  - remove y axis; add values on the background 
  - remove line for Canberra/ACT as the circles are too small
  - change legend text

v8

  - add a selection variable and remove the default mode in which all lines are shown
  - change color of lines
  - exchange placeholders for the figure and graph
  - make map smaller
  - add sub-title to the map
  - add title to the graph
  - added animation
  - change all text style

v9

  - properly arrange the svg and g elements inside the html doc
  - restructure code
  - fix indentation
  - arrange functions in a logical way
  - comment functions
  - move constants at the beginning
  - remove uneeded variables/functions
  - check the elements in the html and reorder them, give all of them classnames
  - move all attributes to css and use the same values for oppacity, fonts, etc.
  - use only "" instead of  ''
  - check var names
  - add constants for miny, maxy

## Resources 

I used mainly the course material and d3 documentation for this project. 

The data set was obtained from the website of Australian bureau of Statistics and is free to use:

Net oveseas migration, Arrivals and Departures, State/Territory, Major groupings and visa, Calendar years 2004 to 2013
http://stat.abs.gov.au/

The map geojson file was taken and modified from the following repository, no license offered:

https://github.com/rowanhogan/australian-states
