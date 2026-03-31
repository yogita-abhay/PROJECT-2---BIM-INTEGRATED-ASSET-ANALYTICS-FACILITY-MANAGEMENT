<img width="2149" height="860" alt="image" src="https://github.com/user-attachments/assets/9d4ca2da-19d5-4871-a4ba-d976273763ea" /># PROJECT-2--BIM-INTEGRATED-ASSET-ANALYTICS-FACILITY-MANAGEMENT

## Project Overview
This project focuses on the Asset Analytics & Facility Management (FM) lifecycle by integrating Building Information Modeling (BIM) with Artificial Intelligence (AI) to optimize civil infrastructure performance. By analyzing the "Data-to-Decision Gap," the study utilizes structural health monitoring (vibration, crack width), real-time IoT environmental metrics, and drone-based visual intelligence. The analysis provides predictive insights for four key infrastructure categories (Bridges, Roads, Buildings, and Pipelines) to transition from reactive repairs to a Proactive Digital Twin model. By correlating historical cost deviations with real-time risk factors, the project supports strategic decision-making in capital expenditure (CAPEX) planning, safety risk mitigation, and structural longevity.

### **Objectives**

1. Analyze Risk-Failure Correlation: Evaluate the relationship between structural health indicators (vibration, load-bearing capacity) and project risk levels to identify early warning signs of asset failure.

2. Identify Asset Performance Gaps: Detect discrepancies between "Planned vs. Actual" durations and costs across different project types to pinpoint systemic inefficiencies in the infrastructure lifecycle.

3. Engineered Predictive Maintenance Metrics: Develop data-driven thresholds for environmental factors (Temperature, Air Quality) and structural wear to automate maintenance triggers within the BIM environment.

4. Optimize Resource & Budget Allocation: Utilize predictive modeling to prioritize high-risk assets for funding, ensuring that limited maintenance budgets are directed toward the most critical infrastructure needs.

5. Isolate Structural & Safety Bottlenecks: Use drone-based monitoring scores and anomaly detection to isolate specific geographical or structural points of failure that require immediate intervention.

### **About the Dataset**

This file (https://www.kaggle.com/datasets/ziya07/bim-ai-integrated-dataset) contains structured data for whole life cycle management of civil engineering projects using BIM and AI integration. It includes key attributes related to cost, schedule, structural health, environmental conditions, and risk assessment, enabling predictive analytics for optimized project execution. Each row represents a construction project or a specific project phase, with multiple variables capturing real-time IoT sensor data, drone-based monitoring, and historical construction records. 

The Intent: You are performing "Post-AI Analysis." You are taking the outputs of AI sensors and using Business Intelligence to make sense of them for the project manager.

### **Dataset Overview**

Project_ID: A unique alphanumeric identifier assigned to each specific construction or infrastructure project.

Project_Type: Categorizes the asset class (e.g., Bridge, Road, Building) to allow for comparative analysis across sectors.

Location: The location (Los Angeles 21%, Seattle 21%, New York, Other 58%), where the physical asset is situated. 

Start_Date: Marks the official commencement of the project or the data collection phase from 2020-01-01 to 2022-09-26.

End_Date: Represents the scheduled or actual completion date for the project lifecycle.

Planned_Cost (USD): The initial estimated budget allocated for the project during the design phase.

Actual_Cost (USD):The total financial expenditure recorded at the time of the latest data entry.

Cost_Overrun (USD):The calculated financial difference between the actual expenditure and the planned budget.

Planned_Duration (days): The projected timeline for project completion as defined in the original schedule.

Actual_Duration (days):  The real-world time elapsed from project start to current status or completion.

Schedule_Deviation (days): Measures the variance (delay or acceleration) between the planned and actual timelines.

Vibration_Level (mm/s): IoT sensor data measuring mechanical oscillations to monitor the structural integrity of the asset.

Crack_Width (mm): A critical structural health metric used to track physical degradation or surface fatigue in materials.

Load_Bearing_Capacity: Defines the maximum weight or stress the structure is currently engineered to safely support.

Temperature (C): Environmental data used to analyze how thermal expansion and weather conditions impact material durability.

Humidity (%): Records the percentage of moisture in the air, which can affect material curing and long-term structural corrosion.

Weather_Condition: Categorizes the external environment (e.g., Cloudy, Sunny, Rainy, Stormy, Snowy) to assess its impact on project timelines and site safety.

Air_Quality_Index: Monitors environmental health parameters at the project site to ensure compliance with worker safety regulations. AQI ranges between 0 to 500.

Energy_Consumption (kWh): Tracks the total power usage of the facility or site, a key metric for calculating operational costs and sustainability.

Material_Usage (m3): Quantifies the volume of resources (like concrete or steel) consumed to monitor supply chain efficiency and waste. m³ (Cubic Meters)Given the values (100–1000), this likely represents the volume of primary material like concrete or steel used in that project phase.

Labor_Hours (hrs): Total cumulative time spent by the workforce on project tasks, used to measure productivity and payroll.

Equipment_Utilization (%): Calculates the percentage of time machinery (like cranes or excavators) is actively working versus sitting idle (%).

Accident_Count: A critical safety metric recording the number of recorded incidents or injuries on-site during a specific phase.

Safety_Risk_Score (0-10): A calculated numerical value representing the likelihood of future hazards based on historical site data. 

Image_Analysis_Score (0-100): A score generated by AI (often from drone footage) to evaluate the quality or progress of construction visually. 

Anomaly_Detected: A binary or categorical indicator showing if the AI has flagged any unusual patterns in structural or operational data.

Completion_Percentage (%): Tracks the current progress of the project phase relative to the total scope of work.

Risk_Level: The final target variable classifying the project’s overall status (e.g., Low, Medium, High) based on all other data points.


### **The Project Workflow**

1.BIM: Provides the 3D data and planned costs.

2.AI Sensors: Provide real-time health data and anomaly flags.

3.Diagnostic Analysis: Connects the two to find the Root Cause of failures.

### **Key Features**
1. Project Metadata: ID, type (bridge, road, building, etc.), location, and timeline.

2. Financial Data: Planned vs. actual cost, cost overruns.

3. Scheduling Data: Planned vs. actual duration, schedule deviation.

4. Structural Health Monitoring: Vibration levels, crack width, load-bearing capacity.

5. Environmental Factors: Temperature, humidity, air quality, weather conditions.

6. Resource & Safety Management: Material usage, labor hours, equipment utilization, accident records.

7. Drone-Based Monitoring: Image analysis scores, anomaly detection, completion percentage.

8. Target Variable: Risk Level (Low, Medium, High) based on cost, schedule, safety, and structural health. 

### **Data Modelling**

<img width="1412" height="859" alt="image" src="https://github.com/user-attachments/assets/981855ac-79b9-43b4-add0-d1a0a5637947" />


### **SCHEMA OF THE MODEL**

1.Fact Table: BIM-AI DATASET

2. Dim Tables: 
a) DIM-PRJ 
b) DIM-DATES 
c) Anamoly Table

3. Logic Table: DIM-AI-INTELLIGENCE

### **EXCEL DASHBOARD**

<img width="1953" height="1000" alt="image" src="https://github.com/user-attachments/assets/d997112d-8afc-4799-ae5f-2236dc54a3cc" />

### **POWER BI DASHBOARD**

<img width="1415" height="789" alt="image" src="https://github.com/user-attachments/assets/b9cf45b1-29a5-4f6a-9428-1b01a0177932" />

<img width="1428" height="799" alt="image" src="https://github.com/user-attachments/assets/bae91784-7de8-441a-90d6-35b43216a6aa" />

### **FINAL KPI METRICS**

1) BIM (Building Information Modeling): A digital representation of a facility's physical and functional characteristics, serving as a shared knowledge resource for decisions during its life cycle.

2) Structural Health Monitoring (SHM): The process of implementing a damage detection and characterization strategy for engineering structures using embedded sensor data.

3) AI Anomaly Detection Frequency: An AI-driven process that identifies data points, events, or observations that deviate significantly from a dataset's normal behavior.

4) Equipment Utilization: A measure of operational efficiency that tracks the active usage time of heavy machinery against its total availability to optimize fleet deployment.

5) Load Bearing efficiency: The ratio of actual structural loading to designed capacity, used to identify underutilized assets or those operating dangerously close to failure thresholds.

6) Project Type Counts: A categorical breakdown of the portfolio that identifies the distribution of different asset classes, such as Bridges, Tunnels, and Buildings, for targeted risk management.

7) Resource Utilization: Average Equipment Utilization and Labor Hours per project type.

8) Cost Overrun Intensity: Total Cost Overrun as a percentage of Planned Cost. (current average is $5.1M).

9) Critical Anamolies: The total volume of structural irregularities identified by the AI sensors across all project sites.

10) Average Completion %: The current aggregate progress of the project portfolio against defined construction milestones.

11) Load Safety Efficiency: A critical safety ratio comparing actual structural loading to design capacity to ensure assets are operating within their engineered stress limits.

12) Environmental profile: Frequency of weather events

13) Structural stress Profile: average load vs Vibration by Asset Category

14) Average Schedule Deviation: The variance between the planned timeline and actual progress, measured in days of delay or acceleration.

15) Total Cost overrun: The total financial leakage representing the difference between the planned budget and actual expenditure across all projects.

16) Average safety risk: An aggregate probability score used to quantify the overall danger level across sites and prioritize high-risk assets for urgent safety interventions

17) Planned vs. Actual: A comparison between the theoretical project goals (budget/time) and the real-world execution data.

18) Image Analysis Score: A quantitative value assigned by a computer vision model reflecting the severity of structural defects identified from site photographs.

### **KEY TAKE-AWAYS**

1. High-Risk Asset Identification
Takeaway: Tunnels and Bridges represent the highest concentration of AI-detected anomalies, accounting for nearly 20% of total alerts, requiring a shift toward prioritized sensor-based inspections for these categories.
Action: Direct maintenance resources to these two asset classes first to mitigate catastrophic risk.

2. Significant Structural Safety Breaches
Takeaway: The Crack Expansion Index (5.0) and Risk Intensity (~3.7) indicate that multiple structures are operating significantly outside of their safe design baselines.
Action: Immediate structural audits are required for projects where the actual crack width exceeds the 'Normal' baseline by more than 2x.

3. Financial & Schedule Correlation
Takeaway: A critical correlation exists between structural health and project delivery, with the portfolio experiencing an average 106-day schedule delay and a total $5.1B cost overrun.
Action: Implementing BIM-AI monitoring earlier in the project lifecycle can prevent these 'hidden' structural costs from ballooning during the late construction phases.

4. Environmental Sensitivity
Takeaway: Structural anomalies show a positive correlation with extreme weather conditions (High Temp/Humidity), suggesting that environmental stressors are the primary catalysts for material fatigue in the current portfolio.
Action: Enhance climate-resilient design standards for future projects in high-temperature or high-humidity locations.

5. Load Capacity Efficiency
Takeaway: The Load Safety Efficiency analysis reveals that while most structures are within capacity, specific outliers are operating near peak stress limits, reducing the safety buffer for unexpected seismic or environmental events.
Action: Install real-time load-limiting sensors on assets identified as 'High Stress' to prevent structural collapse.

### **STRATEGIC RECOMMENDATIONS**

1. Risk-Based Maintenance (RBM) Strategy
Recommendation: Implement an "Automated Alert Hierarchy" that prioritizes Tunnels and Bridges.
The Action: Configure the AI to trigger an immediate onsite inspection request whenever the Crack Severity Index for these specific asset classes exceeds a threshold of 1.5. This moves the team from reactive repairs to predictive maintenance.

2. Structural Reinforcement & Retrofitting
Recommendation: Conduct a targeted audit of projects with a Risk Intensity > 3.0.
The Action: For older structures or high-stress Tunnels identified in the dashboard, initiate a retrofitting program (e.g., adding carbon fiber wraps or steel bracing) to return the Load Safety Margin to a healthy buffer.

3. Environmental Resilience Standards
Recommendation: Update the Material Specification Standards based on location-specific sensor data.
The Action: Since the data shows high anomaly correlation with temperature and humidity, use higher-grade, climate-resilient concrete mixes and corrosion-resistant coatings in projects located in humid or high-heat coastal regions.

4. Cost & Schedule Recovery Plan
Recommendation: Integrate BIM-AI monitoring into the Pre-Construction phase.
The Action: To stop the $5.1B cost leakage, use AI sensor data from similar existing projects during the design phase. This allows engineers to predict structural challenges before they become 106-day delays during the build.

5. Digital Twin Synchronization
Recommendation: Fully synchronize the Live Sensor Dashboard with the BIM Digital Twin.
The Action: Ensure that every "Anomaly" detected in Power BI is visually mapped onto the 3D BIM model. This allows maintenance crews to see exactly where a crack is located inside a tunnel wall before they even arrive at the site.


