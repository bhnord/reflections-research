# Week 13 Reflection

## Source

[When (ish) is My Bus?: User-centered Visualizations of Uncertainty in Everyday, Mobile Predictive Systems](https://doi.org/10.1145/2858036.2858558)
<br/>
<br/>
Matthew Kay, Tara Kola, Jessica R. Hullman, and Sean A. Munson. 2016. When (ish) is My Bus? User-centered Visualizations of Uncertainty in Everyday, Mobile Predictive Systems. In Proceedings of the 2016 CHI Conference on Human Factors in Computing Systems (CHI '16). Association for Computing Machinery, New York, NY, USA, 5092–5103. https://doi.org/10.1145/2858036.2858558

## Reflection

When (ish) is My Bus? explores a way of visualizing uncertainty predictions in a mobile interface design for transit predictions.

Displays of uncertainty can improve trust and decision making in everyday contexts, as single point estimates tend to be
interpreted as being more precise than they really are.

They found, that often times displays of uncertainty are displayed extrinsically in visualizations, which can often be
misunderstood by the viewer.

The researchers believe that uncertainty should be intrinsic to the representation, and a main focus of a visualization.

They identify design requirements specific to transit estimations through literature review, user survey of an existing application,
and iteratively through their own design process.

When creating their visualizations, they had to make them compact enough to fit on a phone, and be readable in a glance.

To this end, they include both a point estimate, as well as a probabilistic estimate of time of arrival and probabilistic estimate of
arrival status (ex: chance the bus has already arrived) for user convenience.

To show these, they explored dotplots with various numbers of dots, and stripeplots with varying amounts of stripes.

Through this, they find that discrete-outcome visualizations of uncertainty (such as dot plot and stripe plot) can improve probability
estimation in space-constrained visualizations of continuous outcomes.

They also discovered that when using too many dots or stripes, the discrete-outcome visualization performs very similarly to a density
visualization, which reflects the principle that discrete plots with too many outcomes converge to continuous encodings.

They conclude that quantile dot plots give the viewers the best estimations of probability in the context of transit prediction.
