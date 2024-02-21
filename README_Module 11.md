Practical Application Assignment 11.1: What Drives the Price of a Car?

Problem Statement:
After understanding, preparing, and modeling your data, write up a basic report that details your primary findings. Your audience for this report is a group of used car dealers interested in fine-tuning their inventory.


Response:
The original dataset contained information on 3 million used cars. The provided dataset contains information on 426K cars. Given the large nature of the dataset and the restricted resources that I have on my laptop and JupyterLab, I was forced to work with a fraction of the data. In addition, after careful analysis of the data set and market research of the used car industry, and using CRISP-DM methodology, it made sense to fragment the data into more realistic/useful business case. For example, demand is very localized. Demand for cars in CA where the weather is mild and steady and higher gas prices is very different from states like CO or IA. Demand for hybrids, more gas efficient vehivles here in CA, tend to push their demand and value higher. Where as in CO due to the snow, less expensive gas, and rural nature, 4X4s, pick-up and SUV are on higher demands.  

For the afrementioned reason (mostly driven by limited computing capability), I have chosen to focus on used car prices in CA. As such, the data preprocessing steps undertaken involve filtering the data for the state of CA only, careful consideration of column removal and data cleansing to refine the dataset for analysis. Firstly, columns such as 'id' and 'VIN' are dropped due to their role as unique identifiers without substantive predictive value, while 'region' and 'state' are excluded due to their high cardinality, which could lead to a significant increase in the number of columns during encoding, thereby potentially overwhelming the model and leading to overfitting.

Furthermore, 'size' and 'cylinders' are simplified, possibly due to their limited variability or potential correlation with other features. 'Drive' is also removed as it's deemed irrelevant for the analysis based on the geographical scope of the data (focused on California). Handling missing values, especially in the 'cylinders' column, poses a challenge, with the decision to drop rows with missing values potentially leading to loss of information. However, by dropping these rows, it ensures the integrity of the remaining data and prevents biased analysis. 

Finally, filtering out vehicles priced below $400 helps focus the analysis on vehicles of potential interest while minimizing the influence of outliers. Despite these challenges, these preprocessing steps streamline the dataset, making it more manageable for subsequent analysis and modeling, and potentially improving the performance and interpretability of the resulting models.

This criterion is linked to a Learning Outcome Findings
· Clearly stated business understanding of problem
· Clean and organized notebook with data cleaning
· Correct and concise interpretation of descriptive and inferential statistics
· Clearly stated findings in their own section with actionable items highlighted in appropriate language for a non-technical audience
· Next steps and recommendations
