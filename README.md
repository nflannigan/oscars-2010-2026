Oscar Best Picture Nominees’ Box Office vs. Ratings from 2010-2026
================

### NOTE: The following graphs were originally designed with the Altair visualization library for Python and were intended to be interactive.

### To view the interactive versions, go to <https://nflannigan.github.io/oscars-interactive/>.

## Introduction

In 2009, the Oscars telecast was coming off a historic ratings slide.
Viewers had declined from a record high of 55 million in 1998 (the year
“Titanic” won best picture) to a low of 32 million in 2008, and some
[publicly
speculated](https://www.nytimes.com/2009/06/25/movies/25oscars.html)
that Oscar-nominated films had become too niche and inaccessible to the
general public. Hoping to capitalize on the popularity of high-grossing
movies like “The Dark Knight” and “Wall-E” (both of which were excluded
from the 2009 best picture nominations), the Academy of Motion Picture
Arts and Sciences president Sid Ganis announced that, starting in 2010,
the number of best picture nominees would be expanded from five to ten.

The question is: did the plan work? Were the nominees for best picture
more popular in the aftermath of the decision? And did Oscar telecast
ratings improve as a result of the change?

## Data

The data used in this project were aggregated from many places. The
names of best picture nominees and the years in which they were
nominated came from the Academy Awards’ [official
website](https://www.oscars.org). Figures for inflation-adjusted box
office grosses came from the film industry data website [The
Numbers](https://www.the-numbers.com).

Ratings in this report refer to Nielsen’s live-plus-same-day ratings,
which include both live viewers and viewers who watched the telecast on
a delay (prior to 3 am local time). The the company has included viewers
on streaming platforms such as YouTube TV, Sling, and Hulu in its totals
[since
2017](https://www.businessinsider.com/nielsens-tv-ratings-starts-counting-hulu-and-youtubes-new-tv-services-2017-7).
The figures themselves were gathered from contemporaneous reporting on
the Oscars by media outlets [Variety](https://variety.com) and the [LA
Times](https://www.latimes.com).

## Visualizations and Discussion

##### To view the interactive version, go to <https://nflannigan.github.io/oscars-interactive/>.

<img width="1096" height="559" alt="swarm-plot" src="https://github.com/user-attachments/assets/fb9fd48e-53b3-4df1-a26a-8afd094aee0b" />


Based on the figure above, it seems that the Academy’s decision to
expand the number of nominees for best picture initially paid off:
“Avatar,” which was then the highest grossing film of all time, was
nominated for best picture in 2010. Though “Avatar” did not go on to win
best picture, its nomination no doubt served as a signal that popular
fare could also be awards-worthy. Since 2010, however, the Academy’s
track record of nominating high-grossing movies has been more mixed. In
recent years, the Academy has nominated several popular movies like “Top
Gun: Maverick,” “Barbie,” and “Wicked.” However, only six of the last 17
years have had any best picture nominees that have grossed more than 500
million dollars, and in none of those years did the highest-grossing
movie go on to win best picture.

##### To view the interactive version, go to <https://nflannigan.github.io/oscars-interactive/>.

<img width="1083" height="537" alt="dashboard" src="https://github.com/user-attachments/assets/f7c92676-e859-41ce-b15d-1b3d1ae7244f" />


Moreover, it’s evident from the dashboard above that the relationship
between Oscar telecast ratings and the popularity of nominated films is
far from clear-cut. The scatterplot suggests a weakly positive
association between cumulative box office grosses, but there were many
periods when box office totals and ratings were far from correlated. For
example, the period from 2010 to 2014 saw consistently high ratings,
despite wildly fluctuating box office totals. Conversely, the period
from 2022-2026 saw consistently low ratings, despite the fact that
grosses during that period were highly variable: 2022 had the second
lowest box office total of the years represented and 2023 had the third
highest.

A statistical analysis of the relationship between cumulative box office
and Oscar telecast ratings bears this analysis out. For every million
dollar increase in the cumulative box office of a given year’s nominees,
Oscar viewership increases in tandem by an average of 8,657 viewers.
This relationship is significant at the alpha = 0.05 level, but it is
weak: the adjusted $R^2$ value is 0.2499.

Overall, it seems that the Academy’s decision to expand the number of
best picture nominees in 2010 has, perhaps, not had the impact they
would have ideally wanted. While recent years have seen may popular
movies nominated for Oscars like 2019’s “Black Panther” and 2023’s “Top
Gun: Maverick,” Oscar ratings began to notably decline in the years
prior to the COVID-19 pandemic and have at record lows ever since. In
this, the Oscar telecast is far from alone — television ratings, in
general, are not what they used to be. Still, if the primary goal of the
expansion was to pique popular interest and increase telecast ratings,
it’s hard to not be disappointed by the results.

## Caveats and Potential Sources of Bias

The biggest issue with the data in used here is that several films had
to be excluded on the grounds that they were distributed on streaming
platforms owned by Apple and Netflix and therefore had either negligible
or non-existent domestic box office grosses. The 14 films excluded
represented 8.97% of the total movies in the dataset. Notably, Apple’s
film “Coda” was excluded for this reason, despite winning the Oscar in
2022.

The specific films excluded were: “Frankenstein”(2026), “Train
Dreams”(2026), “Emilia Pérez”(2025), “Maestro”(2024), “All Quiet on the
Western Front”(2023), “Coda”(2022), “Don’t Look Up”(2022), “The Power of
the Dog”(2022), “Mank”(2021), “Sound of Metal”(2021), “The Trial of the
Chicago 7”(2021), “The Irishman”(2020), “Marriage Story”(2020), and
“Roma”(2019).
