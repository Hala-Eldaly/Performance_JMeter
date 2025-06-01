🧪 ITI JMeter Performance Testing Project
This project demonstrates core performance testing concepts using Apache JMeter, applied to both UI flows and API services, with real-world simulation and analysis.
________________________________________
🚀 Project Breakdown
1️⃣ Task One: Test Plan Scripting
A. UI Scenario — PetStore Workflow
•	Navigate to main page
•	Register new user
•	Browse product categories
•	Add product to shopping cart
•	Proceed to checkout
•	Validate that order confirmation is displayed
B. API Scenario — Restful Booker Flow
•	Perform user authentication
•	Create a new booking
•	Retrieve list of bookings
•	Modify booking with ID = 1
•	Delete booking with ID = 1
Highlights:
•	CSV parameterization via Test_Data.csv
•	Assertions applied on response contents
•	Use of defaults to make requests environment-agnostic
•	Simulated user delays using timers
•	Cookie & cache management for consistent runs
________________________________________
2️⃣ Task Two: Execution & Analysis
•	Execution setup: 2 concurrent users, 10-minute duration
•	Monitored using Aggregate Report
•	Final documented report contains:
o	Screenshot from test result
o	SLA evaluation summary:
	✅ SLA 1: Error rate ≤ 10%
	✅ SLA 2: 90% responses ≤ 3 sec
	✅ SLA 3: 99% responses ≤ 5 sec
________________________________________
3️⃣ Task Three: Load Profiling
Simulated progressive load using Stepping Thread Group plugin:
•	Ramp-up: Adds 100 users, 1 per second
•	Ramp-down: Users exit at same rate (1/sec)
________________________________________
📁 Included Files
Path	Description
jmeter/Performance_Testing_Jmeter_Project.jmx	Main JMeter test plan
jmeter/Test_Data.csv	Input data for parameterization
jmeter/Aggregate Report_HalaEldaly.docx	Test results and SLA checks
Attechments/	Screenshots and visual evidence
________________________________________
🧰 Tools & Technologies
•	Apache JMeter
•	CSV Data Config
•	HTTP Request Defaults
•	Assertions & Extractors
•	Timers, Cookie & Cache managers
•	Stepping Thread Group plugin
________________________________________
▶️ How to Execute
1.	Open the .jmx file inside JMeter.
2.	Make sure Test_Data.csv is in the same directory.
3.	Run test using configured thread group settings.
4.	Use Aggregate Report to analyze performance.
5.	For load testing, switch to the Stepping Thread Group configuration.

