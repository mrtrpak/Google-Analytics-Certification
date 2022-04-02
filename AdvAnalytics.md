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

**Limits and Caveats to Custom Metrics:**
- Not a must but should know and not avoid its benefits.
- Can create up to 20 Custom Metrics.
- Can't apply retroactively.
- Cannot be shared in the Solutions Gallery like goals, segments, dashboards and custom reports.
- Cannot be deleted but can be disabled.

### Event Tracking

- **Event Tracking:** allows you to capture user interactions on site which Google doesn't auto capture.

**Benefits of Event Tracking:**
- Track interactions Google Analytics Goals can't track (usually requires specific page to be 
loaded like thank you page). Allows you to track interactions on a single page.
- Better understanding user behavior. If users are engaging with your content and performing 
intended actions important for your site and business.
- View event tracking reports. All data collected is reported within the Event Tracking 
sub-section in the Behaviour Reports section.

**Example Events:**
- Click-to-call phone number
- External link clicks like third-party live chat
- Clicks on email addresses
- Video plays
- Podcast plays
- Selected color or size (ecommerce sites)
- Abondonment of form field
- Movement of mouse
- Scrolling down the page
- Clicks to social profiles

**How to Setup Event Tracking:**
1) Copy the tracking code template. To track an event a snippet of code is added to the link on 
your site you want to track. When the link is clicked the interaction is tracked and displayed as an event in Google Analytics.
    - Template: onclick="ga('send','event','Category','Action','Label','Value');"
2) Replace the template fields. replace category, action, label and value to describe user interaction on website.
    - **Category:** required; typically the object or group of objects that was interacted with
    - **Action:** required; type of interaction (play, download)
    - **Label:** optional; useful for summarising what the event is about (name of video or PDF)
    - **Value:** optional; numeric value associated with the event
3) Implement the tracking code. Add the link and event tracking code.
Or use **Google Tag Manager** to add the tracking code.
    - **Example:** 
    <ahref-"www.example.com/pdf/company.pdf"
    onclick="ga('send','event','PDF','Download','Company PDF Download');>
    *ANCHOR TEXT*</a>
    
**View Event Tracking Reporting:**
- View event reports: Click Behavior > Events > Overview to look at the events you have tracked
and see how it is performing.

### Other Useful Configurations (Cross domain tracking, users Ids, etc.)

- **Custom Session Settings:** set how long sessions can last.
    - By default sessions end after 30 minutes of inactivity or closes the browser.
    - Can extend the length if average users spend a lot more time on the site.
    - For example a game site a user may play for multiple hours in one session. 
    - Go to Admin > Session settings to ajust session timeout.

- **Cross-Domain Tracking:** track users and sessions across multiple domains.
    - w/o this the shopping behavior and checkout won't get linked together.
    - Google cannot like anonymous ID (client ID) by one domain to another domain.
    - setup cross-domain tracking using Google Tag Manager or modify tracking code.

- **User-ID:** track users across multiple devices and sessions.
    - by default Google will NOT be able to identify sessions from the same user when sessions
    happen in different browsers on the same device or browsers on different devices.
    - this is because anonymous ID (client ID) assigned by Google is stored in the browser.
    - to use this you must have a sign-in that generates your own IDs and be able to consistenly
    associate them with a set of data.
    - can set this up in the Admin section uder User ID.

- **Internal Site Search:** see how users search your site.
    - if you have a search field that customers can use on your site you can setup "site search"
    to track what search terms users enter.
    - helps identify missing or obscured content, optimize navigation and site layout, improve
    search results and even generate ideas for new keywords for marketing campaigns.
    - to setup go to Admin > View > View Settings. Enable site search tracking and enter the 
    "query parameter" that your website uses in the URL when users search on your site.
    
- **Custom Channel Group:** customize how Google Analytics groups channels in your reports.
    - by default Google groups your traffic sources using default channels: Organic, Social,
    Direct, Referral and Display.
    - to setup go to Admin > make a copy of the default channel grouping. 
    - Edit it to label your traffic in other ways for analysis.
    - example: move traffic source from "social" to "community".

- **Data Import:** upload data from external sources and combine it with data already collected.
    - data imports provide an alternative to collecting data by the JavaScript tracking code.
    - if importing custom dimensions and metric data, need to create custom dimensions and 
    metrics prior to uploading the data.
