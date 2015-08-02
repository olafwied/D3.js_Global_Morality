This is a project for Udacity's Data Analyst Nanodegree. 

Summary: 
This figure shows how views on moral questions depend on where you live. 

The data shown here provides survey responses of different countries for the following three questions on marriage:

"Do you think ...

1) extramaritial affairs 
2) divorce 
3) premaritial sex

... are/is morally

a) acceptable (green)
b) not acceptable (red) or 
c) not a moral issue (orange)?" 


Source: http://www.pewglobal.org/2014/04/15/global-morality/ (there are a lot more questions)

Design: 

In order to demonstrate the dependence of the responses on the geographic, region the data is shown on a map. As the responses are given in percentages (limited by 100%), I used stacked bars and traffic light like colors to visualize the different proportions. "Mouseover" events (for the stacked bars and the summary on the side) and buttons ("click" events) are added to allow the viewer to explore the data interactively.

Update: The different regions are highlighted using different colors. The colors were chosen in such a way that they are easy to distinguish and easy on the eyes by using different hues that fall in the medium range of intensity (generated from http://colorbrewer2.org).

Update: To make the relationship between moral views (represented by the survey responses) and geographic region more visible I added a bar chart with the average responses grouped by the greographic region. Especially for the question on premarital sex, it shows the different persepctives on moral issues across regions.



Feedback:

I posted the figure on gist (bl.ocks.org/olafwied) and shared the visualization on facebook. 

According to the feedback, it was easy to get the main message that responses depend on the geographic regions. (E.g. one person wrote: "There seems to be a solid consensus regarding affairs as bad. The other two questions appear to show a difference between western cultures (North America, Australia and Europe) vs others (China, Middle East and Africa) and the acceptance of premarital sex and divorce.
[...]
Main takeaway for me was the differences between geographic regions for the first 2 questions.")

I received further (oral and written) feedback regarding some technical issues: 

- Some countries in the middle east were difficult to differntiate -> I varied their x-position and added opacity
- The information displayed when hovering over a bar could not be seen for some eastern countries -> I added an if-statement to shift the x-position of the text position for Asian countries
- One person mentioned that it would be nice to display regions seperately to make the dependence on the geographic region more striking -> I added extra buttons and introduced a new update function

I updated several things to make the relationship between geographic regions and survey responses on moral questions more visible. See "Design".


Resources: 

mercator map and interactions: 
https://www.udacity.com/course/data-visualization-and-d3js--ud507

further d3.js examples: 
https://github.com/mbostock/d3/wiki/Stack-Layout 
http://bl.ocks.org/mbostock/1134768#index.html 
http:/bl.ocks.org/yuuniverse4444/8325617

color scheme:
http://colorbrewer2.org 
(more information here: http://www.perceptualedge.com/articles/visual_business_intelligence/rules_for_using_color.pdf)

aligning svgs:
http://stackoverflow.com/questions/20141817/how-to-align-two-svgs-side-by-side-in-d3-js