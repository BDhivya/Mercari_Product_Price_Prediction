<p style="font-size:30px;text-align:center"> <b>Mercari Price Suggestion Challenge</b> </p>

<h1>1. Business Problem</h1>

<h2>1.1. Description</h2>

Source: https://www.kaggle.com/c/mercari-price-suggestion-challenge
        
Data: Mercari: The Selling App, Japan.
        
Download train.tsv.7z and test.tsv.7z from Kaggle.

__Context__:

Source: https://www.kaggle.com/c/mercari-price-suggestion-challenge/discussion/50250

__Problem Statement__:

To build an algorithm that automatically suggests the right product prices given the user-inputted text descriptions of the products.


<h2>1.2. Source/Useful Links</h2>

<h2>1.3. Real-world/Business objectives and constraints.</h2>

- Low latency requirement.
- Errors can be costly.
- Interpretability is important.
- Probability of Price suggestion for a product can be useful.
- Price suggestion range can be useful.

<h1>2. Machine Learning Problem Formulation</h1>

<h2>2.1. Data</h2>


<h3>2.1.1. Data Overview</h3>

- ***train_id or test_id :***  the id of the listing or product.
- ***name :***  the title of the listing or product. 
- ***item_condition_id :***  the condition of the items provided by the seller.
- ***category_name :***  category of the listing or product.
- ***brand_name :***  brand name of the product or listing.
- ***price :***  the price that the item was sold for. This is the target variable that should be predicted. The unit is USD. This column doesn't exist in test.tsv since that is what you I have to predict.
- ***shipping :***  1 if shipping fee is paid by seller and 0 by buyer
- ***item_description :***  the full description of the item. 
     
 **Note**: The data has been cleaned to remove text that look like prices (e.g. $20) to avoid leakage. These removed prices are represented as [rm]
 

