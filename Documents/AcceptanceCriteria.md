# Acceptance Criteria — Medical Claim Denial Analysis System

## Feature: Denial Analytics Dashboard

### AC-01: Denial KPIs Visibility
Given the dashboard is loaded  
When a user views the landing page  
Then key KPIs must display:
- Total Claims
- Total Denied Claims
- Denial Rate %
- Preventable Denied %

### AC-02: Drilldown to Claim Details
Given a user selects a denial category or payer filter  
When the user clicks on a chart or table row  
Then the claim-level table must update to show only relevant denied claims

### AC-03: Preventable Denial Identification
Given denial data is categorized by reason  
When reason category = Coding or Eligibility  
Then the dashboard must count these denials as Preventable

### AC-04: Filters Sync Across Visuals
Given a user applies filters such as Payer, Category, Department, or Date  
When visuals refresh  
Then all KPIs, charts, and tables must reflect filtered context consistently

### AC-05: Trend Visibility
Given historical claim and denial data exists  
When the user views the Denial Trend chart  
Then Denial Rate % must display monthly or quarterly changes correctly

### AC-06: Performance
Given standard dataset volume  
When the dashboard loads  
Then all visuals must render within 5 seconds
