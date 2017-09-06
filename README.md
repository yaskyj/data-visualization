# Data Visualization with D3
## Table of Contents
1. [Project Files](#section1)
2. [Summary](#section2)
3. [Design](#section3)
4. [Feedback](#section4)
5. [Resources](#section5)  
[Data Document Links](#section5_1)


## <a id='section1'>Project Files</a>
Files contained in repository:
* [docs/index.html](https://github.com/yaskyj/data-visualization/blob/master/docs/index.html) - code for data visualization. Live site is located [here](https://yaskyj.github.io/data-visualization/).
* [data/CleanData.Rmd](https://github.com/yaskyj/data-visualization/blob/master/data/CleanData.Rmd) - R file to import, clean, merge, and export data into one file
* [data/data.csv](https://github.com/yaskyj/data-visualization/blob/master/data/data.csv) - cleaned and merged data file for import into visualization
* [data/gdp.xlsx](https://github.com/yaskyj/data-visualization/blob/master/data/gdp.xlsx) - original GDP file from Gapminder.org
* [data/population.xlsx](https://github.com/yaskyj/data-visualization/blob/master/data/population.xlsx) - original population file from Gapminder.org
* [data/regions.xlsx](https://github.com/yaskyj/data-visualization/blob/master/data/regions.xlsx) - original region mapping from gsociology.icaap.org.
* [data/school.xlsx](https://github.com/yaskyj/data-visualization/blob/master/data/school.xlsx) - original average years in school for men 25 to 34 years old from Gapminder.org

## <a id='section2'>Summary</a>
This visualization shows the average years in school by country against the national GDP per person in USD adjusted for inflation. These features are shown by year and the bubble points on the chart are sized by the population. The chart shows that GDP in positively correlated with the level of education of the country and that both of these measures generally increase from year to year. It also shows that there is not a strong correlation in all cases, such as with Eastern Europe and Russia (i.e. former Soviet bloc countries).

## <a id='section3'>Design</a>
One of my favorite visualizations is [Hans Rosling's 200 Countries, 200 Years, 4 Minutes](https://www.youtube.com/watch?v=jbkSRLYSojo). I really wanted to recreate that type of visualization showing the correlation between wealth and education showing changes through the years. I found the datasets needed on the [Gapminder.org website](https://www.gapminder.org/data/). I initially wanted to use literacy rates as the measure of education, but there wasn't enough data across all years so I decided on average years in school for males 25-34 (as they didn't have the measure for both male and female).

I've used DimpleJS in previous work projects, so I googled for examples of animations. I found pretty much exactly what I was trying to do on the [DimpleJS.org site](http://dimplejs.org/advanced_examples_viewer.html?id=advanced_storyboard_control) as an example.

After cleaning/merging the data and getting the basic animations working with the code example I found, I showed the visualization to four coworkers, received verbal feedback (some of it conflicting), and then incorporated the feedback into the final visualization. Detailed feedback and how it was incorporated can be found in the [feedback section](#section4) below.

## <a id='section4'>Feedback</a>
### List of feedback with resolutions:
* Too many years cluttering the side - I removed years 1970 through 1989.
* Title too small and not enough information about the graph - I changed the title and it's position. In addition, I added more text at the top to put the graph in context.
* No explanation of the bubble size - added text at the top of the graph to explain the size of the bubbles.
* Axis labels too small
* No explanation of the axis
* legend spaced weirdly
* Bottom of the chart is cluttered looking with so many bubbles
* GDP not explained as USD and adjusted for inflation
* One persion said that the animation was going to quick to view individual bubbles while another person said that the animation wasn't fast enough to notice the changes between years - I added an interactive input for time

## <a id='section5'>Resources</a>
[Animating and storyboard example on dimplejs.org](http://dimplejs.org/advanced_examples_viewer.html?id=advanced_storyboard_control)  
[Interactive legend example on dimplejs.org](http://dimplejs.org/advanced_examples_viewer.html?id=advanced_interactive_legends)
[Wrapping Text example](https://bl.ocks.org/mbostock/7555321)

### <a id='section5_1'>Data Document Links</a>
[Region Mapping](http://gsociology.icaap.org/data/WorldPopulation.xlsx)  
[Gapminder Website](https://www.gapminder.org/data/)  
[GDP](https://docs.google.com/spreadsheet/pub?key=0AkBd6lyS3EmpdHo5S0J6ekhVOF9QaVhod05QSGV4T3c&output=xlsx)  
[Average Years in School - Males 25 to 34 years old](https://docs.google.com/spreadsheet/pub?key=0ArfEDsV3bBwCdHlYZHNWN1YtWVNudU9UbWJOd19nUVE&output=xlsx)  
[Population](https://docs.google.com/spreadsheet/pub?key=phAwcNAVuyj0XOoBL_n5tAQ&output=xlsx)