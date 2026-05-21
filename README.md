# The-Red-Dragon
Can a simple time-series model beat a period-specific tracking health app? I built an ARIMA model using personal tracking data that cut prediction error down to 0.5 days—outperforming a commercial app by 60%.


<img width="1584" height="684" alt="__results___19_0" src="https://github.com/user-attachments/assets/b08dadff-b532-4c12-ace9-70330acd8bd2" /> <br>

# Goals
To test ARIMA, a period tracking app, and my own actual cycle start dates to see which of the two performed the best. 

# Finished Project
Read the entire Kaggle Notebook [here](https://www.kaggle.com/code/marissan/red-dragon?scriptVersionId=321185247)

# Programs Used
- Python
- Excel for data collection
- "My Calendar" period tracking app
- Krita for Dragon Drawing

# Analysis Questions and Findings
- Which performed better?
    - **In the smaller testing sample (4 months of 2026), we found that ARIMA exhibited the lower MAE of .25 in comparison to the app's 1.25**
- Why?
    - **The app appeared to use moving averages, relying heavily on the previous month to determine the next. When the cycle wasn't exactly 27 days (the average), the app's cycle length swung greatly in the other direction to compensate.**
 
# Data Collection
This data was collected by manually recording the app's prediction and recording my actual period start dates. The variance was calculated between the two. 

# Inspiration
The red dragon idea was inspired by this [reddit post](https://www.reddit.com/r/women/comments/1hwdoi8/comment/m60hogd/?utm_source=share&utm_medium=web3x&utm_name=web3xcss&utm_term=1&utm_content=share_button) where a woman described her husband bringing her snacks as "offerings for the red dragon". Given the immense pain my periods cause me, I 100% understand equating them to a dragon! Not to mention, it's cute and whimsical to equate the biological process to some sort of mythical beast. <br>
<br>

The project inspiration came from generally trying to see how the app functioned. Did it learn over time? Were the failures of it to learn a result of a wildly "all over the place" cycle? There are so many external factors that can impact a cycle, so I was curious on how the app accounted for that. The benefits of understanding my own cycle was also a bonus. I am definitely more in tune of what phase I'm in and how that impacts my energy levels and hormones. The idea to compare it to ARIMA came after my spree of Python work. This project was actually intended to be a gateway into reopening my dusty PowerBI toolbox, but alas, ARIMA was a much more fascinating idea. 

# Reflection
This came together quickly! I enjoyed going through the ARIMA process again and feeling more certain than the last time I had took a break and come back. I think routine practice (but not every day) has been a great way to solidfy concepts. The triple line graph was a great way to visualize the entire project as well, especially with the ARIMA backtest where you can literally "see" it learning and how those learnings helped it in the testing phase. I also enjoyed using pmdarima for automatically uncovering the best order to auto-fit our model without so many extra steps. 
