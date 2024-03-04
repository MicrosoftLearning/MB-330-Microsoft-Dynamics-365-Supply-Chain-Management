---
lab:
    title: 'Case study 2B Sales and marketing: Customer trade agreements'
    module: 'Module 3: Implement and manage supply chain processes '
---
Case study 2B Sales and marketing
=================================

Objectives
----------

- *Create a customer trade agreement for specific customers, a specific item
    and for a certain date range.*

Exercise \#3 Create a customer trade agreement
----------------------------------------------

*Objective: Create a customer trade agreement for specific customers, a specific
item and for a certain date range.*

The sales managers always try to standardize the sales price list and discounts
(trade agreements) for products. Sometimes they create special price lists and
discounts for special customers.

The sales manager you are working with decided to create sales price trade
agreement for item A0001 for all retail customers accounts and to set that price
at \$20. she also want to add a validity date for that price.

In order to record this sales price in the system she will use the trade
agreement journal, so that whenever a sales order is created for item A0001 and
the customer is from the retail accounts group, the price will default to \$20.

**What would you do to guide her thru this entry?**

### Create a trade agreement named “Sales price adjustment

1. Go to **Sales and marketing**, then to **Prices and discounts**, and then to
    **Trade agreement journals**.

2. Select **New**.

3. Name: Select **S_Price**, **Sales price adjustment**.

4. Select the **Lines** button to open the journal.

5. Relation: Select **Price (sales)**.

6. Account code or Party code type: Select **Group**.

7. Account selection: Select **03**, **Retail accounts**.

8. Item code or Product code type: Select **Table**.

9. Item Relation: Select **A0001, HDMI 6' Cables**.

10. From: Enter **1**.

11. Amount in currency: Enter **20.00**.

12. Change to the **Details** tab.

13. From date: Select **February 15, 2017**.  

14. Lead time: Enter **2**.

15. Select **Validate** \> **Validate all lines**.

16. Select **OK**.

17. After successful validation, **post** the journal

18. Close all pages

