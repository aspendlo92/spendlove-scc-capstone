# Andy Spendlove: Swire Coca Cola Capstone Competition
This portfolio summarizes my contributions and key takeaways from the capstone project in the MSBA program at the University of Utah, where we analyzed a variety of data including customer profiles, transactions, and delivery costs, to identify trends, create predictive models, or otherwise mine actionable insights for them to improve their business.

# Table of Contents

1. [Business Problem and Objective](#business-problem-and-objective)
2. [Solution to the Business Problem](#solution-to-the-business-problem)
3. [My Contribution](#my-contribution)
4. [Business Value of the Solution](#business-value-of-the-solution)
5. [Difficulties Encountered](#difficulties-encountered)
6. [What I Learned](#what-i-learned)

## Business Problem and Objective

Swire Coca-Cola wanted to optimize how they assign customers to two delivery methods: Red Truck (premium customer service, higher cost) and White Truck (little to no direct customer engagement, lower cost). Historically, Swire used a basic threshold to determine channel assignment: whether the customer ordered 400 gallons a year annually. However, they recognized the limitations of this approach and asked our class to design a more data-driven method for determining which customers would benefit most from the premium Red Truck service.

Swire provided us with detailed customer profile and transactional data, to be able to use key business metrics in our analysis and modeling. Our objective was to develop a more nuanced strategy that could help Swire prioritize customers who would gain the most from personalized engagement through the Red Truck channel.


## Solution to the Business Problem

We explored several analytical approaches—including Random Forest, Lasso regression, and correlation analysis—to uncover drivers of customer growth. While these methods offered some insight, the most actionable results came from combining DBSCAN clustering and T-learners for causal inference.

This approach revealed that Sales Representatives were the order channel with the highest conditional average treatment effect across the customer base. If all customers not currently using Sales Reps were to switch, we estimated an average uplift of just over nine gallons per year. This led us to our final proposed solution, which was that Swire utilize heterogeneous treatment effect (HTE) modeling such as this that we had done for this Sales Rep intervention and apply our method to other variable, data sets, or even different anaytical projects within their business to determine what interventions would work best for different segments of their customer base.


## My Contribution

My main contributions to my team and our solution were:
--Serving as the project leader in the early stages of the project, gathering contact information, scheduling weekly group meetings, keeping an agenda, and keeping notes, until the project got off the ground enough where strictly coordinating these meetings was no longer necessary, as we were collaborating and chatting among ourselves more naturally.
--Writing R code to create a series of histograms and boxplots that explored the relationship between all the possible predictor variables in the data and our selected target variables
--Constructing multiple regression models, utlizing logistic, lasso, and ridge regression, to explore the possibility of creating a predictive model with suitable performance metrics to answer Swire's business problem.
--Synthesizing insights from our individual modeling projects into the finished notebooks and PowerPoint presentations that we submitted to the school and to Swire Coca Cola itself, including collaborating on the finished projects conceptually and co-authoring them.
--Conducting some final exploratory analysis into the tangible benefits of our proposed Sales Representative order channel intervention, looking at how many customers would be lost YoY if Swire stayed with their current 400-gallon threshold to establish a baseline against which to compare our method.


## Business Value of the Solution

Our solution provided actionable value in two ways: 1.) we discovered a specific intervention, switching customers' order channels to Sales Representative, and through our analysis quantified exactly what impact that would have on their business (41 customers would surpass the 400-gallon threshold with the targeted Sales Rep intervention, directly contributing to revenue growth), and 2.) this demonstration of HTE modeling was tailored and delivered to them in a way where they could take our work and apply it to other situations or data sets to discover new interventions to boost sales, keep customers off of White Truck, and retain Red Truck customers. Speaking metaphorically, we both presented them with fish and showed the an improve way of fishing.


## Difficulties Encountered

One of the biggest challenges we ran into was being overly reliant on predictive models early on. While tools like random forest and Lasso regression helped us spot patterns, they didn’t give us a clear picture of what was actually driving customer growth. We were identifying correlations, but not necessarily causes.

We also ran into limitations with the dataset—it was relatively small, especially for clustering, which made it hard to trust some of our initial insights. Eventually, we shifted our focus to more exploratory and segment-based methods, like DBSCAN clustering, which helped us better understand the types of customers who benefit from different service strategies. That pivot took some regrouping, but it ultimately led us to much stronger and more actionable takeaways.


## What I Learned

This project really underscored the importance of choosing the right analytical approach for the question you're trying to answer. By relying heavily on what we were familiar with early on or what we assumed would work best based on last semester's practice capstone, I think we ended up spinning our wheels and heading down winding roads to nowhere. It was only when we regrouped and refocused on the simple task at hand--uncovering actionable insights for SCC from their data--that we made headway and created this final product that we're ultimately very proud of.

I also gained a deeper appreciation for how exploratory techniques like clustering and causal inference can work hand-in-hand to uncover not just what is happening, but why. It was exciting to see how our final solution moved beyond just identifying good customers to actually guiding Swire toward smarter interventions.

On a more personal note, this was a great reminder of how valuable it is to have a collaborative, communicative team. We each brought different skills to the table, and being able to synthesize those perspectives into a clear, data-driven recommendation was super rewarding.
