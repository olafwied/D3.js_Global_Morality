This is a project for Udacity's Data Analyst Nanodegree. 

Summary: 
This figure shows how views on moral questions depend on where you live. The data shown here provides survey responses of different countries for the following three questions on marriage:

"Do you think ...

1) extramaritial affairs 
2) divorce 3) 
premaritial sex

... are/is morally

1) acceptable 
2) not acceptable or 
3) not a moral issue?" 


Source: http://www.pewglobal.org/2014/04/15/global-morality/ (there are a lot more questions)

Design: 

In order to demonstrate the dependence of the responses on the geographic, region the data is shown on a map. As the responses are given in percentages (limited by 100%), I used stacked bars and traffic light like colors to visualize the different proportions. "Mouseover" events and buttons ("click" events) are added to allow the viewer to explore the data interactively.

Feedback:

I posted the figure on gist (bl.ocks.org/olafwied) and shared the visualization on facebook. 

According to the feedback, it was easy to get the main message that responses depend on the geographic regions. (E.g. one person wrote: "There seems to be a solid consensus regarding affairs as bad. The other two questions appear to show a difference between western cultures (North America, Australia and Europe) vs others (China, Middle East and Africa) and the acceptance of premarital sex and divorce.
[...]
Main takeaway for me was the differences between geographic regions for the first 2 questions.")

I received further (oral and written) feedback regarding some technical issues: 

- Some countries in the middle east were difficult to differntiate -> I varied their x-position and added opacity
- The information displayed when hovering over a bar could not be seen for some eastern countries -> I added an if-statement to shift the x-position of the text position for Asian countries
- One person mentioned that it would be nice to display regions seperately to make the dependence on the geographic region more striking -> I added extra buttons and introduced a new update function



Resources: 

mercator map and interactions: 
https://www.udacity.com/course/data-visualization-and-d3js--ud507

further d3.js examples: 
https://github.com/mbostock/d3/wiki/Stack-Layout 
http://bl.ocks.org/mbostock/1134768#index.html 
http:/bl.ocks.org/yuuniverse4444/8325617