Exercise 1: Create a new warehouse layout
=========================================

You need to create a warehouse in **USMF** by using "basic warehousing" in the
Inventory management module, not to warehouses created in the Warehouse
management module.

This warehouse has the following format for its location Aisle-Rack-Shelf which
will be represented with numerical values such as **001-01-01.**

The default location is 450 X 250 X 200 as width, depth and height. You do not
wish to create Outbound docks or Bulk locations.

Set the default location capacity
---------------------------------

1.  Go to **Inventory management \> Setup \> Inventory and warehouse management
    parameters**.

2.  Click the **Locations** tab.

3.  In the **Standard width** field, enter 450.

4.  In the **Standard depth** field, enter 250.

5.  In the **Standard height** field, enter 200.

6.  Click **Save**.

7.  Close the page.

Define the location name format
-------------------------------

1.  Go to **Inventory management \> Setup \> Inventory breakdown \>
    Warehouses**.

2.  Click **New**.

3.  In the **Warehouse** field, type 17.

4.  In the **Name** field, type Raw materials.

5.  In the **Site** field, click the drop-down button to open the lookup.

6.  In the list, find and select site 1.

7.  Expand the **Location names** section. The options in this section define
    the default format for location names. In our example, we'll include the
    aisle number, rack number and shelf number.

8.  Set the **Include aisle** option to Yes.

9.  Set the **Include rack** option to Yes.

10. In the **Format** field, for the rack, type -\#\#

11. Set the **Include shelf** option to Yes.

12. In the **Format** field, for the shelf, type -\#\#

13. Click **Save**

Define warehouse locations
--------------------------

1.  On the Action Pane, click **Warehouse**.

2.  Click **Location Wizard**.

3.  On the Welcome screen, click **Next**.

4.  De-select the **Outbound docks** option

5.  De-select the **Bulk locations** option

6.  Click **Next**.

7.  On the Create inventory aisles screen, click **Next**.

8.  On the Edit and delete aisles screen, click **Next**.

9.  On the Create inbound docks screen, click **Next**.

10. On the Edit and delete inbound docks screen, click **Next**.

11. On the Create picking locations screen, click **Next**.

12. On the Specify additional information for all your picking locations screen,
    note that the physical dimensions shown on this page are the ones that you
    set at the start of this procedure. Click **Next**.

13. On the Edit and delete picking locations screen, click **Next**.

14. Click **Finish**.

15. Close all pages.

Exercise 2: Create costing version, item model group and tracking number group
==============================================================================

As a warehouse employee at **USMF**, you need to create a standard cost version
to record products that use the item model group with inventory model of
**Standard.** You also need to group items based on FIFO inventory model.

Therefore, you need to create an item model group, a cost version and tracking
number group to allocate batch and serial numbers.

Create cost version
-------------------

1.  Go to **Cost management \> Predetermined cost policies setup \> Costing
    versions**.

2.  Click **New**.

3.  In the **Costing type** field, select 'Standard cost'.

4.  In the **Version** field, type 'SeahorseST'.

5.  In the **Name** field, type 'Seahorse Standard Costing '.

6.  In the **Block activation** field, select 'No'.

7.  Click **Save**.

8.  Close the page.

Create item model group
-----------------------

1.  Go to **Cost management \> Inventory accounting policies setup \> Item model
    groups**.

2.  Click **New**.

3.  In the **Item model group** field, type 'STDN'.

4.  In the **Name** field, type 'Standard Cost'.

5.  In the **Inventory model** field, select 'Standard cost'.

6.  Expand the **Inventory policies** section.

7.  In the **Approved vendor check** method field, select 'No check'.

8.  Click **New**.

9.  In the **Item model group** field, type 'FIFO2'.

10. In the **Name** field, type 'FIFO 2'.

11. Click **Save**.

12. Close the page.

Create Tracking number group
----------------------------

1.  Go to **Inventory management \> Setup \> Dimensions \> Tracking number
    groups**.

2.  Click **New**.

3.  In the **Number group** field, type 'ASer'.

4.  In the **Name** field, type 'Auto-Serial'.

5.  Select No in the **Date** field.

6.  Select No in the **Lot ID** field.

7.  Select Yes in the **Number sequence No.** field.

8.  Select Yes in the **Only for inventory transactions** field.

9.  Select Yes in the **On physical update** field.

10. Click **New**.

11. In the **Number group** field, type 'USer'.

12. In the **Name** field, type 'Unique-Serial'.

13. Select No in the **Date** field.

14. Select No in the **Lot ID** field.

15. Select Yes in the **Number sequence No**. field.

16. In the **Number sequence code** field, choose any number sequence of your
    choice

17. Select Yes in the **Only for inventory transactions** field.

18. Select Yes in the **On physical update** field.

19. Set **Per qty.** to '1'.

20. Click **New**.

21. In the **Number group** field, type 'Batch'.

22. In the **Name** field, type 'Auto Batch'.

23. Select No in the **Date** field.

24. Select No in the **Lot ID** field.

25. Select Yes in the **Number sequence** No. field.

26. In the **Number sequence code** field, choose any number sequence of your
    choice

27. Select Yes in the **Only for inventory transactions** field.

28. Select No in the **On physical update** field.

29. Close the page.
