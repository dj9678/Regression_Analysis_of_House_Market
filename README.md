<h1>Regression Analysis of House Market</h1>							
<p>February 2023 - May 2023 | By Dongsuk Jeong</p>
<h2>Purpose</h2>
<p>
  - To forecast real estate prices in Atlanta, Georgia, using a multiple linear regression model<br>
  - To elucidate the factors that significantly influenced house price between pre- and post-COVID-19 by utilizing house price from 2019 and 2023 
</p>
<h2>Methodology</h2>
<span class="image main"><img src="Portfolio_Methodology1.jpg" alt="" /></span>								

<h2>Data Collection & Wrangling</h2>
<p>	
  - Collected data from Zillow<br>	
  - Removed outliers<br>
  - Redefined the quantitative variables to less catetories<br>
  - Estimated the house price of 2019<br>
</p>

<h2>Analysis</h2>
<p>
  1. Initial MLR Model<br>
    - Included all the predictors variables in the model with house price as response variable<br>
    - Low R squared value, which indicates the low model valication<br>
    - Violated the constant variance assumption<br>
</p>
<p>
  2. MLR Model with Log Transformation<br>
    - Conducted Boxcox transformation and changed both response and predictor variables to log form<br>
    - Better constant variance assumption, still low model validation<br>																
</p>
<p>
  3. MLR Model with Interaction variables<br>
    - Initially, included all the interaction variables in the model<br>
    - Better model validation, but too many predictors variables and violation of constant variance assumption<br>
    - Conducted stepwise variable selection to find out the most important variables in the model<br>
    - After variable selection, model validation got worse again<br>
    - Conducted Cook's distance to check the outlier issue in the model and removed them<br>
    - Better model validation, but the result of coefficients were against of intuition<br>		
    - Conducted the VIF test to check the multicollinearity issue in the model<br>
    - Removed the interaction variables that possibly caused the multicollinearity<br>
    - Finally, had good model validation and model assumptions
</p>
<p>
  4. Final model for 2023 & 2019<br>
    - Based on the previously founded model, construct the final model for 2019 and 2023<br>										
</p>
<span class="image main"><img src="Portfolio_Methodology1_1.jpg" /></span>
<span class="image main"><img src="Portfolio_Methodology1_2.jpg" /></span>
								
<h2>Conclusion</h2>
<p>
  - From the 2023 model, bedrooms and bathrooms have a positive effect on the house price<br>									
  - From the 2019 model, only squared feet has a positive effect on the house price, but type of home shows the negative effect on the house price  compared to single house<br>
  - From the both 2019 and 2023 model, multifamily and town home shows the more positive impact on house price compared to single house type when  considering the year of built<br>
</p>
