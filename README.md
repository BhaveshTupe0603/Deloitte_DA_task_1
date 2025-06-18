# 📊 Deloitte Virtual Job Simulation – Telemetry Data Analysis with Tableau

This repository contains my solution for the **Telemetry Data Analysis** task from the **Deloitte Data Analyst Virtual Experience Program** hosted on Forage.
![Screenshot 2025-06-03 212852](https://github.com/user-attachments/assets/68f3631e-2181-473d-9de8-bff282eba389)

---

## 🎯 Task Objective

The goal of this task is to analyze telemetry data collected by **Daikibo** and visualize potential machine downtime using **Tableau**. This simulation helps demonstrate data wrangling, dashboard creation, and interactive filtering skills.

---

## ✅ Steps Followed

1. **Installed Tableau**  
   - Used the [Tableau Free Trial](https://www.tableau.com/products/trial) and registered with my email.

2. **Loaded Data**  
   - Downloaded and unzipped `daikibo-telemetry-data.json.zip`.
   - Imported the JSON data into Tableau.

3. **Created Calculated Field**  
   - Created a new calculated measure:
     ```
     IF [Status] = "Unhealthy" THEN 10 ELSE 0 END
     ```
   - Renamed this measure as **`Unhealthy`**, representing **10 minutes of potential downtime** for each "Unhealthy" status.

4. **Visualizations**
   - **Sheet 1**: Bar chart showing **Down Time per Factory** using SUM(Unhealthy).
   - **Sheet 2**: Bar chart showing **Down Time per Device Type**, also using SUM(Unhealthy).

5. **Interactive Dashboard**
   - Combined both sheets into a **Dashboard**.
   - Configured the **Factory chart** as a **filter**, so selecting a factory updates the device-type chart accordingly.

6. **Result**
   - Identified the factory with the **highest downtime**.
   - Took a screenshot of the dashboard showing filtered data and uploaded it as my final submission.

---

## 📁 Files Included

- 📷 Screenshot of final dashboard (submission requirement)
- 📄 README.md – Task summary and steps followed

---

## 🧰 Tools Used

- **Tableau Desktop** – Data visualization and dashboard creation  
- **Daikibo Telemetry Dataset** – JSON file provided in the simulation  

---

## 👨‍💼 Program Info

**Deloitte Data Analysis Virtual Job Simulation**  
Hosted on: [Forage](https://www.theforage.com)

---

## 📌 Note

The dashboard demonstrates:
- Use of **calculated fields**
- **Interactive filtering** between visuals
- Identification of **operational inefficiencies** across factories and devices

---

