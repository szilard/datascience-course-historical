
David Donoho's [50 Years of Data Science](https://dl.dropboxusercontent.com/u/23421017/50YearsDataScience.pdf) 
(September 2015) is a great piece. Two main points of interest to me are: 
(1) it argues that data science is the product of many *decades* and
(2) it describes an ideal data science *curriculum* 
Inspired by this, I'm releasing here a course proposal draft I wrote in 2009 for a possible
course or small set of courses of "data science". This happened before the term "data science" became commonly
used (so I used instead the term "modern statistical data analysis"). It was also before the plethora of online 
courses and books on the subject that would make this course less unique.


#### Begin verbatim from 2009

-----------------

**Course title:** Elements of modern statistical data analysis

**Course objective:** to familiarize students with some of the most fundamental methods used for analyzing complex data and for building cutting-edge statistical models

**Motivation:** With more and more data being collected in all aspects of modern life, extracting knowledge from data becomes ever more valuable in many domains, for example in science or in business. The increasing complexity of the data requires methods that go beyond the simple arithmetics of spreadsheets and necessitates more flexible approaches than simple parametric (e.g. Gaussian or linear) models. Unlike traditional confirmatory statistical modeling (e.g. hypothesis testing), exploratory data analysis advocates focusing on the data first (studying the variables, handling missing values, finding patterns, detecting outliers etc.) and only then building models. One key component of this approach is data visualization, which can be a very powerful tool in understanding various important features of the data. For the visualization to be the most effective one must follow several graph design principles that provide representations that are easy to decode for humans. Furthermore, the size and complexity of modern data requires the use of specialized software for data manipulation, computations, statistical modeling, and data visualization. In order to represent complex patterns or build predictive models, techniques developed most often at the borderline of statistics and machine learning must be used. This course will equip students with both the theory and practical knowledge necessary for starting analyzing complex data generated in modern life, for example in science or in business. Students will learn how to perform data analysis in an exploratory style, create effective graphs that help them understand the data and also communicate the extracted information to others, build sophisticated predictive models, and meanwhile they will get familiar with R, a very powerful software tool for statistical analysis (R has become the de facto standard tool for statistical analysis in academia and it is gaining more and more foot in the industry as well).

**Topics:**

**1. Software for data analysis: R**

- R as a tool for data analysis: “programming language and software environment for statistical computing and graphics” (Wikipedia), open source, free, multiple platforms (Windows, Linux, Mac), both interactive and batch use, over 2000 packages for specialized problems; comparison with Excel and other tools
- basics: data types and structures (vectors, matrices/arrays, factors, data frames), basic operations, functions, control structures (loops, conditionals), basic numeric and statistical functions (e.g. probability distributions), statistical models (linear regression, formulas, models as objects), reading data from files/databases, basic graphics, R packages
- R code will be extensively used in the lectures, assignments, and a possible term project - the lectures could be supplemented with computer practice sessions

**2. Exploratory data analysis**

- exploratory vs confirmatory, observational data vs designed experiment, “model-free” data analysis (descriptive statistics, finding regularities, detecting outliers, extensive use of visualization)
- basics of data storage and management (relational databases, SQL)

**3. Data visualization**

- the power of revealing complex patterns in data, relevance for data analysis and for information communication, graphics as data encoding, goal to be followed: to make visual decoding (conveying and understanding the information) easy
- encoding data in graphs: objects (points, lines, bars, areas etc.), visual attributes (position, color, shape, size, line style etc.)
- fundamentals of visual perception: preattentive vs attentive processing, attributes of preattentive processing, applications to visual design (maximizing “data-ink ratio”, highlighting the most important data features, de-emphasizing non-data elements etc.)
- ggplot2 package in R: the grammar of graphics, incorporating the principles of visual design, expressive and concise code due to well though default settings; ggplot2 basics: data, mappings, geoms, stats, scales (axes and legends), facets
- fundemental plot types: histograms/density, quantile plots, box plots; scatter plots, smoothing, dealing with overplotting (jittering, transparency); grouping and paneling; contour plots/bivariate density etc.

**4. Statistical learning (machine learning / data mining)**

- supervised learning / predictive modeling: regression and classification, the curse of dimensionality, the function approximation paradigm, simple local vs. global methods, the bias-variance tradeoff
- linear regression, linear regression with subset selection or coefficient shrinkage (ridge, lasso), linear discriminant analysis, logistic regression
- bivariate smoothing: splines, kernel smoothers; kernel density estimation
- nearest neighbors, decision trees, bagging, boosting, random forests, neural networks (single hidden layer feed-forward), support vector machines
- model selection and performance evaluation: model complexity and the bias-variance tradeoff, regularization, training (in-the-sample) and test (out-of-the-sample/generalization) error, cross validation and bootstrapping, Monte Carlo methods
- unsupervised learning: clustering (K-means, hierarchical)
- data mining in practice: CRISP-DM (domain understanding, data understanding/exploration, data preparation/cleaning, modeling, evaluation, deployment)

-----------------

#### End of verbatim from 2009



In 2009 the term "big data" also just started to pick up and Hadoop was still in its
infancy and being used only in select companies. 6 years later (that is now) I would put 
"databases, SQL" into a separate section and expand it with topics such as
analytical databases and "big data" systems.

All this above corresponds more or less with the curriculum David Donoho's paper advocates:

GDS1: Exploratory data analysis and data manipulation/preparation and cleaning (2. above)

GDS2: Systems/databases (2. above, but as I mentioned, it deserves a
separate section)

GDS3: Programming: R (1. above)

GDS4: Data visualization (3. above)

GDS5: Modeling (statistics/machine learning) (4. above)

**Looks like data science did not change much since 2009 afterall.**

(Donoho would also include a "meta" course  GDS6: The science of data science)

Unlike the way many of the currently available "data science programs" work, I think
the GDS courses should be taught to students who already have solid fundations
(i.e. have taken previously courses) in math (esp. probability theory,
linear algebra etc.), computer science (algorithms, data structures, hardware etc.), 
statistics, some business (e.g. project management etc.) etc.


