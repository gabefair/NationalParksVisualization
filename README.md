# National Parks [#TidyTuesday](https://github.com/rfordatascience/tidytuesday) Design Contest

## Exploring our National Parks
We decided to explore the [National Parks #TidyTuesday](https://github.com/rfordatascience/tidytuesday/tree/master/data/2019/2019-09-17) R dataset for our DSBA 5122 design contest project. The dataset had been visualized before, providing us with a starting point, and lots to learn. Some visualizations we looked at were:
1. https://fivethirtyeight.com/features/the-national-parks-have-never-been-more-popular/
2. https://twitter.com/jakekaupp/status/1174139740515438593
3. https://evancanfield.netlify.com/posts/2019-09-16-national-parks-tidytuesday/tidy-tuesday-38/
4. https://github.com/gkaramanis/tidytuesday/tree/master/week-38

## Critique
#### What are good design aspects?
1. Having a graphic that is displayed in high enough quality to distinguish all parts of a line or scatterplot is sometimes an overlooked point. Data Visualizations today are included on websites and presentations that will be seen on projectors, mobile devices, and even on tablets that change the color temperature of the monitor during different times of the day and night. So it is important for data visualizations to be robust and responsive for all these devices and use cases.
2. Conscious concern for the color blind and the color disadvantaged when choosing colors for a plot. GGplot will naturally choose distinct colors while maintaining the lightness of the color pallet the same. This is sometimes not the best design considering the accessibility of the audience. The Okabe-Ito color scheme is a good example of a color pallet that is accessible (as cited in Wilke Ch. 19).
3. Minimizing activity in the visualization and focusing attention on the point while emphasizing the point to be conveyed makes for great visualizations. Some examples are labels for racing car plots, like the visualizations used in the `fivethirtyeight` article.

#### What are ways to improve this visualization?
1. Since the data is inherently geographical in nature, using a geographical map could provide better visualizations.
2. Use an effective color palette which is color disadvantage conscious.
3. Reconsider the need for axis labels, especially in a geographical plot.
4. Contemplate which legends need to be shown, especially if using both size and color to emphasize a specific feature.

#### What questions did we have with the reference code?
We noticed that some TidyTuesdays submittors used personal (e.g. [jkmisc](https://github.com/jkaupp/jkmisc)) libraries that did not work well with the version of R avaliable on the Rstudio cloud. We were able to recreate the graphic submission after using the [devtools](https://github.com/r-lib/devtools) package to install these.

## Design Scenario

#### Tasks and Data Analysis
1. Use geographical nature of data by adding geolocations using [Google's geocoding API](https://developers.google.com/maps/documentation/geocoding/start) with [R's ggmap package](https://cran.r-project.org/web/packages/ggmap/index.html).
2. Order the National parks based on Popularity
3. Characterize the distribution of visitors to the parks


#### Interactive elements
1. Use timeline data for interactive visualizations over time.

#### Dashboard for scenario
View our flex dashboard for this design contest project - 

#### Presentation for design contest
View our presentation for the design contest - http://bit.ly/designcontestdsba5122

# Acknowledgements
We would like to thank the people at [`fivethirtyeight`](https://fivethirtyeight.com/features/the-national-parks-have-never-been-more-popular/) for their visualizations which gave us a great starting point for this project. We would like to thank [Torsten Sprenger](https://github.com/spren9er) for his [visualization of the park visits](https://github.com/spren9er/tidytuesday/blob/master/tidytuesday_201938_national_park_visits.r).

We would like to thank [Ryan Wesslen](https://wesslen.github.io) and his amazingly comprehensive [DSBA 5122 course at UNCC](https://dsba5122.com) for all the concepts and ideologies we have learnt and imbued into this project.

We would like to thank the [#TidyTuesday](https://github.com/rfordatascience/tidytuesday) and [R4DS](https://r4ds.had.co.nz) community for making varied and interesting datasets available for researchers to practice and work on, and grow together as a community.
