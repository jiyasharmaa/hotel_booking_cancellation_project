# 🏨 Hotel Booking Cancellation & Guest Behavior Analysis

An end-to-end spreadsheet data analysis project examining **119,390 hotel booking records** across City and Resort hotels from **2015 to 2017**. Built using **WPS Office Spreadsheets**, this workbook features a cleaned dataset, structured Pivot Tables, and an interactive visual Dashboard uncovering key drivers behind reservation cancellations, guest demographics, and room assignment outcomes.

---

## 📊 Dataset & Workbook Structure
The workbook (`hotel_booking.xlsx`) is organized into three dedicated sheets:
1. **`hotel_booking.xlsx` (Cleaned Dataset):** 119,390 records × 14 refined columns covering hotel type, cancellation flags, arrival dates, party composition (`adults`, `children`, `babies`), country of origin, room types, and engineered analytical columns.
2. **`pivot` (Pivot Table Summaries):** Cross-tabulated summaries tracking total bookings vs. cancelled bookings across guest types, hotel categories, room assignment status, and arrival months.
3. **`Dashboard` (Interactive Visuals):** Executive visual summary translating pivot aggregations into charts for quick stakeholder insights.

---

## 🧹 Data Cleaning & Feature Engineering
To prepare the dataset for pivot analysis and dashboarding, the following transformations were applied:
* **Feature Selection:** Streamlined raw booking logs down to 14 high-impact operational and demographic fields.
* **Custom Categorization (`guest_type`):** Engineered a guest segmentation column classifying bookings into **Couples**, **Single** travelers, and **Family** groups based on adult, child, and baby counts.
* **Room Satisfaction Flag (`room_status`):** Created a derived status comparing `reserved_room_type` against `assigned_room_type` to categorize each stay as **Desired** (matched) or **Undesired** (reassigned).

---

## 🔍 Key Analytical Insights & Findings

* **Overall Booking & Cancellation Volume:**
  * Out of **119,390 total bookings**, **44,224** were cancelled (**37.04%** overall cancellation rate), while **75,166** resulted in successful check-outs.
* **City Hotel vs. Resort Hotel:**
  * **City Hotels** accounted for the majority of volume with **79,330 bookings** and **33,102 cancellations** (~41.7% cancellation rate).
  * **Resort Hotels** recorded **40,060 bookings** and **11,122 cancellations** (~27.8% cancellation rate).
* **Guest Type Breakdown:**
  * **Couples** represent the largest customer segment (**81,560 bookings**, **32,424 cancellations**), followed by **Single** travelers (**22,577 bookings**, **6,555 cancellations**) and **Families** (**15,253 bookings**, **5,245 cancellations**).
* **Room Assignment Impact:**
  * **104,473 guests** received their **Desired** room type, while **14,917** received an **Undesired** room reassignment—allowing operations teams to track room-matching efficiency alongside cancellations.
* **Seasonal Trends:**
  * Booking demand and cancellations peak during summer months (**July** with 12,661 bookings and **August** with 13,877 bookings) and dip sharply during winter (**November–January**).

---

## 🛠️ Tools & Techniques Used
* **Spreadsheet Environment:** WPS Office Spreadsheets
* **Techniques:** Data cleaning, conditional logic / feature engineering (`guest_type`, `room_status`), multi-table Pivot Tables, and Dashboard visualization.

---

## 📂 Repository Structure
```text
├── hotel_booking.xlsx    # Workbook containing Cleaned Data, Pivot Tables, and Dashboard
└── README.md             # Project documentation & analytical summary
