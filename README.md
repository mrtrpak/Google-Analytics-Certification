# Google-Analytics-Certification

## Why Google Analytics

- If **marketer, business owner or entrepreneur** then is probably most important tool to use.
- Thrive on the ability to make data-driven decisions.
-  Gives you the metrics to see what is working and what isn't working.
-  Flying blind without analytics in place. "If you can't measure it, you can't prove it." Peter Drucker
-  Is the **industry standard** for web analytics and is a requirement for digital marketing or ads.

## How Does Google Analytics Works

- To collect data, a small piece of **tracking code** is added to EACH page on a website. 
- The code will collect **anonymous** info about a visitor interactions with the site.
- Google Analytics can calculate which pages are most popular or determine if users reached purchase page.
- Collect info like **language of browser, type of browser, the device used, operating system used, 
users location, age and gender.**
- Also collects the **"traffic source"** which brought the user to the site in the first place.
- EX: search engine, ad clicked on or an email marketing campaign.
- Uses a **Browser cookie** (small bit of text stored in the browser) to generate random ID to 
distinguish between new and returning visitors and tie all the activity of a visitor into single visit.
- Each period of activity is called a **session**. It ends a session by default after **30 minutes** of 
inactivity or when a user closes a browser.
- All this info is sent to Google Analytics to populate your reports.

## Google Analytics Setup

1) Create or sign in to Analytics account
2) Setup a property (represents your website or app and is the collection point in Analytics for data).
3) Add the tracking code to site. Admin > tracking info > add after opening tag on each page.
4) Verifty code is working by opening up website in separate tab and check Analytics.

## Create Reporting Views

- **Views:** The level in an Analytics account where you can access reports and analysis tools.
- **Google Analytics recommends** you setup at least **3 views:** a "raw data", "test" and "master" view.

- **Raw Data View:** left unfiltered and untouched. Can always go back to all the data that was collected.
- **Test View:** test new filters to see how traffic gets affected. Test first to make sure you are not
filtrating any visitors that you otherwise would expect to show up to have more reliable data.
- **Master View:** main view to use to read your data day to day. Already tested filters are added here.

**How to Create Additional Views**
1) **Add a new reporting view.** Admin section of your property and click "create view".
2) **Add view name and timezone.** Then click "create view".

**Limits and Caveats of Views**
- default unfiltered view will be called **"All Website Data"** and can rename view to match view name 
recommendations by Google Analytics.
- When new view is created only the website data from the **date the view was created** is included.
- If you delete a view you have **35 Days** to restore the view.

**Account Structure**
- **Account:** Access point for analytics and the top-most level of organization.
- **Property:** Website, mobile app or device. Up to **50 Properties** for each account.
- **View:** Access point for reports. Defined view of data from property. Up to **25 Views** to per property.

**Why Create Additional Views?**
- When you add a property to an account, Analytics creates a **reporting view** for that property.
- **Best practice** to leave the original view unchanged. Then always has **backup** of raw data.
- Can create additional views and apply filters to them to view a specific subset of data
- **You want to do this b/c:**
    - **Convenience:** if consistently need to look at a particular subset of data, it is easier to 
    have a view that is dedicated to that data.
    - **Data Security:** give the editorial team access to analytics reports about company, but can
    restrict access to sensitive data.
    - **Data Accuracy:** filter data like spam traffic or internal traffic.

## Add Filters to Views

**Common Filters:**
- **Exclude Internal Traffic:** Won't skew data with internkal traffic. Filter to exclude traffic from head office.
- **Filter Domain Referrals:** Reduce spam traffic from data. Filter that excludes traffic from selected domians.
- **Filter on Geography:** Consolidate countries into sales regions. Can track data from a region
that is spread across multiple countries.
- **Search-and-Replace Filter:** Replace codes or long urls with simpler more intuitive versions.
For example replacing the product ID with the product name. 

**How to Set Up Filters:**
1) Create a Filter: got admin > filters > create a filter. Need edit access to add filters to views.
2) Define the filter: add filter name, select the filter type and specify the info to include or exclude.

**Limits and Caveats to Filters:**
- Filters require up to **24 hours** beore they are applied to the data.
- **Filter order does matter**. Filters are applied in the order in which they are set in your view.
If there is a chance one filter influences the other you can assign a filter order.
- **Filters are destructive**. If a filter excludes data from a view, that data can never be 
recovered for that view. Should ALWAYS maintain an unfiltered view of your data so you always have 
access to your full data set.
- **Filters cannot be applied retroactively**. Data that has been processed already will not be filtered out of reports. Set your filters up ASAP.

## Google Analytics Goals

- **Goals:** measure how well your site or app fulfills your target objectives.

**Benefits of Setting up Goals:**
- measure how often users complete an activity, conversion, that contributes to the success of your business not just the number of pageviews and visitors.
- See data in your **goal reports** and any other report that provide data on goals and goal conversion.
- Identify the **traffic source** that delivers the most conversions not just visitors.
- Identify the subset of users who contribute the most to conversions not just page visits.
- Track the **exact pathways** users take before completing a Goal.
- Track number of completions from individual **marketing campaigns.**

**How to Setup Goals:**
1) Add a new goal. Go into Admin > Views > Goals > New Goal. Need edit access to create goals.
2) Complete the goal description. Enter the goal name and choose goal type. 
3) Enter the goal details. EX: enter the URL of the page that is shown when the user converts or
completes the conversion process. Click "Verify" at the bottom to ensure it's working.
**Optional Steps**
- Add a goal value. If each sign-up is worth $1 you can set the goal value equal to 1. If wanted to 
track ACTUAL REVENUE we would need to turn on **Ecommerce Tracking**.
- Add a funnel. Measure drop off at each step of the goal completion process. (best for Ecommerce)

**Setup Ecommerce Tracking:** (optional goals step)
- **Ecommerce Tracking** measures transactions and revenue. 
- Go to Admin > Ecommerce settings > enable Ecommerce and implement added Ecommerce tracking code.

**Key Goal Reports:**
- **Goal URLs:** See which pages the goals were completed on.
- **Reverse Goal Path:** Shows the 3 steps users took prior to completing selected goal. As well as
the page on which they completed the goal.
- **Funnel Visualization:** Funnel reports take reverse goal path a step further and shows you the 
drop out and success rates of each step leading up to a conversion.
- **Goal Flow Report:** improved version of the funnel report. More flexible report (segments can be added) and better able to show converters who skipped steps in the conversion funnel.

**Limits and Caveats of Google Analytics Goals:**
- Goals are limited to **20** per reporting view.
- Goals **CANNOT be applied retrospectively** to data already collected. Create goals when setup property.
- **A conversion is counted once per session per configured goal.** Only 1 conversion can be applied to each session.
- **Event Goals:** tracking clicks to call for example. Requires setup of event tracking.
- **Smart Goals:** specifically designed to help Google Ads user who don't have enough conversions
to use the Google Ads optimization tools.
