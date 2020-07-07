Exercise: Configure mobile devices
==================================

In preparation for setting up the mobile device for your warehouse, you are
asked to first set up a Work class, which you will name Purch-Orders. It will
have the Put location types of Bay-door, Bulk, and Pick.

Add a work class
----------------

1.  In company **USMF**, open **Warehouse management \> Setup \> Work \> Work
    classes**.

2.  Click **New** to create a work class.

3.  In the **Work class ID** field, enter **P-Orders.**

4.  For **Description**, enter **Purchase Orders.**

5.  For **Work order type**, select **Purchase orders.**

6.  On the **Valid put location types** FastTab, click **New.**

7.  Enter **Baydoor.**

8.  Click **New** again.

9.  Enter **Bulk**.

10. Click **New** again.

11. Enter **Pack**.

Create a Mobile Device Menu Item and Menu
-----------------------------------------

As Warehouse manager in Seahorse Retailers, you have to configure the mobile
device options. You will be setting up two functions: Purchase order receive and
Purchase order put away. You will then add them to your Mobile device menu.

### Set up mobile device menu items

1.  Open **Warehouse management \> Setup \> Mobile device \> Mobile device menu
    items**.

2.  Click on **New**

3.  For **Menu item name**, enter **PO Receive**

4.  For **Title**, enter **PO Receive**

5.  For **Mode**, select **Work**

6.  Set the U**se existing work** slider to **No**.

7.  On the **General** FastTab, on **Work creation process**, select **Purchase
    order line receiving.**

8.  Set the **License plate grouping policy option** to **License plate
    grouping**.

9.  Set the **Generate license plate** slider to **Yes**

10. Set all other sliders to No.

11. Click **Save** in the action pane.

12. Click **New** in the action pane.

13. For **Menu item name**, enter **PO Putaway**

14. For **Title**, enter **PO Putaway**

15. For **Mode**, select **Work**

16. Set the **Use existing work** slider to **Yes**.

17. On the **General** FastTab, for Directed by, select User grouping

18. Set the **Group put away** slider to Yes.

19. Set all remaining sliders to **No**.

20. On **Work classes** FastTab, click **New.**

21. For **Work class ID**, select **P-Orders.**

22. Click **Save** in the action pane.

23. Close the page.

### Set up a mobile device menu.

1.  Open **Warehouse management \> Setup \> Mobile device \> Mobile device
    menu**.

2.  Select **Inbound** in the left menu bar and click **Edit** in the action
    pane.

3.  In the **AVAILABLE MENU AND MENU ITEMS** pane, select **PO Receive** and
    click the right directional arrow.

4.  In the **AVAILABLE MENU AND MENU ITEMS**, select **PO Putaway** and click
    the right directional arrow.

5.  Click **Save** in the action pane.

6.  Close the form.

Create Mobile Device Users
--------------------------

As Warehouse manager in Seahorse Retailers, you have to configure the mobile
device users. Add Ted Howard as a worker with a user ID and User name as thoward
with a default warehouse of 62. His password will be 1234 on the mobile device.

### Set up a work user for the mobile device.

1.  Open **Warehouse management \> Setup \> Worker**.

2.  Click **New**.

3.  In the **Worker** field, select **Ted Howard**.

4.  On the **Users** FastTab, click **New**.

5.  For **User ID**, enter **thoward**.

6.  For **User name**, enter **thoward**.

7.  For default warehouse, select **62.**

8.  For **Menu name**, select **Main**.

9.  Click **Save** in the action pane.

10. For **Password**, enter **1234**.

11. For **Confirm password**, enter **1234**.

12. Click **Set password**.

13. Close the form.

Set up a mobile device menu item for completing work of type Purchase order
---------------------------------------------------------------------------

As a warehouse manager, you need to create a menu item that is used for
performing work of type Purchase order. The work class that’s associated with
the menu item determines which work is valid.

### Create a mobile device menu item

1.  **Go** to **Warehouse management \> Setup \> Mobile device \> Mobile device
    menu items.**

2.  Click **New**.

3.  In the **Menu item name** field, enter a unique value. For example, you
    could type POMove. Remember the value, you'll need it later.

4.  In the **Title** field, type PO Move. This is the title which will be
    displayed on the mobile device.

5.  In the **Mode** field, select 'Work'.

6.  Select **Yes** in the **Use existing work** field.

7.  The **Display inventory status** field determines whether the inventory
    status of the on-hand inventory will be displayed to the warehouse worker on
    the mobile device. Select **Yes**.

8.  In the **Directed by** field, select **'System grouping'**. When you select
    something in the Directed by field, additional fields appear in the
    **General** section on this page. The fields that appear depend on what you
    selected. When you select **System grouping**, two new fields are added.

9.  In the **System grouping** field, select **'WorkPoolId'**. When warehouse
    workers open this menu item, they’ll be asked to scan a Work pool ID. All
    work orders with this Work pool ID and open work order lines with one of the
    work classes added to this menu item will be pushed to the user.

10. In the **System grouping label** field, type **Work pool**. This is the text
    displayed to the user on the mobile device.

11. Select **Yes** in the **Override license plate during put** field. This
    option allows warehouse workers to override the target license plate when
    items are put down on a license plate-controlled location.

12. Select **Yes** in the Group put away field. If all the Put lines on the work
    order share the same location, the user will receive one combined Put
    instruction for all lines.

13. Expand the **Work classes** section.

14. Click **New**.

15. In the **Work class ID** field, type 'Purchase' and tab off. The work pool
    restricts the work that the menu item can be used for. In this case it will
    be used for open work order lines that have the Purchase work class ID.

16. Click **Save**.

### Set up work confirmation

1.  Click **Work confirmation setup** in the action pane.

2.  In the **Work type** field, select 'Pick'.

3.  Select the **Auto confirm** check box. The work instruction with work type
    Pick will be auto-confirmed. This instruction will not be presented to the
    user.

4.  Click **New**.

5.  In the **Work type** field, select 'Put'.

6.  Select the **Location confirmation** check box. The warehouse worker will be
    asked to perform a confirmation scan of the location, when the item is put
    down.

7.  Click **Save**.

8.  Close the work confirmation page.

9.  Close the Mobile menu item page.

### Add the menu item to a mobile device menu

1.  Go to **Mobile device** menu.

2.  Click **Edit**.

3.  Use the Quick Filter to find records. For example, filter on the Name field
    with a value of 'inbound'. You want to find the menu you use for inbound
    menu items. In **USMF** this is called Inbound.

4.  In the tree, select 'a value' POMove.

5.  Click on the arrow that points to the right.

6.  Click **Save**.

7.  Close the Mobile device menu page.
