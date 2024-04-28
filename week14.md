# Week 14 Reflection

## Source

[Visual Exploration of Big Spatio-Temporal Urban Data: A Study of New York City Taxi Trips](https://ieeexplore.ieee.org/document/6634127)

<br/>
<br/>
N. Ferreira, J. Poco, H. T. Vo, J. Freire and C. T. Silva, "Visual Exploration of Big Spatio-Temporal Urban Data: A Study of New York City Taxi Trips," in IEEE Transactions on Visualization and Computer Graphics, vol. 19, no. 12, pp. 2149-2158, Dec. 2013, doi: 10.1109/TVCG.2013.226.
keywords: {Visual analytics;Cities and towns;Data visualization;Data models;Analytical models;Time factors;Mathematical model;Visual analytics;Cities and towns;Data visualization;Data models;Analytical models;Time factors;Mathematical model;visual exploration;Spatio-temporal queries;urban data;NYC taxis},

## Reflection

This paper was about analysing taxi trips in urban locations.

The researchers believe that taxi trips can be valuable
indicators of many aspects of city life such as economic
activity or mobility patterns.

This data,however is difficult to analyze due to its complexity.

There are many variables in the data such as geographical
location and time of the trip, as well as just the sheer size of
the data that make analysis of the dataset difficult.

They propose a model to visually query taxi trips, and express
many queries based on geographical location as well as time.

They used queries following a simple template: "SELECT \* FROM
trips WHERE \<constriants\>", similar to an SQL query.

They allowed users to visually constrain the dataset in three
ways: spatially, temporally and via attributes.

This was done via UI components such as a time selection widget,
a tool bar, and multiple coordinated views to specify time and
attribute constraints with different spatial constraints.

They also create a new rendering strategy that removes clutter
from the visualization by showing it through overlay heat maps.

The researchers also performed case studies to assess their
system.

They explored taxi activities in different regions, in
transportation hubs and behavior of taxi demand over time, such
as during Hurricane Sandy and Irene.

This allowed them to assess the power of the model and system, as
well as the usability of the model and system.
