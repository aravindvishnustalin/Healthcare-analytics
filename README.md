**SITUATION :** GetBetterHealth.com is a startup that wants to help lower costs and increase effectiveness of the health care industry in the United States. They believe that US Medical System is inefficient. We are given a health outcome data sheet which comprises different health outcomes such as Life Expectancy and Infant mortality rate across countries. We are also given Health Care Spend data which includes GDP of various countries. GBH need to create a pitch deck that helps them secure funding.

**TASK:** Evaluate relative efficiency of US Health care system compared to other countries, given the percentage of GDP spent on health care, using suitable KPI's and visualizations. 

**ACTION:** 
1. Performed Power Query Transformations for Health Care Spend Data in Power BI to obtain the  GDP of every country averaged across the years.
   ![image](https://github.com/user-attachments/assets/ab983ccf-2bf9-401b-be95-90bff0dc88de)

2. Performed a series of Power Query transformations to Health Outcomes Data to obtain average numbers for every needed outcome & country and also merge the GDP of every country into this data.
   Then, a KPI called **Health Care Effectiveness Score** is created  to effectively evaluate a country based on both Health Outcome and GDP. This indicates if the country utilizes its GDP effectively on improving its health outcomes.
   
  **Health Care effectiveness score = Normalized Outcome Value / Normalized GDP**

  **Normalized GDP** is calculated by ratio of GDP of a country and Maximum GDP among countries. 
  **Normalized Outcome value** is calculated by ratio of Outcome value of the country and Maximum Outcome value across countries, for a specific outcome.

   For Male and Female expectancy, the score is calculated using above equation. For Infant Mortality, the inverse of the equation is needed and is automatically performed by Power BI.

   **The Health Outcomes Data**:
   ![image](https://github.com/user-attachments/assets/0e700445-4679-47d3-bb28-adea41871256)

   **The Health Care Spend Data:**
   ![image](https://github.com/user-attachments/assets/e8e1de72-fd37-4214-ac4b-36dfb3e51c05)

  3. Created **Power BI** reports to visualize the relative efficiency of US compared to other countries using **Scatter Plots** and **Health Care Effectiveness Score** tables.
  4. **JMP Pro** Statistical software is used to accurately calculate expected outcome data in US for the three outcomes based on linear fit across all countries.

**RESULT:**
1. **Female Life Expectancy at Birth Outcome:**
   
   ![image](https://github.com/user-attachments/assets/2594c8ba-0476-461a-9e28-d6038176820a)

   From the visual, we infer that Female expectancy increases with increase in GDP for most of countries except some outliers. United States is indicated by square box and is one of the outlier. This indicates that United States should have higher Female Expectancy for its GDP.

   **JMP Result:**
   
   ![image](https://github.com/user-attachments/assets/941bd41d-f52e-4926-aaf7-40e1d073a08f)
   
   This gives slope and intercept of the fit line. The expected ideal life expectancy from US can be calculated from this. The actual life expectancy for US can be obtained from the table. Both are compared. Same procedure is repeated for all outcomes.
   
   The expected Life expectancy of females at birth in the US is approximately 88.57. 
   The actual life expectancy of females at birth in US from the data, averaged over years,  is 80.91.
   The United States has approximately 9.46% lower life expectancy than expected based on its GDP.

   **Health Care Effectiveness Score Analysis:**
   
   ![image](https://github.com/user-attachments/assets/02667e14-ca75-473c-8e90-93b97bad0491)
   
   From the report, we infer that Indonesia has the highest score and US has the lowest score. On comparing the percentage higher/lower than average, Indonesia and India seem to perform fairly better than other countries. United States shows strictly lower outcomes than average, followed by Germany.

3. **Male Life Expectancy at Birth Outcome:**
   
  ![image](https://github.com/user-attachments/assets/a72a4d65-c832-4ec7-927c-30bf30570695)
  
   From the visual, we infer that Male expectancy increases with increase in GDP for most of countries except some outliers. United States is indicated by square box and is one of the outlier. This indicates that United States should have higher Male Expectancy for its GDP.

   **JMP Result:**
   
   ![image](https://github.com/user-attachments/assets/ff24cc1f-a09a-4215-8fc2-3d420ac0f28b)
   
   This gives slope and intercept of the fit line. 
   The expected life expectancy of males at birth in the United States is approximately 84.
   The actual life expectancy of males at birth in US from the data, averaged over years,  is 75.88.
   The US has approximately 10.70% lower life expectancy than expected based on its GDP.

   **Health Care Effectiveness Score Analysis:**
   
  ![image](https://github.com/user-attachments/assets/56b156f1-aeb3-4127-a4e2-46049d36c5f0)
  
   From the report, we infer that Indonesia has the highest score and US has the lowest score. On comparing the percentage higher/lower than average, Indonesia and India seem to perform fairly better than other countries. United States shows strictly lower outcomes than average, followed by Germany.

5. **Infant Mortality Rates:**
   
  ![image](https://github.com/user-attachments/assets/87e7931f-427c-4c04-a596-3725e6e9bb9b)
  
   From the visual, we infer that Infant Mortality decreases with increase in GDP for most of countries except some outliers. United States is indicated by square box and is one of the outlier. This indicates that United States should have lower Infant Mortality for its GDP.

   **JMP Result:**
   
  ![image](https://github.com/user-attachments/assets/078a57bc-5726-4427-9c23-6a72af3466fd)
  
   This gives slope and intercept of the fit line. 
   The expected infant mortality rate in the US is calculated to be approximately -4.016. This seemingly negative value suggests that ideally, the US should not just have zero but negative deaths. But however Zero infant       Mortality is expected from US for the GDP it spends.
   The actual infant mortality rate in the US from the data is 5.85 averaged over years.
   The US has 5.85% higher infant mortality than the expected number of 0.

   **Health Care Effectiveness Score Analysis:**
   
  ![image](https://github.com/user-attachments/assets/cc2615ed-c792-4fa7-993d-3a2ba8badb33)
  
   From the report, we infer that Japan has the highest score and India has the lowest score. On comparing the percentage higher/lower than average, Indonesia and India seem to perform fairly poorer than other countries. United States and Netherlands are however in the mid range when it comes to Infant Mortality Rate.

**OVERALL INFERENCE:**  The United States need to improve health care system to increase Life expectancy of both Males and Females. On the other side, India and Indonesia needs to focus on reducing Infant Mortality rate. The level of priority with which each countries must take action on each of these outcomes is illustrated by the Health Care Effectiveness Score table in the report.









