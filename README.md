# Summary

This visualization shows the total distance flown by all airplanes departing from each state. We can see that the darker states are the ones that have airline hubs and that California (Los Angeles and San Francisco) and Texas (Dallas and Houston) stand out because each have two major airports.

We can also realize the growth of the total distance flown in the country, except in 2001, 2002, 2008 e 2009. Another insight is that most of the states have its peak during the year in July, August probably because of the vacation's period.

# Design

### Cleaning
I downloaded the [data](http://academictorrents.com/details/a2ccf94bbb4af222bf8e69dad60a68a29f310d9a) with over 3.5 million US domestic flight records from 1990 to 2009. Because of the size of data I had to clean it with Python before using it removing a few fields and grouping the records by year and state.

### Initial Steps

In this project I would like to visualize the US states' fligths behavior along the years. To better ilustrate the objective, a map structure was designed filling the states with a sequential single hue green coloring. The color would represent the total distance flown by all airplanes that year. 

An animation was developed going through each year and showing the differences between states and past years. After the animation some buttons were displayed for an interactive phase. Two buttons 'By years' and 'By months' would switch the visualization flights distance. The first button would make the visualization shows the total distance flown by all airplanes from that state in the selected year. The second button would make the visualization shows the total distance from that state in the selected month and year. When the 'By months' was selected a third column with buttons was displayed with the respective months of the year to be selected.

### Post-feedback

With the feedbacks I reorganize the vizualisation. I wrote some paragraphs to explain the mapping and the major insights. The 'By months' button was removed and a new bar graph was plotted to show the flights distance by month. A legend for the colors was added to explain what the values of the colors mean. The total US flights distance was included in the visualization. The last improvement was the tooltip when the mouse was over a state displaying the name and the total flights distance of that state.

# Feedbacks

The first feedback received was that the flight distance was not self explanatory and no reason were given for California and Texas standing out. The adjustment was to write a few paragraphs explaining what was the meaning of flight distance and the reason for the two states standing out. Other insights were also described in those paragraphs.    

The second feedbacker indicated that a legend of colors was going to help the visualization. He also noticed that the difference between months is barely noticeable. To resolve these issues I created a legend of colors and I removed the 'By months' button creating instead a bar graph with the total distance by each month when the mouse was over a state.

The last feedback stated that the actual value could be displayed in tooltips when the reader hovers over a state. I created a tooltip popping up under mouse cursor when the mouse was over a state. The tooltip shows the name of the state and the total flight distance in the year for that state.

# Reference

- http://bl.ocks.org/mbostock/2869946
- https://github.com/d3/d3-scale-chromatic
- http://bl.ocks.org/stephanedimanche/c687bd302bc55a0d2e40e1426349ce84
- http://bl.ocks.org/rpgove/f2abb9b4acaec88f099b
- http://bl.ocks.org/michellechandra/0b2ce4923dc9b5809922