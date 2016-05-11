# Project 6 - complete a data visualization using d3

## Summary 

For this project I focused on a data set showing the net overseas migration pattern for Australia for a period of 11 years. The data contains information about how many people settled in or left the country and which types of visas they used. Additionally, the dataset contains information about which particular state they settled in or left.

## Design 

Initially I wanted to make a design showing the evolution over the time of the data. After discussing with my friends and also looking at the data patterns, it turned out that this kind of animation offers little insight in the data set. Hence, I decided to focus on the types of visas instead. 

Visualizing the data posed the problem of multidimensionality and also huge difference in scale for the data for various states. The first step to reduce the dimensionality was to condense the many types of visas under only five categories. Secondly, I decided to show the trends of coming to/leaving australia for various types of visa holders. For example, the story line should show that there is a general trend of emmigration, using permanent and temporary visas. 

I chose to use a line chart to show the overall trend - it should convey the ideas that immigration dominates emigration. I wanted to show how this trend was computed, so I overimposed two sets of bar charts showing the arrivals and departures. Even so, there was a huge difference across regions and I chose to add a map in which to show using pie charts the immigration/emmigration. The pie charts use colors for the two categories. Their surface reflects the size of the phenomena for each state.

A few unexpected facts were observed:
- roughly half of the temporary visa holders actually decided to leave the country
- more australian citizens chose to leave the country than to move their home back to it
- although the overall trend for australian citizens is close to 0, it is the result of large numbers of incoming/outgoing persons
- there is a clear influx of New Zealand citizens and very few choose to leave
- the economical crises from 2006-2008 triggered a large amount of immigrants, as expected. A new immigration policy was adopted and the effects were quite effective, bringing the numbers down and stabilizing the influx.

The second kind of observations focuses on the geography of the country. The South-East part of the continent attracts most of the immigrants, with The North-East and Western part following closely. The other regions are less favorite destinations, maybe because geographical conditions make them significantly less populated.

Back to the design choices, as can be observed from the previous versions of the index.html file, I intended to include a general graph with the overall data by default. This would have changed when the user moved the mouse over the lines in the graph or legend, then went back to the original display. The feedback was that thegeneral overview contained basically no information and it was difficult to "chase" with the mouse a line and stop on it to see the change. So, the overall view got dropped in the last version.


- explain any design choices you made including changes to the visualization after collecting feedback

## Feedback 

scale in map
drop time
trends in/out
drop overall

- include all feedback you received from others on your visualization from the first sketch to the final visualization

## Resources 

- list any sources you consulted to create your visualization
- 
