# PROJECT-4-GROUP 9 

# Contributers
- Olufemi Olarewaju
- Saiyara Islam 
- Omar Salloum
- Ibsar Hashmi


# Overview of the Analysis 

Model Optimization:
Cutoff based on 7000 counts and above per category:

total 150 category of which, top 10:,

categoryName                            Value Counts
Baby                                     24077
Luggage  Travel Gear                     22449
Handmade Home Décor                      19143
Handmade Kitchen  Dining                 19074
Handmade Jewellery                       18545
Beauty                                   18320
Men's Jewelry                            17969
Women's Watches                          17386
Boys                                     17233
Electronics                              16393

Bottom 10 categories:,

categoryName                            Value Counts
Men's Clothing                            9660
Automotive Tires  Wheels                  9482
Mailboxes  Accessories                    9329
Boating  Watersports                      9300
Women's Clothing                          9298
RV Parts  Accessories                     9259
DVD Players  Recorders                    9244
Pet Supplies                              9224
Power Transmission Products               9102
Patio, Lawn  Garden                       9037

The features of this model included:

* boughtInLastMonth
* titleLength
* categoryName
* Price
* stars
* reviews

The target of this model was isBestSeller and the purpose of the model was to determine whether, with the column features available from the dataset, would the neural network model be able to classify categories to "isBestSeller" over 75% or not.

Variables removed from the input data included the ASIN (product ID), product description (changed to product description length instead and posted as titleLength) as well as product and image URLs.

Dataset was handled in Pyspark due to 2+ million rows of information.

The neural network consisted of 3 layers, two inner layers of a single node each (tried and test with multiple nodes as well) with a single output node.
both inner layers of a node each ran with a "relu" activation while the output node ran on a "sigmoid" activation.

The runs were 100 Epochs however less than 20 Epochs would have derived the same results.

The model hit the target performance of 75% and delivered 99.99% accuracy with a validation loss of 0.018%

Steps to increase model performance (what other methods were tried)
--


# Model Training 
- Faced challenges in scaling the data with all categories in Google Colab.
- Experimented with various category limits to address the scaling issues.
- Settled on a feasible range that ultimately resulted in an impressive 99% accuracy.
- Emphasized the importance of limiting categories due to machine limitations.
- Ensured meaningful results by prioritizing categories based on counts.

# Presentation 
Link: https://docs.google.com/presentation/d/1hC79vpHBMCeMz90v7cKOk7tVNw9jDoI7L7W_FkEnd1U/edit#slide=id.g1f0e066efc7_0_194


# References 
- https://pixelfy.me/blog/amazon-choice-vs-best-seller/#:~:text=As%20obvious%20from%20the%20name,Best%20Seller%20Rank%20(BSR)
- https://www.threecolts.com/blog-articles/amazon-best-seller-rank
- https://archive.ics.uci.edu/
- https://sell.amazon.com/blog/amazon-best-sellers-rank