# Zomato Global Restaurant Analytics | Power BI

## 📊 Project Overview
This project analyzes global restaurant data from Zomato to uncover insights into restaurant performance, pricing, customer ratings, and cuisine diversity across continents, countries, and cities.

The objective was to convert fragmented Excel data into a single, interactive Power BI dashboard that enables both high-level and granular business analysis.

---

## 🎯 Business Goals
- Analyze total restaurant distribution globally
- Enable drill-down analysis by continent, country, and city
- Identify top-performing restaurants by:
  - Average customer rating
  - Lowest average cost
- Compare restaurants by:
  - Services offered (online delivery, table booking)
  - Rating color categories
- Analyze cuisine diversity and top cuisine-serving restaurants
- Deliver a responsive, multi-page Power BI report (web + mobile)

---

## 🗂️ Data Sources
- Excel datasets segmented by continent:
  - Africa, Asia, Europe, North America, South America, Oceania
- Country-Code dimension table
- Central Fact Table

---

## 🔧 Data Preparation
- Cleaned inconsistent city names and encoding issues
- Removed unused columns for performance optimization
- Split restaurant name and address fields
- Created a separate cuisines dimension table
- Ensured unique and non-null values in dimension tables

---

## 🧠 Data Modeling
- Star schema data model
- Proper cardinality and cross-filter directions
- Custom geography hierarchy:
  - Continent → Country → City
- Countries grouped into continents using lookup logic

---

## 📐 DAX Measures
- Restaurant Count
- Average Cost
- Average Rating
- Cuisine Count

### Rating Color Logic
| Rating Range | Color |
|-------------|-------|
| Above 4.5 | Dark Green |
| 4.0 – 4.4 | Green |
| 3.5 – 3.9 | Yellow |
| 2.5 – 3.4 | Orange |
| 1.8 – 2.4 | Red |
| Below 1.7 | White |

---

## 📈 Dashboard Features
- KPI cards for cost, rating, and restaurant count
- Interactive map with drill-down hierarchy
- Dynamic slicers for geography, ratings, and services
- Restaurant-level detail view (address, cuisines, cost, rating)
- Multi-page navigation
- Mobile-optimized dashboard views

---

## 🚀 Deployment
- Published to Power BI Service
- Public web access enabled
- Responsive mobile layout designed

---

## 🧰 Tools & Technologies
- Power BI
- Power Query
- DAX
- Excel
- Data Modeling & Visualization

---

## 📷 Dashboard Preview
See `/dashboards/web_view` and `/dashboards/mobile_view` for screenshots.

---

## 📌 Business Impact
- Enabled leadership to compare restaurant performance across 15+ countries
- Reduced manual reporting effort through automated dashboards
- Improved decision-making using interactive filters and drill-downs
