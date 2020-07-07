Exercise 1: Manage planned orders
=================================

Firm a Planned Order
--------------------

You need to firm a planned order in **Dynamics 365 for Finance and Operations**.

1.  Open **Master planning \> Master planning \> Planned orders**.

2.  In the **Planned orders** page, select the line for order number **004261**.

3.  Click the **Firm** button in the action pane.

4.  In the **Firming** page, in the **Update marking** field, select
    **Standard**.

5.  Click **OK**.

Review the purchase order
-------------------------

1.  Open **Procurement and sourcing \> Purchase orders \> All purchase orders**.

2.  In the **All purchase orders** page, sort the list by the **Delivery date**
    field.

3.  Verify the firmed order is now listed with a status of **Open order**.

4.  Close the pages.

Change a Planned Order Type
---------------------------

You need to change the planned order type for an order.

1.  Open **Master planning \> Master planning \> Planned orders**.

2.  In the **Planned orders** page, select the line for order number **004262**.

3.  Select the **Planned order** tab in the action pane.

4.  Click the **Change to …** drop-down arrow in the **Maintain** area.

5.  Select **Planned production order**.

6.  In the **Change to planned production order** page, click **OK**.

Review the planned order and verify the change
----------------------------------------------

1.  In the **Planned orders** list page, verify that the **Reference** field has
    been updated to **Planned production orders** for order number **004262**.

2.  Close the pages.

Exercise 2: Create and run intercompany master plans
====================================================

Create an Intercompany Planning Group
-------------------------------------

As the materials and production scheduling manager, you need to develop a new
intercompany planning group. Assemblies are shipped from DEMF to USMF. While at
USMF they are painted and finished with the North American logo. Then they are
transferred to the USRT operation for sale. Use the Plans 20, DynPlan, and
MasterPlan respectively to accomplish this goal.

1.  Create an intercompany planning group.

2.  In the USMF Company, click **Show navigation pane**.

3.  Open **Master planning \> Setup \> Intercompany planning groups.**

4.  Click **New** in the Action pane.

5.  Enter Intercompany Extended Group in the **Name** field.

6.  Click **Save**.

7.  Click **New** on the tool bar for Intercompany planning group members tab.

8.  Select DEMF in the **Legal entity** field.

9.  Enter 0 in the **Scheduling sequence** field.

10. Click **New** on the tool bar for Intercompany planning group members tab.

11. Select **Legal entity - DEMF**, **Scheduling sequence - 0, Master plan –
    20.**

12. Leave **Automatic Copy to Static Plan** and **Automatic Copy to Dynamic
    Plan** checkboxes blank.

13. Click **Save.**

Assign item allocation key
--------------------------

1.  Select **Master Planning \> Demand Forecasting \> Item Allocation Keys.**

2.  Select **Wizard.**

3.  Select **Apples** from **Item Group** drop-down menu.

4.  Type **Apples Group** in **Name** box.

5.  Click **Next.**

6.  Click **Next** on the **Overview** page after verifying information is
    correct.

7.  Click **Finish** on the **Completed** page after verifying information is
    correct.

8.  Select **Demand Forecasting \> Intercompany Planning Groups.**

9.  Select **Item Allocation Keys.**

10. Select **Apples** under the **Unassigned Item Allocation Keys** box, then
    select **\>** to move it to the **Assigned Allocation Keys** box.

Run an Intercompany Master Plan
-------------------------------

As the materials and production manager, you will need run the Intercompany plan
utilizing the Intercompany planning group that you created earlier. View the
results in the Intercompany supply and demand form.

1.  In the USMF company, click **Show navigation pane**.

2.  Open **Master planning** \> **Run** \> **Intercompany master planning**.

3.  Select **60** for **Intercompany planning group**.

4.  Select **2** for **Number of intercompany planning iterations**.

5.  Select **Regeneration** for **First iteration**.

6.  Select **Net change** for **Subsequent iteration**.

7.  Select **Track processing time** setting slider to **No**.

8.  Set **Number of threads** to **0**.

9.  Click **Run in the background.**

10. Click Ok.

11. Open **Master planning \> Inquiries and reports \> Intercompany master
    planning \> Intercompany supply and demand.**
