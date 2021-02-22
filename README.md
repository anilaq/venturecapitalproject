# venturecapitalproject


# Executive Summary 



I conducted analysis on a crunchbase dataset that shows information on startups that have gone through different funding rounds. The aim here is to predict whether or not a company will reach series A. This should be done within 2 hours. 

You can also link to

Email Me <anila.m.qureshi@gmail.com> 
My LinkedIn <https://www.linkedin.com/in/anila-qureshi-262aa670/> 
Medium Blog <https://medium.com/me/stories/public> 

# Background Information

With the task at hand it is important to understand the industry for the analysis that is being conducted. Venture Capital is a powerful industry that is mostly seen as a U.S dominated force. The United States is fostered on the idea of imagination, innovation and the success on startups. Venture Capital plays a huge role in the success of U.S based businesses. Although venture capital is very saturated within the United States it is not limited to that area of scope. 

In fact, In Reach Ventures is trying to break down the barriers to entry for startups that exist within the EU and UK. This is important because innovation and company creation is largely focused around political climates. From a quick search on whether a company will succeed in raising series-a or not largely has to do with the amount of funding the startup would like to raise. 

According to a TechCrunch(<https://techcrunch.com/2017/08/23/does-it-really-matter-how-much-your-startup-raises/>) article, a company that is most likely to reach serie-a has raised around $2million in pre-series-a funding. 

Aside from domain knowledge on the amount of money that should be raised I took it upon myself to break this down into simple data analysis and problem solving. My goal was to do a basic regression model on the data at hand. In order to do so, I would have to process and clean the data accordingly. 

My large assumption/hypothesis is to test the more money raised pre-series-a, the bigger likelihood a company raises and reaches series-A. 

Steps: 

1. I first went in to the dataset and removed all columns that were not in USD. 
2. I then wanted to take a look at unique object_id. This would tell me whether companies did multiple rounds and if so, how many. I ended up finding that some companies did multiple angel rounds, multiple seeds and so on. 
3. I then created queries based on object_id and companies that have done angel, seed, and convertibles (pre-series-a rounds). 
4. Create a regression model to predict which features are most important for predicting series A

# Findings

Given the time constraint, my original choice of using a random forest model or KNN-Means given that there is a mix numerical and categorical variables makes things a bit more difficult. 

Within this time frame I have found that there are a lot of N values. This means that companies have chosen not to disclose whether they raised, what their pre_money_valuation is, or what their post_money_valuation is. This depletes my data picture down and makes a regression model using categorical variables very difficult. I have conducted a very basic ordinary least squares and then done a linear regression. But just as I predicted it did not give much value. 

However, just by creating the columns in steps 2 & 3. One is able to do a general assumption of whether a company will make it to series A. 
