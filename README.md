# PROJECT-4-GROUP 9 

# Contributers
- Ibsar Hashmi
- Omar Salloum
- Olufemi Olarewaju
- Saiyara Islam 

# Overview 


Model Optimization:
Cutoff based on lowest value counts:

categoryName	Value Counts
Outdoor Lighting Products	53
International Food Market	180


Water Coolers, Filters  Cartridges	526
Girls	559
Pogo Sticks  Hopping Toys	688


Handmade Toys  Games	1537
TV Accessories	1656
Scaffolding Equipment	1772
Play Sets  Playground Equipment	1925
Cigarette Lighters	2366
Automotive Care	2514
Job Site Lighting	2696
Paper  Plastic Household Supplies	2843
Breakfast Cereal	2949
Outdoor DÃ©cor	3015
Coffee, Tea  Espresso	3082
Automotive	3169
Women's Accessories	3483
Home  Kitchen	3519
Kitchen Storage  Organization	3551
Bath Products	3590
![image](https://github.com/Saiyara98/PROJECT-4-/assets/141441445/296bae43-9dd8-4044-ba3c-a2da821df260)



# Background Information 

Dataset Optimization
performed a parquet transformation on the amazon dataset. removed asin, description, product url, and image url. produced two csvs, one with boughtLastMonth column removed and the other without. cleared error rows with shifted data. total of 52582 rows cleared. datasets had rows with missing values that the model will pick up as 0s.

Discussed with the team to either use these data set or use the original and use different target and feature columns to run the neural network model as that works as well.

datasets optimized and cleaned: https://drive.google.com/drive/folders/1qSx7CM7TZl_ZcG_hKWsbitTM4n4vgMRW?usp=sharing

# Presentation 


# Links 
- https://pixelfy.me/blog/amazon-choice-vs-best-seller/#:~:text=As%20obvious%20from%20the%20name,Best%20Seller%20Rank%20(BSR)
- https://www.threecolts.com/blog-articles/amazon-best-seller-rank
- https://archive.ics.uci.edu/
- https://sell.amazon.com/blog/amazon-best-sellers-rank


- Data classification
    - Picked top 10 and bottom 10 products based on last month sold/reviews category to decide on classification targets
            (The model demonstrates meaningful predictive power at least 75% classification accuracy)
        
        - Top 10 based on reviews
            Electronics
            Bedding
            Home  Kitchen
            Televisions  Video
            Beauty
            Data Storage
            Automotive Care
            Pet Supplies
            Men's Shoes
            Printer Accessories
        
        - Bottom 10 based on reviews
            Industrial  Scientific
            Motorcycle Accessories  Parts
            Automotive Tires  Wheels
            Dishwashing Supplies
            Arts  Crafts Supplies
            Men's Shoes
            Women's Shoes
            Fresh Flowers  Indoor Plants
            Pogo Sticks  Hopping Toys
            Swimming Pool  Outdoor Water Toys


