# Food-recommender
This system recommends food recipes according to user input.
# AIM
<p>The main aim of the system is to recommend the best food recipes according to the user input.</p>
<p>The user will provide input such as : </p>
<ul>1. The typeof food they wish to cook</ul>
<ul>2. The range of time within which they are willing to cooking.</ul>
<ul>3. The range of calories they wish to intake</ul>
<p>According to the user input the recommendation system will suggest
few food recipes that best suits the user's demand</p>
<h1>DATA</h1>
<p>I took the dataset from kaggle,since the size of the dataset is around 290 Mb and the 
  size limit of github is only 100Mb,I couldn't upload the dataset.</p>
  <p>Hence I have mentioned the link for the dataset,you can click the link
  and then have a look as the csv file <a href="https://www.kaggle.com/shuyangli94/food-com-recipes-and-user-interactions?select=RAW_recipes.csv">link</a>
<p>The dataset consist of around 2,30,000 rows and 12 columns</p>
<h1>PRE-PROCESSING:</h1>
<p> For the system to recommend recipes according to user wish,I initially
  segregated the recipes into 5 types :
  <li>Veg dessert(without egg)</li>
   <li>Non-Veg dessert(withegg)</li>
   <li>Healthy snack(without egg)</li>
   <li>Veg</li>
   <li>Non-Veg</li>
 <p>Then i added a new column called foodtype where each dish was under either one of the types of food</p>
 <p>Then from the nutrients column I extracted the calories value and then created a new column that contains the calories values
  of that dish</p>
  <p>All these processing is done in the recipes.py file inside the pre-porcessing folder.
  Once the pre-processing is finished,I added those values into the recipe.csv file</p>
  <p>The recomm.py file contains the code where the user provides input and the recipe is recommendation.
Once the user has given their input the system will generate a dataframe containing all the dishes that satisf the user demand.
Then the model randomly selects any 3 recipes and shows those recipes to the user.
The main idea behind this was whenever the user wishes to get recipe for the same input,he/she will always find different recipes
and not the same recipes which they got previously.</p>
  <h1>LEARNING OUTCOME:</h1>
<p>My main aim was to learn how to make an end-to-end application after
  processing the data.Hence,I used flask to render my web-application.<p>
 <p>In this project, I learnt how to use flask along with html ,CSS and bootstrap and make a web-app, so that users can also use it.<p>
 
  
  
  
 
