# README - Internship Tasks

## Overview
This document outlines six internship tasks that involve data visualization in a dashboard. The tasks require filtering and displaying charts based on specific criteria, including job roles, qualifications, locations, preferences, and time-based visibility.

## Prerequisites
- Tableau or any data visualization tool.
- Access to the dataset containing company details, job postings, user preferences, and geographic information.
- A dataset with attributes: `Company Name`, `Role`, `Job Title`, `Country`, `Preference`, `Latitude`, `Longitude`, `Qualification`, `Work Type`, `Experience`, `Salary Range`, `Job Portal`, `Company Size`, `Contact Person`, and `Job Posting Date`.

## Tasks

### Task 1: Top 20 Companies with UX Designers
- **Chart**: Bar Chart
- **Filters**:
  - Role: `User Experience Designer`
  - Job Title: `UI/UX Designer`
  - Company Name: More than 5 characters
- **Sorting**: Top 20 companies with maximum UX Designers

### Task 2: Top 10 Companies with Data Engineers
- **Chart**: Bar Chart
- **Filters**:
  - Role: `Data Engineer`
  - Job Title: `Data Scientist`
  - Country: Exclude Asian countries, ignore countries starting with `C`
  - Latitude: Above `10`
  - Preference: `Female`
  - Qualification: Only `B.Tech`
  - Job Posting Date: Between `01/01/2023` and `06/01/2023`
- **Time Constraint**: Visible only between `3 PM IST to 5 PM IST`
- **Note**: This task does not generate any output from the given dataset and conditions.

### Task 3: Preference vs Work Type (Internships)
- **Chart**: Scatter Plot
- **Filters**:
  - Work Type: `Intern`
  - Latitude: Below `10`
  - Country Name: Should not start with `A, B, C, D`
  - Job Title: Should not exceed `10 characters`
  - Company Size: Below `50,000`
- **Time Constraint**: Visible only between `3 PM IST to 5 PM IST`

### Task 4: Full-time Jobs in Africa
- **Chart**: Map Visualization
- **Filters**:
  - Qualification: `B.Tech, M.Tech, PhD`
  - Work Type: `Full Time`
  - Country: Only in Africa
  - Job Title: Starts with `D`
  - Preference: `Male`
  - Company Size: More than `80,000`
  - Contact Person: Starts with `A`
  - Job Portal: `Indeed`
- **Additional Feature**: Click on `Latitude & Longitude` to open a map showing the exact location.
- **Time Constraint**: Visible only between `3 PM IST to 6 PM IST`
- **Note**: This task does not generate any output from the given dataset and conditions.

### Task 5: Data Science & Aerospace Engineering Jobs in India & Germany
- **Chart**: Bar Chart (Color-coded)
- **Filters**:
  - Country: `India` (Orange) & `Germany` (Green)
  - Qualification: `B.Tech`
  - Work Type: `Full Time`
  - Experience: More than `2 years`
  - Job Titles: `Data Scientist, Art Teacher, Aerospace Engineer`
  - Salary Range: More than `$10K`
  - Job Portal: `Indeed`
  - Preference: `Female`
  - Job Posting Date: Before `08/01/2023`
- **Time Constraint**: Visible only between `3 PM IST to 5 PM IST`

### Task 6: Mechanical Engineers in Asia
- **Chart**: Bar Chart
- **Filters**:
  - Company Size: Less than `50,000`
  - Job Title: `Mechanical Engineer`
  - Experience: More than `5 years`
  - Country: Asian countries
  - Salary Range: More than `$50K`
  - Work Type: `Part Time` & `Full Time` (Ignore others)
  - Preference: `Male`
  - Job Portal: `Idealist`
- **Time Constraint**: Visible only between `3 PM IST to 5 PM IST`

## Implementation Notes
- **Data Processing**:
  - Ensure that the dataset has cleaned and structured values.
  - Use calculated fields in Tableau for filters and time-based visibility.
- **Time-based Visibility**:
  - Use `NOW()` or `DATEPART('hour', NOW())` to filter data dynamically based on current IST time.
  - If using Tableau Server, ensure server time is converted to IST.
- **Color-Coding**:
  - Assign specific colors to categories for easy distinction.

## Conclusion
This document serves as a guide for implementing the internship tasks related to job data visualization in Tableau. Follow the constraints carefully to ensure accurate representation of data in the dashboard.

---
**Author:** Ankit Kumar

