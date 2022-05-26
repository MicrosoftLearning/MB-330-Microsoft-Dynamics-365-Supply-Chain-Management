---
lab:
    title: 'Case study 5 Master planning'
    module: 'Module 6: Implement master planning '
---
Case study 5 Master planning
============================

Objectives
----------

-   *Firm and review a planned purchase order, change it to production, and
    verify the change.*

-   *Create a planning group, assign an item allocation key, and run the
    intercompany master plan.*

Exercise \#1 Process and view planned orders
--------------------------------------------

*Objective: Firm and review a planned purchase order, change it to production,
and verify the change.*

The planning manager in USMF wants to know how to setup, manage, and use the
master planning module, as well as how to process planned orders.

To firm planned orders, He will need to be sure that the master planning is
running correctly, or there are some planned orders in the form that you can
use.

You were called to help the planning manager to perform the above tasks

You will need to use the following:

-   Firm a planned purchase order.

-   Review the purchase order.

-   Change the planned purchase order type.

-   Review the planned order and verify the change

### Firm a planned order

1.  Open **Master planning \> Master planning \> Planned orders**.

2.  On the **Planned orders** page, select the line for order number **004126**.

3.  Click the **Firm** button in the action pane.

4.  On the **Firming** page, in the **Update marking** field, select
    **Standard**.

5.  Click **OK**.

### Review the purchase order

1.  Open **Procurement and sourcing \> Purchase orders \> All purchase orders**.

2.  On the **All purchase orders** page, sort the list by the **Delivery date**
    field.

3.  Verify the firmed order is now listed with a status of **Open order**.

4.  Close the pages.

### Change a planned order type

You need to change the planned order type for an order.

1.  Open **Master planning \> Master planning \> Planned orders**.

2.  On the **Planned orders** page, select the line for order number **004137**.

3.  Select the **Planned order** tab in the action pane.

4.  Click the **Change to …** drop-down arrow in the **Maintain** area.

5.  Select **Planned production order**.

6.  On the **Change to planned production order** page, click **OK**.

### Review the planned order and verify the change

1.  On the **Planned orders** list page, verify that the **Reference** field has
    been updated to **Planned production orders** for order number **004262**.

2.  Close the pages.

Exercise \#2 Create and run intercompany master plans
-----------------------------------------------------

*Objective: Create a planning group, assign an item allocation key, and run the
intercompany master plan.*

You were called to help the materials and production scheduling manager, to
develop a new intercompany planning group.

Assemblies are shipped from DEMF to USMF.

While at USMF they are painted and finished with the North American logo.

Then they are transferred to the USRT operation for sale.

He wants to use the Plans 20, DynPlan, and MasterPlan respectively to accomplish
this goal.

He would like to validate the Intercompany master planning parameters and
perform some setups before running the intercompany master plan.

Then he would need to run the intercompany plan using the planning group that he
will create. Finally he would want to view the results in the intercompany
supply and demand form.

Would you assist the planning manager in doing the following?

-   Create an intercompany planning group.

-   Assign an item allocation key.

-   Run an intercompany master plan.

### Create an intercompany planning group

1.  In the USMF Company, click **Show navigation pane**.

2.  Open **Master planning \> Setup \> Intercompany planning groups.**

3.  Click **New** on the Action pane.

4.  Enter **Intercompa** in the **Name** field and **Intercompany Extended Group** in the description.

5.  Click **Save**.

6.  Click **New** on the tool bar for Intercompany planning group members tab.

7.  Select DEMF in the **Legal entity** field.

8.  Enter 0 in the **Scheduling sequence** field.

9.  Select **20** for the **Master plan** field.

10. Leave **Automatic Copy to Static Plan** and **Automatic Copy to Dynamic
    Plan** checkboxes blank.

11. Click **Save**.

### Assign item allocation key

1.  Select **Master Planning \> Setup \> Demand Forecasting \> Item Allocation Keys.**

2.  Select **Wizard**.

3.  Select **Audio** from **Item Group** drop-down menu.

4.  Type **Audio Group** in **Name** box.

5.  Click **Next**.

6.  Click **Next** on the **Overview** page after verifying information is
    correct.

7.  Click **Finish** on the **Completed** page after verifying information is
    correct.
    
8.  Switch to the **DEMF** company. Repeat steps 1 - 7.

9.  Switch to the **USMF** company.

10.  Select **Demand Forecasting \> Intercompany Planning Groups.**

11.  Select **Item Allocation Keys.**

12. Select **Apples** under the **Unassigned Item Allocation Keys** box, then

13. Select **Audio** under the **Unassigned Item Allocation Keys** box, then
 
14. Select **\>** to move it to the **Assigned Allocation Keys** box.

### Run an intercompany master plan

1.  As the materials and production manager, you will need run the intercompany
    plan utilizing the intercompany planning group that you created earlier.
    View the results in the intercompany supply and demand form.

2.  In the USMF company, click **Show navigation pane**.

3.  Open **Master planning** \> **Run** \> **Intercompany master planning**.

4.  Select **Intercompa** for **Intercompany planning group**.

5.  Select **2** for **Number of intercompany planning iterations**.

6.  Select **Regeneration** for **First iteration**.

7.  Select **Net change** for **Subsequent iteration**.

8.  Select **Track processing time** setting slider to **No**.

9.  Set **Number of threads** to **0**.

10. Click **Run in the background.**

11. Click **OK**.

12. Open **Master planning \> Inquiries and reports \> Intercompany master
    planning \> Intercompany supply and demand.**
