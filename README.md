# Comparable Property Finder

The Cook County Assessor’s Office (CCAO) uses LightGBM for its residential and condominium valuation models. LightGBM is a machine learning framework that works by iteratively growing many decision trees. It is especially suited to data with many categorical variables and complex interactions, such as housing data.

However, LightGBM is also complicated. Its outputs can be difficult to explain and interpret, especially as model complexity grows. Techniques such as SHAP values can help, but aren’t intuitive to the average person.

This [vignette](https://ccao-data.github.io/lightsnip/articles/finding-comps.html) written by CCAO colleague outlines how we created a novel technique to explain LightGBM outputs specifically for housing data. The technique finds comparable sales from the model training data by exploiting the tree structure of a LightGBM model. Its goal is to help diagnose model issues and answer a common question from property owners, “What comparable sales did you use to value my property?”

For more context on my specific contribution to this approach, explore [this presentation](https://github.com/claireboyd/comparable_property_finder) which outlines the design of the additional functionality of the [lightsnip package](https://ccao-data.github.io/lightsnip/index.html).
