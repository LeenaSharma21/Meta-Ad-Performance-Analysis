**Total Impressions**

Total Impressions = COUNTROWS(FILTER('ad_events', 'ad_events'[event_type] = "Impression"))

**Total Clicks**

Total Clicks = COUNTROWS(FILTER('ad_events', 'ad_events'[event_type] = "Click"))

**CTR % (Click-Through Rate):**

CTR % = DIVIDE([Total Clicks], [Total Impressions], 0)

2. Efficiency & Cost Metrics

   **Total Ad Spend**
   Total Spend = SUM('campaigns'[total_budget])

   **CPC (Cost Per Click)**
   CPC = DIVIDE([Total Spend], [Total Clicks], 0)

   **CPM (Cost Per 1,000 Impressions)**
   CPM = DIVIDE([Total Spend], [Total Impressions], 0) * 1000

3. Conversion & ROI Metrics

   **Total Conversions (Purchases)**
   Total Purchases = COUNTROWS(FILTER('ad_events', 'ad_events'[event_type] = "Purchase"))

   **Conversion Rate %:**
   Conv. Rate % = DIVIDE([Total Purchases], [Total Clicks], 0)
