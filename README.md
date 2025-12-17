# Amazon-Search-Engine-NLP

The objective of this project was to create a review-based search engine for opinions
expressed on Amazon using an opinion-based approach.
The minimum requirements of the project is the baselineBoolean search which finds
matches to all keywords. However, boolean search does not understand "sentiment" nor
"context". As such, I created a number of additional NLP-based methods to better attempt to
recognize sentiment, aspect-opinion relationships, and context of a review.
The original dataset included over 210,000 reviews, but I limited myself to a smaller
dataset of 10,000 reviews to help with processing time within Google Colab. I uploaded a csv
file, switching it from the excel file that was provided so that the data can be read better on colab
and then I switched my runtime type to run on A100 GPU for faster results. This project is done
using jupyter notebook on colab, completely in python. I’m also importing all libraries or
dependencies that were necessary to the project. After that, I begin preprocessing and follow up
with each method which will be run through the five user-defined searches, and the results from
each method will be compared based upon the number of reviews returned, and their relevance.
Ultimately, the final objective of the project was not only to develop several different
retrieval methods; but to demonstrate the differences in behavior between each method as they
attempted to retrieve both the "aspect" and "opinion" from the reviews.
