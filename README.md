# Lift Analysis on Car Brands  
![intro_bkgd](https://user-images.githubusercontent.com/47257479/102415236-72a95180-3fbd-11eb-90bf-102df808264a.png)  

## Quick Links  
- [Introduction](#Introduction)  
- [Section A: Lift Analysis on Car Brands](#Section-A)   
- [Section B: Car Attribute Analysis](#Section-B)   
- [Extra: Aspirational Car Brands](#Extra)   


## Introduction  
User Generated Content (UGC) is any form of content, such as images, videos, text, and audio, that has been posted by users on online platforms such as social media and wikis. Over the years, people from various industries have realized the huge potential business value of UGC when it is applied to target marketing, product management and so on. In this project, we analyzed UGC from [Edmunds](https://forums.edmunds.com/) to sketch consumers' perception of their car brands and the brand's competitors. We attempted to translate the user generated content to market structure and competitive landscape insights.  

### Packages Used  
* Pandas  
* NumPy  
* Selenium  
* NLTK  

Our code could be found [here](https://github.com/haohe1113/lift-analysis-on-car-brands/blob/main/lift_analysis_on_car_brand.ipynb)  

## Section A 
**Lift Analysis on Car Brands**    
**In this section, we will identify the top 10 mostly mentioned brands by consumers from the UGC we just scraped. Then, we will calculate lift ratios for associations between each pair of the top 10 brands and present a lift table. We *will* also visualize the lift table by a MDS map.**   

### Lift Table  
![lt1](https://user-images.githubusercontent.com/47257479/102414204-b56a2a00-3fbb-11eb-87c9-c5338c07e96b.png)  

### Visualize Lift Table by MDS Map  
![mds](https://user-images.githubusercontent.com/47257479/102414314-efd3c700-3fbb-11eb-9771-f54d713ece5f.png)  

### Insights  
Assuming that our brand manager works at Saturn, we can show that there is a high lift between Saturn and Chevrolet.  Based on the comments in the forum, they are usually being compared as similar cars.  However, in the United States, Saturn cars are generally not popular in comparison to Chevrolet cars.  Given this, the brand manager could make the brand more popular by hiring celebrities to show off their vehicles.  
If, on the other hand, our brand manager is from Chevrolet, we can show that the cars are being compared too similarly.  Given the reputation of Chevrolet, it seems as though the brand manager is doing a good job of marketing Chevrolet.  It may still be useful, however, to bring up the fact that the Saturn Aura is being compared with the Chevrolet Malibu at the same level. 

## Section B
**Car Attribute Analysis**  
**In this section, we will identify the attributes that are strongly associated with the polular brands, based on that, we will provide marketing and product-managing advice to each popular carmaker.**  

### Lift Table on Polular Car Brands vs Attributes  
![lt2](https://user-images.githubusercontent.com/47257479/102414503-46d99c00-3fbc-11eb-834c-12c30d798b3c.png)  

### Insights  
For Ford, performance and reliability have low lift values, and so a recommendation to the product manager would be to improve the driving and safety of the car.  For the advertising/marketing manager, we would recommend emphasizing these attributes in their commercial efforts.  
We found that people who talk about Mazda typically don't talk about value and reliability.  We would recommend that Mazda improve their cars by making them more affordable or more safe.  For the advertising manager, we would recommend using commercials that emphasized safety.  
Toyota cars are not really known for looking good or being strong performers.  To improve in this area, we would recommend that the product managers hire designers that can improve in these areas.  We would recommend that the marketing/advertising manager emphasize the aesthetics of these cars.  

## Extra  
**Aspirational Car Brand**   
**Which is the most aspirational brand in terms of people actually wanting to buy or own?**    
We chose common phrases that people use to express aspiration.  We went through a these posts to determine these phrases as indicators for the most aspirational brand.  We replaced these phrases with the word "aspiration" and then calculated lifts between this word and the brands, to find the most "aspirational" brand.  
### We Caught a Bot!
Based on the analysis, there is a bias in this forum towards suzuki cars.  The explanation can be found with the comments made by `iluvmysephia1`, who has inflated the forum with their love for the Suzuki brand.  In most (if not all) of their posts, they express their opinion on Suzuki as the superior brand for Mid-Sized Sedans.  As a suggestion, it may be a good idea for companies to create their own bots to counter this inflation with their own aspirational posts.  That way, consumers that visit this post won't be swayed by this individual's posts, but rather will have a range of options to consider.
