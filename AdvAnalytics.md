# Advanced Google Analytics

## Advanced Configuration Settings

### Custom Dimensions

- **Dimensions:** describes data; gender, age, country, city, device, browser, source/medium are 
all examples of dimensions in standard Google Analytics reports. Report organizes dimensions into rows.

- **Scope:** for standard dimensions, Google auto categorises the scope. In custom dimensions 
you must select which scope the dimension value will be applied too. 

**4 types of Scope:** and (standart dimensions in Google and where they fit in each).
- **Hit:** Value applies to the single hit for which it is set. (Page, page title, event category)
- **Session:** Value applies to all hits in a single session. (Landing page, Campaign, Source/Medium)
- **User:** Value applies to all hits in current and future sessions. (Age, Gender, City/Country)
- **Product:** Value applies to the product that has been set. (Product, Product SKU, Product Category) -- Requires Enhanced Ecommerce --

**Benefits of Custom Dimensions:** 
- track dimensions not available in Google Analytics. Can import data from a CMS 
(Content Management System) like WordPress or CRM (Customer Relationship Managment) like Salesforce.

- Build reports using custom dimensions. Available in custom reports and available for use with
advanced segments. Can be used as secondary dimensions in standard reports.

- Analyze company specific data. Get actionable insights tailored to needs of business.

**Example:**
- Author: if running a multi-author blog, can create a custom dimension to capture "Author" data 
from your website. Then create a custom report with Author as the primary dimension to measure 
differences between authors. To help grow business see which authors are viewed more often.

- Other examples: shipping methods, logged in Users, Member type (free, paid, gold, platinum) 

**How to Setup Custom Dimensions:**
1) Add New = Go to Admin > Custom Definitions > Custom Dimensions (need edit access to add)
2) Enter the dimension Name and select Scope. **Scopes:** hit, session, user or product
3) Implement tracking code. Copy and paste into your platform to collect custom data. 
    - Don't forget to replace the dimension value with your own.
    - Different businesses will do this in different ways depending on data & collection method.
    - **Google Tag Manager** is great option for managing Custom Dimension tracking code.

**Limits and Caveats to Custom Dimensions:**
- Are not a must to implement but be aware of benefits.
- Can create up to 20 custom dimensions.
- Can't apply a custom dimension retroactively. Only apply to data that was collected afterwards.
- Should not send Personally Identifiable Information (PII) as values. This is Against Google's Terms of Service.
- Cannot be shared in the Solutions Gallery like goals, segments, dashboards and custom reports.
- **Cannot be deleted** but can be disabled.

### Custom Metrics

- Metrics: measures data; metrics will invariably be a number, ratio or percentage. Reports 
organize metrics into columns.

**Benefits of Custom Metrics:**
- Track metrics not available in Google Analytics. Can import data Google doesn't auto collect.
- Build reports are available in custom reports and for use with advanced segments.
- Analyze company-specific data. Actionable insights tailored to needs of the business.
- Can help see the impact of discounting/sales/promotions on any product brand.

**How to Setup Custom Metrics:**
1) Add a custom metric. Admin > Custom Definitions > Custom Metrics. Need edit access.
2) Select the scope. Custom Metrics only has scope options of hit or product.
3) Select the formatting type. Select Integer, Currency or Time. Hit CREATE.
4) Implement the tracking code. Copy and paste into platform.
    - Replace the metric value with your own.
    - Different businesses do this in different ways based on data collection method and data.
    - **Google Tag Manager** is a great option for managing Custom Metric tracking code.

### Event Tracking 

### Other Useful Configurations (Cross domain tracking, users Ids, etc.)
