# E-commerce User Funnel Analysis

The objective is to Analyze user behavior in multi category E-commerce store to uncover friction points, product opportunities and potential optimizations in the user funnel.

## Data Overview
[Dataset](https://www.kaggle.com/datasets/mkechinov/ecommerce-behavior-data-from-multi-category-store/data?select=2019-Oct.csv)
- The dataset contains around ~42 million entries, featuring 9 columns providing information such as event_time, event_type, product_id, category_id, category_code, brand, price, user_id and user_session.

### Key Questions
1. Where are users dropping off in the funnel?
2. Are there peak hours where users are more likely to purchase?
3. Which product categories have higher conversion rates?
4. What patterns exist in multi-session or repeat behavior?
5. How can this data inform UX, promotions, or product strategy?

## Data loading & cleaning

Loaded the csv data using pandas; checked shape, info, head and converted data type.

## Data Preprocessing 

Extracted useful features like hour and day of week from event_time column.

## Event Funnel Conversion Rate

- Calculated how many users perform each type of event (view, cart, purchase).
- Analyzed Conversion rates for :
  * view → cart
  * cart → purchase
  * view → purchase

## Event Distribution over time

- Checked how events are distributed across hours of the day which shows the `peak hours` where purchases are more likely to be made.

![image](https://github.com/user-attachments/assets/6c403bf2-8e16-476f-96da-9f6f4893113f)

## Session Funnel Breakdown

- Grouping by user session to analyze which combinations of actions/event (view,cart,purchase) occur within sessions to determine whether user's complete the funnel in single session or not.

## Product Funnel Breakdown by Category

- Exploring which product categories have highest conversion rate i.e. high view → purchase conversion rate.

## Key Visualizations

- To help stakeholders interpret the analysis quickly, we’ll visualize:
1. Top product categories by conversion

    ![image](https://github.com/user-attachments/assets/b21851de-12d8-45b2-bad5-08971f460b5e)

3. Purchase activity by hour of day

    ![image](https://github.com/user-attachments/assets/a6bc2307-92d9-4356-afd4-cc3a99fd2d5a)


# Key Insights
- Big drop off is from `view → cart`, suggesting the need for better product presentation, CTA's or indicators. 
- Time from `7-9 hrs` have peak purchase behavior. Consider aligning promotions or retargeting campaigns to this window.
- `Smartphones and appliances` have best Conversion rates. These categories may put in priority placement on the homepage or ad campaigns.
- Many users don't complete the funnel in one session. Retargeting or reminders could drive follow-through.


This analysis provides a baseline product analytics report that can support product and growth teams in identifying areas of friction and opportunity.

