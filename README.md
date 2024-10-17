# Project Background
VelocityX is focused on creating an immersive spectator experience that monetizes and promotes autonomous racing worldwide. Here are some features of the app:
- Immersive Fan Experience: During major racing events, VeloCityX offers “Live 360” coverage. Using mobile devices, fans can experience races from multiple angles, including cockpit views, aerial drones. Live chats and forums allow fans to discuss races in real-time.
- Interactive Fan Engagement: For interactive fan engagement, VelocityX introduces “Fan challenges” users can predict race outcomes, such as which vehicle will complete the most laps without recharge or which team will achieve the fastest pit stop. These challenges are gamified and allow fans to earn points and rewards for accurate predictions.
- Monetization Strategies: VeloCityX includes “Virtual Merchandise and Sponsorship Integration” Fans can purchase virtual merchandise such as team jerseys, vehicle skins, and exclusive digital collectibles. The app offers sponsorship opportunities where brands can sponsor race events or place ads to reach target audiences.
# Clustering - **K Means**
## Find the best k
- Silhouette scores and elbow curve
- Feature Engineering
- Davies-Bouldin Scores
- Calinski-Harabasz Scores
- Visualize using PCA
# Insights on customer behaviors and recommendations
## Cluster 0: rational users
### Predictive Accuracy and Virtual Merchandise Purchase (0.33):
- Since Purchase Tendency is partially based on Sponsorship Interactions, the strong positive correlation is expected. But this cluster has already been the one with the closest number of correlation between 0.62 (virtual merchanise purchases and purchase tendency) and 0.79 (ads clicks and purchase tendency). It indicates that compared to the other two clusters, in cluster 0, users who interact more with ads are also likely to purchase merchandise, confirming that these two behaviors are strongly connected. From this insight: we could provide these users some tutorials or analysis from experts to help with their prediction process, so as to increase predictive accuracy. Besides, we can consider charging on these articles or helper methods.
### Sponsorship Interactions and Purchase Tendency (0.79):
- Since Purchase Tendency is partially based on Sponsorship Interactions, the strong positive correlation is expected. But this cluster has already been the one with the closest number of correlation between 0.62 (virtual merchanise purchases and purchase tendency) and 0.79 (ads clicks and purchase tendency). Also, from the bar chart above the heatmap, cluster 0 has the highest average number of ads interaction. It indicates that compared to the other two clusters, in cluster 0, users who interact more with ads are also likely to purchase merchandise.
## Cluster 1: live watchers
### Time on Live 360 and Virtual Merchandise Purchase (0.21):
- A direct, positive correlation between Time on Live 360 and Virtual Merchandise Purchase suggests that time spent engaging with live events has a direct impact on a user's willingness to interact with ads or make purchases. To capitalize on this, we could promote merchandise and sponsorship ads during live events, as those already spending significant time on live coverage are more likely to respond positively to such promotions.
### Sponsorship Interactions and Virtual Merchandise Purchase (-0.21):
- The negative correlation suggests that users who interact more with sponsorship ads are less likely to purchase virtual merchandise. Users who are interacting frequently with ads may need additional motivation to purchase virtual merchandise. Possible approaches include:
- Ad-Incentivized Merchandise Promotions: Link ad interactions with merchandise discounts or exclusive items. For example, users could unlock an exclusive virtual item or receive a discount code after interacting with a certain number of ads.
- Segment-Specific Campaigns: Since sponsorship interactions and merchandise purchases are negatively correlated, we may need to create distinct marketing strategies:
  - For users who focus more on sponsorship interactions, provide incentives to engage with merchandise (e.g., by offering merchandise tied directly to ads or promotions).
  - For users who are more focused on purchasing merchandise, emphasize exclusive offers not tied to sponsorship interactions, allowing them to purchase without needing to engage in ads.
### Engagement Index and Virtual Merchandise Purchase (0.28):
- Users who engage in either chat activities, lives (especially on lives because of the 0.73 correlation rate), or fan challenges are more likely to purchase virtual merchandise. Recommendation: Personalized Merchandise Offers: Consider targeting highly engaged users (those with a higher Engagement Index) with special offers or exclusive virtual items to capitalize on their broader activity.
## Cluster 2: introverted users
### Fan Challenges Completed and Virtual Merchandise Purchase (0.39):
### Recommendations: Challenge-Based Rewards:
- Offer merchandise-related rewards for users who complete or perform well in fan challenges. For example:
- Discount codes or exclusive virtual items could be given as rewards for accurately predicting race outcomes or for completing a certain number of challenges. This will create an additional incentive to participate in challenges and increase the likelihood of users purchasing virtual items.
- Leverage the Competitive Spirit:
- i.e. adding leaderboards or progress tracking where users who complete challenges could unlock unique virtual merchandise. This could enhance the competitive spirit and drive further purchases.
# Predictive Model
# Proposed Fan Challenge - Ad Boosted Prediction Challenge
# Bootstrapping - simulation
# Random Forest - predicted outcomes
## Improvement Rate: Approximately 40% (38.00%-41.00%) of users moved to 'Medium to High Purchases'
- The proposed intervention strategies have demonstrated significant positive impacts across different user clusters, leading to improved engagement and monetization outcomes.
## Key observations from the transition matrices are as follows:
- Cluster 0 (Rational Users): A notable shift was observed, with 7 users moving from 'Medium Purchases' to 'High Purchases'. This suggests that the expert insights and ad interactions have effectively driven increased purchase behavior in this group. Monetization is positively impacted, with more users being motivated to make higher-value purchases.
- Cluster 1 (Live Watchers): Users in this cluster also showed improvements, with 6 users moving from 'Medium Purchases' to 'High Purchases'. The emphasis on live event promotions and ad-incentivized merchandise appears to have increased both engagement and the likelihood of making purchases. Engagement during live events has translated into higher purchase rates.
- Cluster 2 (Introverted Users): There was a significant movement, with 15 users moving to 'High Purchases' and 11 users moving from 'Medium Purchases' to 'High Purchases'. The gamification of fan challenges and rewards for completing challenges have successfully encouraged higher engagement and monetization for introverted users.
- Overall, the comparison of purchase categories before and after intervention shows a clear improvement, with almost one half of users moving to 'Medium to High Purchases'. This indicates that the tailored strategies for each cluster were effective in enhancing both user engagement and the overall revenue potential through increased merchandise purchases.
