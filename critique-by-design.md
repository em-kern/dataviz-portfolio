| [home page](https://cmustudent.github.io/tswd-portfolio-templates/) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# An Exercise in Redesign

This page shows my process of redesigning a chart: selection, critical review, sketches and feedback, and a final redesign.

## Step one: the visualization

For my redesign, I chose the visualization "The 20 Largest Solar Power Plants in the World" from the Makeover Monday site. The initial visual was really complex, but came from a pretty simple data set, so I was curious to see how I could streamline it and pull out a key message. One of my criteria for choosing a redesign was that it have an expert video, so that I could go compare my work once I was done, and learn some new tools with a data set that I was familiar with. The subject matter is also interesting to me. As the world tries to transition from fossil fuels to renewables, it's interesting to see data on which countries are leading the way, what any trends over time are, and how solar can better scale up while accounting for land sprawl. 

Original vizualization: https://solarpower.guide/solar-energy-insights/largest-solar-plants

## Step two: the critique

My first impression of the visual was that it's showing a lot of different pieces of information (timeline, power output, acreage, country), and doing it in a way that's too visually stimulating. It shows three colorful charts as part of the same visualization, and the center cylindrical 3-D bar chart (which shows the main message of the chart, the largest solar plants) is difficult to read. It ends up being a lot of eye candy and keeps the eye moving around, but is hard to pull a key message from. I did like getting a sense of which countries are leaders in solar, and that plant size is mostly increasing over time. The chart is also representing the data truthfully. 

When thinking about what I would change, I would want to add more context for the audience. What does MWp mean, and why is acreage of the plant important? I also knew that I would end up simplifying the chart into one, so that the audience could get an impression from one glance, and removing some visual frills. 

## Step three: Sketch a solution

For my initial sketches, I drew a few representing different measurements. My first was a dual axis bar chart, showing power output and land size of each plant. I also drew a simple descending bar chart of simply the most powerful plants, with small informational blurbs about what an MWp is equivalent to, and which plant was using land most efficiently. My last sketch was a scatterplot showing land efficiency of MWp/acre as a function of power output per plant.

## Step four: Test the solution

Questions I asked for feedback:

- Which sketch jumps out to you the most?
- Do you understand what each one is about?
- Is there anything that you would add that I haven't thought of?

Synthesis: 

I spoke to three class members for feedback, all master's students in public policy and management. Their consensus was that the scatterplot was the one they understood most instantaneously. They found the dual axis bar chart hard to interpret and get trends from, since the eye has to scan back and forth, and it's hard to visually get a proportion. They found the descending bar chart too simplistic in comparison to the others. 

On the scatterplot, they liked that they could instantly spot a few outliers, and could get an idea that certain plants were more or less powerful, or more or less efficient. One person said the scatterplot made them ask more meaningful questions, like why certain plants were performing better. They also noted that they wanted a more standard title, to let them know that these were the most powerful solar plants, rather than a title that had too much interpretation.

## Step five: build the solution

After gathering feedback, I watched the expert tutorial that went along with my data. The tutorial showed some charts that aligned with my sketches, and some new ones that incorporated more interactive elements in Tableau. It was fun to try out drilldowns and adding more Python rules for my data. When picking which chart I wanted to showcase here, I wanted to show the one I had designed myself and that I had gotten good feedback on, so I went off of my scatterplot.

I graphed power output by land use efficiency, as that was what most jumped out to me when working with the data. I wanted to highlight which plants were most efficient, so I added an average line to the y axis, dividing the points by more efficient and less efficient. I changed the title to be more descriptive, and added a subititle to guide the reader to think about the data the way that I was thinking about the data. I ended up adding color to each data point based on country of origin, but played around with less colorful options, like only having the points above the average efficiency line in color. That is a decision that I could go back and forth on. I do think it's a little too colorful, but I went with the option to show more information, in case the audience wanted to see country trends.

Overall, this was a fun exercise to do, and really helpful to get feedback on my work as well as learn from more expert examples. 

<div class='tableauPlaceholder' id='viz1758242024949' style='position: relative'><noscript><a href='#'><img alt='Land Usage of the World&#39;s 20 Most Powerful Solar PlantsWhat can we learn from the plants that succeed in avoiding sprawl? ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;6F&#47;6FMQ3PRGQ&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='path' value='shared&#47;6FMQ3PRGQ' /> <param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;6F&#47;6FMQ3PRGQ&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' /></object></div>                
<script type='text/javascript'>                    
  var divElement = document.getElementById('viz1758242024949');                    
  var vizElement = divElement.getElementsByTagName('object')[0];                    
  vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    
  var scriptElement = document.createElement('script');                    
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
  vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

## References

Original vizualization: https://solarpower.guide/solar-energy-insights/largest-solar-plants

Chosen from Makeover Monday: https://makeovermonday.co.uk/

Data: https://data.world/makeovermonday/2021w37/workspace/file?filename=20+Largest+Solar+Power+Plants.xlsx

Youtube tutorial: https://www.youtube.com/watch?v=BGCkC56Fysw&list=PLX-uPHRG0cLb697Ie-ZGSObRLLNhxzJGK&index=88

