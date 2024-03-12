# Coupon-Dataset-Analysis
This repository consists of a Jupyter notebook, along with associated data and images, that analyzes some aspects of a dataset collected 
from Amazon's Mechanical Turk. The data describes whether a driver will accept a coupon to various food-and-drink establishments under 
different scenarios.

Please see the Jupyter notebook [ASubbaraman-Coupon-Analysis.ipynb](https://github.com/Vamana/Coupon-Dataset-Analysis/blob/main/ASubbaraman-Coupon-Analysis.ipynb) for details about the dataset, data transformations performed to clean up the data, and analysis code. 

### Conclusions
We focused on exloring the demographics of drivers who accepted "fine dining" coupons, and also contrasted this with those who accepted fast food coupons. <br/>
- #### <b>There is a possible age bias in the dataset.</b> <br/>
  We see from the age histogram below that <b>upwards of 70% of the recipients of all coupons were less than 40 years of age, </b> so the data possibly has an age bias built in.  Any age-related analysis will have to be viewed with caution!
  ![CouponRecipientsByAge](https://github.com/Vamana/Coupon-Dataset-Analysis/assets/7783577/bb6b7b00-f56c-41aa-80dc-89bf27aa5832)

- <b>Distribution of fine dining coupons across marital status groups and incomes are similar,</b> <br/>
The plot below shows no initial data bias.

![FineDining-all](https://github.com/Vamana/Coupon-Dataset-Analysis/assets/7783577/08b8516f-708e-4dfe-992f-12d2cfaaa2cf)

- <b>Lower-income singles and lower-income unmarried-with-partners tend to accept fine dining coupons, as do wealthier married people.</b> <br/>
We hypothesize that singles/unmarried might use the fine dining coupons for a dinner date. This could be of interest to the marketing department. Wealthier people accepting fine-dining coupons is understandable since they have more disposable income.

![FineDiningYes-marital](https://github.com/Vamana/Coupon-Dataset-Analysis/assets/7783577/227f8e9b-32aa-4e73-8d84-d1db65dc0bef)

- <b>Fast-expiring (2-hour) _fine dining_ coupons were not accepted as much as longer expiry (1 day) coupons.</b> <br/>
  Possibily, fine dining requires more planning and less spur-of-the-moment, making a fast-expiring coupon less attractive.

  ![FineDiningYes-expiry](https://github.com/Vamana/Coupon-Dataset-Analysis/assets/7783577/747a4dfd-5e6b-461a-a054-568cf0bb0c35)

- <b>By contrast, in the case of _fast food_ coupons, the difference of expiry times was not as marked as with fine dining.</b> <br/>
  
![FastFoodYes-expiry](https://github.com/Vamana/Coupon-Dataset-Analysis/assets/7783577/b5de5e65-8e85-4387-8ebf-9543a1130fde)

Since fast food is often consumed on the go and on a contingency basis, a timely coupon will still be acceptable even if it expires soon. </br>
This can be seen even more clearly in the boxplots below, where we see that for fine dining, long and quick expiry coupon acceptance are similar, but for fast food, quick expiry coupons are redeemed more.


![FineDiningYes-expiry-box](https://github.com/Vamana/Coupon-Dataset-Analysis/assets/7783577/dfd3d2b5-db0f-4019-9501-550d33bd57d9)


![FastFoodYes-expiry-box](https://github.com/Vamana/Coupon-Dataset-Analysis/assets/7783577/e0fd9e2d-8590-4d97-8421-e9b47e136444)

### Further exploration:
- It will be worth exploring if there actually is an age bias in the dataset as mentioned earlier.
- It will be very intersting to analyze how accepetance rate depends on the face value of the coupon. From a marketing point of view, is there a sweet spot where acceptance rate is high but the face value is not too high for the vendor to make a profit?
- The maximum number of coupons were given out by coffee houses. It will be interesting to do a deep dive into what drives acceptance of those coupons.

