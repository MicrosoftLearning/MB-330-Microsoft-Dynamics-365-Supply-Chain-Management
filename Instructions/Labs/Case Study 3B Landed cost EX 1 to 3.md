---
lab:
    title: 'Case study 3B Landed cost'
    module: 'Module 3: Implement and manage supply chain processes'
---
Case study 3B Landed cost
=================================

Objectives
----------

- Set up landed cost parameters.
- Manage shipping containers.
- Set up Auto Cost.

Exercise \#1 Set up landed cost parameters
----------------------------------------------

Scenario
---------
In this exercise, you’ll help the system administrator at USMF use the Landed cost parameters page to set up general information and configuration settings that are used across the Landed cost module for posting, status updates, number sequences, and behavior.

*Objective: Set up landed cost parameters.*

### Set up the General tab

1. Open **Inventory management \> Setup \> Landed cost \> Landed cost parameters**.
2. On the **General** tab, select the General FastTab.
3. Set **Use shipping rate** to **Yes**. A shipping rate is set for a defined period and is used to estimate costs of goods that use multiple currencies.
4. Select your preferred rate type in the **Exchange rate type** field. This will be the default collection of exchange rates used for multi-currency calculations for a voyage and voyage costs.
5. Set **Update purchase order quantity** to **Accept**.
6. On the **Costing** FastTab, set **Posting specification** to **Total**.
    o **Total** – A total figure is posted to the ledger.
    o **Item group** – The adjustment is specified per item group.
    o **Item number** – The adjustment is specified per item. This value provides the most detail.
7. Set **Allow zero costs** to **No** to show an error if a user tries to post a cost estimate for a voyage invoice or purchase order that doesn't include a value for the expected voyage cost.

#### Make Landed cost features visible

1. On the **Feature visibility** tab, set **Activate** to **Yes** to turn on Landed cost features.
Note: Even when this option is set to **No**, the module itself, including the **Landed cost parameters** page, will remain available to users who have the correct permissions to access it.
2. Select Save.


Exercise \#2 Create shipping containers for voyages
-------------------------------------------------------------------------------------------

### Scenario
---------
USMF recently implemented Dynamics 365 Supply Chain Management. A newly hired employee wants to know how to create shipping containers. The employee wants to group goods that are physically grouped together or in cases where costs must be shared only across those goods, usually because they're physically together.
You’ll need to assist the employee with the following tasks:
    - Create a voyage.
    - Add a purchase order to a staging list.
    - Add a staging list to a shipping container.

*Objective: Manage shipping containers*

### Create a voyage

1. Go to Landed cost, select Voyages, then select All voyages.
2. In the Action pane, select + New.
3. In the Description field, enter Shipping1.
4. In the Booking reference field, enter 1111.
5. In the Vessel field, select ABC357806.
6. In the Mode of delivery field, enter 40.
7. In the Shipping company field, select 1002.
8. Select OK. 


### Add a purchase order to a staging list
1.	On the Action pane, select Voyage editor.
2.	In the Setup name field, select Inquiry.
3.	On the Inbound orders FastTab, select the first two purchase orders. 
4.	On the Lines to select FastTab, select the checkbox for each purchase order line that you want to include in the new shipping container.
5.	On the Lines to select FastTab on the toolbar, select Add to staging list.



### Add a staging list to a shipping container
1.	On the toolbar, select View staging list.
The Add staging list to shipping container page is opened. The purchase order lines that you selected are listed on the Lines in staging list FastTab. All the purchase order lines in this list will be added to the shipping container that you create. You can remove any line by selecting it and then selecting Remove line on the toolbar of the FastTab.
2.	On the Lines in staging list FastTab, on the toolbar, select Add to new shipping container.
3.	In the Shipping container field, select ECMU4657496.
4.	In the Journey template field, select AUMEL-AKLNZ.
5.	In the Shipping container type field, select 40'FCL.
6.	Select OK.


Exercise \#3 Set up Auto Cost
-------------------------------------------------------------------------------------------

### Scenario
---------
Now you’ll help the IT manager at USMF set up Auto Cost for transactions so that the cost will apply whenever any product is transported by any ship.

*Objective: Set up Auto Cost*

### 

1. Go to **Landed Cost** \> **Setup** \> **Costing Setup** \> **Auto Costs**. 
2. In the Cost area field, select Voyage
3. Select + New.
4. In the Account Code field, select All. This signifies that the Auto Cost Setup applies to all created voyages. Alternatively, you can set it to a specific vendor cost type group or designate a particular shipping company by choosing Group or Table, respectively.
5. In the Mode of delivery field, select 40.
6. In the From port field, select USLGB.
7. In the To port field, select CNNGB.
8. On the Lines FastTab, select + Add.
9. In the Cost type code field, select Air.
10. In the Apportionment method field, select Quantity.
11. In the Category field, select Percent.
12. In the Cost value field, enter 10.
13. Select Save.

