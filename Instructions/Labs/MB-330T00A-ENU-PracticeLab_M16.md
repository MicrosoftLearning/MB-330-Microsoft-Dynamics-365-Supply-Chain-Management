Exercise 1: Perform inbound operations
======================================

Perform a Purchase Order Receipt
--------------------------------

As a warehouse manager for Contoso Orange Juice, you need to process a purchase
order receipt using a mobile device. You have ordered 1 box of the Grapefruit
juice. These will be from Vendor US-112 and shipped to Warehouse 62. The unit
price will be \$2.50 per box.

Create a purchase order.
------------------------

1.  In **USP2**, Open **Accounts payable \> Purchase orders \> All purchase
    orders.**

2.  Click **New** in the action pane.

3.  Select **Vendor US-112**.

4.  On the **General** FastTab, enter storage dimensions of Site **3** and
    Warehouse **30**.

5.  Click **OK**.

6.  On the **Purchase order lines** FastTab, select item **P9500. Ignore any
    warnings.**

7.  Enter a quantity of **10.**

8.  Enter a unit price of **\$2.50**.

9.  On the Purchase tab of the action pane, in the **Actions** group, click
    **Confirm**.

10. Note your Purchase Order number.

11. Close the form.

Create a purchase order receipt using the mobile device.
--------------------------------------------------------

1.  Log in to the mobile device with the user you have enabled.

2.  Click **Inbound**.

3.  Click **Purchase receive**.

4.  Enter the purchase order number in the **PONUM** field.

5.  Click the green checkmark.

6.  Enter Item number **P9500**.

7.  Click the green checkmark.

8.  Enter a quantity of **1** in the **Qty** field.

9.  Click the green checkmark.

10. Click the green checkmark again.

11. Enter LP number **LP951**.

12. Click the green checkmark.

13. Enter today’s date as the vendor batch date.

14. Click the green checkmark.

15. Enter a date six months from the current date as the Expiry date.

16. Select the green check mark.

17. Select the Use as expiration date arrow.

18. Select No and select the green check mark.

19. For Country/Region of Origin 1, enter USA.

20. Select the green check mark.

21. Select the green check mark again to bypass the second Country/region entry.

22. Note the Work completed notification.

Exercise 2: Configure wave processing
=====================================

Configure wave processing
-------------------------

You need to set up the criteria that determine what work is generated for a
warehouse when a wave is processed, and whether waves are processed manually or
automatically. You specify the criteria by setting up wave templates and queries
that match a wave with released lines in sales orders, production orders, or
Kanban orders.

When you set up a wave template, you specify the sequence in which the templates
will be matched to released lines on sales orders, production orders, or Kanban.
When a line is released to the warehouse or to production, it uses the first
wave template that it meets the criteria for.

We recommend that you put templates with the most specific criteria at the top
of the list. The broader the criteria, the more likely it is for a line to meet
the criteria, and this could lead to lines being assigned to the wrong wave.

1.  In **USMF**, go to **Warehouse management \> Setup \> Waves \> Wave
    templates**.

2.  Click **New**.

3.  In the **Wave template name** field, type **GTL-Wave**.

4.  In the **Wave template description** field, type **GTL Wave**.

5.  In the **Site** field, enter or select site **2**.

6.  In the **Warehouse** field, enter **24**.

7.  Set the **Automate wave creation** field to **Yes**. Select this option to
    automatically create a wave when a sales order, production order, or kanban
    is released to the warehouse.

8.  Set the **Process wave at release to warehouse** option to **Yes**. Select
    this option to automatically process the wave and create work when a line is
    released to the warehouse.

9.  Set the **Automate wave release** option to Yes. Select this option to
    automatically release the wave. The picking work is created and made
    available on mobile devices.

10. Set the **Assign to open waves** option to Yes. Lines are assigned to waves
    based on the query filter for the wave template.

11. Set the **Process wave automatically at threshold** option to Yes. Select
    this option to automatically process the wave when its values reach the
    thresholds for weight, shipment, and lines specified in the Wave thresholds
    field group. This option is available only if Shipping is selected in the
    Wave template type field.

12. Set the **Automate replenishment work release** option to Yes. Select this
    option to create demand-based replenishment work and release it
    automatically. You must add the replenishment wave method to the wave
    template, and create a replenishment template of the type Wave demand.

13. Expand the **Methods** section. Wave template methods allow you to control
    the sequence of activities that each wave is going through when it’s
    processed. For example, you might have a method for wave replenishment. When
    you add a method, it’s automatically listed in the appropriate location in
    the sequence of steps. If you’ve set the Automate replenishment work release
    option to Yes, you need to add the replenish method here. Wave attributes
    act as filters, to restrict the kind of items that can use the wave. For
    example, you could specify an item group.

14. Click **Save**.

15. Close the wave templates page.

16. Go to **Warehouse management \> Setup \> Warehouse management parameters**.

17. Expand the **Wave processing** section.

18. In the **Wave processing batch group** field, enter or select a value.

19. Set the **Process waves in batch** option to Yes.

20. In the Wait for lock (ms) field, enter the time, in milliseconds, that an
    allocation step will wait for a system resource that is locked by another
    allocation step. When this time is exceeded, the wave is not processed and
    an error message is displayed.

21. Click **Save**.

22. Close the parameters page.

23. Go to **Production control \> Setup \> Production control parameters**.

24. In the **Release to warehouse** Production line release field, select an
    option. For sales orders and kanban orders, inventory must be reserved
    before the order is released to the warehouse. Otherwise, the items or
    allocation lines cannot be processed in a wave. For production orders, you
    also have the option of choosing Allow partial reservation. For example,
    this is useful if you have the materials that you need to start production,
    and can then wait until the additional materials become available to finish
    the process. If you select this option, you must manually repeat the release
    to warehouse process when the additional materials become available.

25. Close the parameters page.

Exercise 3: Perform cycle counting
==================================

Perform Cycle Counting Setup
----------------------------

As a warehouse manager in Orange Juice, you need to set up a cycle count for the
mobile device.

Set up a cycle counting adjustment type.
----------------------------------------

1.  In USP2, open **Warehouse management \> Setup \> Inventory \> Adjustment
    types**.

2.  Click **New** on the action pane.

3.  In the **Inventory adjustment type** field, enter **New Cycle Count**.

4.  In the **Description** field, enter **New Cycle Count.**

5.  In the **Name** field, select **Counting**

6.  Select the **Remove reservations** check box.

Set up warehouse management parameters for cycle counting.
----------------------------------------------------------

1.  Open **Warehouse management \> Setup \> Warehouse management parameters**.

2.  Click the **Cycle counting** tab on the left pane.

3.  In the **Default cycle counting adjustment type code** field, select **New
    Cycle Count**.

4.  In the **Default cycle count work class ID** field, make a selection.

5.  In the **Default cycle count work priority** field, enter **1**.

Set up a spot cycle counting menu item.
---------------------------------------

1.  Open **Warehouse management \> Setup \> Mobile device \> Mobile device menu
    items**.

2.  Click **New** in the action pane.

3.  In the **Menu item name** field, enter **Spot Cycle Count**.

4.  In the **Title** field, enter **Spot Cycle Count**.

5.  Select **Work** in the **Mode** field.

6.  Set the **Use existing work** slider to **Yes**.

7.  Click **Save** in the action pane.

8.  Set the **Display inventory status** slider to **Yes**.

9.  Select **System directed** in the **Directed by** field.

10. Expand the **Work classes** FastTab.

11. Click **New** in the FastTab.

12. Make a selection in the **Work class ID** field.

13. Click **Cycle Counting** in the action pane.

14. On the **Mobile device cycle counting** form, enter **2** in the **Number of
    attempts** field.

15. Click **OK** to close the form.

16. Click **Save** in the action pane.

Add the spot count menu item to the mobile device menu.
-------------------------------------------------------

1.  Open **Warehouse management \> Setup \> Mobile device \> Mobile device
    menu**.

2.  Select **Inbound** in the left-hand pane.

3.  Click Edit in the action pane.

4.  In the **Mobile device menus** section, select **Spot Cycle Count** from the
    **Available menus and menu items** list.

5.  Click the right directional arrow to add the menu item to the **Menu
    structure** list.

6.  Click **Save** in the action pane.

Define cycle counting
---------------------

Cycle counting is a warehouse process that you can use to audit on-hand
inventory items. This task recording shows how to set up the default counting
work priority, enable a mobile device menu item to process both picking and
counting operations, enable a counting threshold trigger when a location becomes
empty, and enable a cycle counting plan for a specific item in a specific
warehouse. Typically, these tasks are performed by a warehouse manager. You can
go through this procedure in the USMF demo data company or in your own data.

Set the priority of counting work
---------------------------------

1.  Go to **Warehouse management \> Setup \> Warehouse management parameters**.

2.  Click the **Cycle counting** tab.

3.  In the **Default cycle count work priority** field, enter a number. This
    step changes the priority of cycle counting work compared to other types of
    work in the warehouse. By entering a number that is lower than the number
    for other types of work, you raise the priority of the cycle counting work.

4.  Click **Save**.

5.  Close the page.

Enable the mobile device
------------------------

1.  Go to **Warehouse management \> Setup \> Mobile device \> Mobile device menu
    items**.

2.  Click **New**.

3.  In the **Menu item name** field, type a value.

4.  In the **Title** field, type a value.

5.  In the **Mode** field, select **'Work'**.

6.  Set the **Use existing work** option to Yes. When you set this option to
    Yes, the system will look for existing work when the mobile device menu item
    is used.

7.  In the **Directed by** field, select 'System directed'. When "System
    directed" is selected, the warehouse worker will be directed to open work
    that is in defined work classes. (We will create these work classes next.)

8.  Expand or collapse the **Work classes** section.

>   Next, we will create two work classes that will be used with this mobile
>   device menu item. When the menu item is used, these work classes will be
>   queried, and the work that has the highest priority will be shown to the
>   user.

1.  Click **New**.

2.  In the **Work class ID** field, select a value.

3.  Click **New**.

4.  In the **Work class ID** field, select a value.

5.  Click **Save**.

6.  Close the page.

7.  Go to **Warehouse management \> Setup \> Mobile device \> Mobile device
    menu**.

8.  In the tree, select the menu item that you just created.

9.  Click **Edit**.

10. Click the arrow to add the menu item to the menu.

11. Click **Save**.

Create a counting threshold
---------------------------

1.  Go to **Warehouse management \> Setup \> Cycle counting \> Cycle count
    thresholds**.

2.  Click **New**.

3.  In the **Cycle counting threshold ID** field, type a value.

4.  Set the **Process cycle counting immediately** option to Yes.

5.  In the **Description** field, type a value.

6.  Click **Save**.

7.  Click **Select locations**.

8.  In the **Criteria** field, select a value.

9.  Click **OK**.

10. Close the page.

Create a cycle count plan
-------------------------

1.  Go to **Warehouse management \> Setup \> Cycle counting \> Cycle count
    plans**.

2.  Click **New**.

3.  In the **Cycle counting plan ID** field, type a value.

4.  In the **Description** field, type a value.

5.  In the **Maximum number of cycle counts** field, enter a number.

6.  Click **Save**.

7.  Click **Select locations**.

8.  In the **Criteria** field, select a value.

9.  Click **OK**.

10. In the **Days between cycle counting** field, enter a number. For example,
    if the Days between cycle counting field is set to 5, cycle counting work
    will be created every five days. However, if cycle counting work is
    processed on day three, the next cycle counting work will be created five
    days after the last cycle counting was processed, on day 8.

11. Click **Save**.

12. In the Cycle count plan product selections area, click **New**.

13. In the **Sequence number** field, enter a number. The sort is from the
    smallest number to the largest number. The value must be more than 0 (zero).

14. In the **Description** field, type a value.

15. Click **Save**.

16. Click **Define product query**.

17. In the **Criteria** field, enter or select a value.

18. Click **OK**.

19. Close the page.

Define partial location cycle counting process
----------------------------------------------

When you use cycle count plans to create counting work, you can guide the actual
counting operations by requesting that only specific products and product
variants be counted instead of all on-hand inventory at the location. By
filtering on specific products, the warehouse manager can reduce review
overhead, help prevent consolidation mistakes, and save time. Typically, a
warehouse manager performs the setup tasks. You can go through this procedure in
the USMF demo data company or in your own data.

Create a work pool
------------------

1.  In USP2, Go to **Warehouse Management \> Setup \> Work \> Work pools**.

2.  Click **New**.

3.  For Work Pool ID, enter **WP001.**

4.  For description, enter **Work pool 001.**

5.  Click **Save**.

Create a cycle counting work template
-------------------------------------

1.  In USMF, go to **Warehouse management \> Setup \> Work \> Work templates**.

2.  In the **Work order type** field, select 'Cycle counting'.

3.  Click **New**.

4.  In the **Sequence number** field, enter a number. The sort order is from the
    smallest number to the largest number. The value must be more than 0 (zero).

5.  In the **Work template** field, type a value.

6.  In the **Work template description** field, type a value.

7.  In the **Work pool ID** field, enter or select a value.

8.  In the **Work priority** field, enter a number.

9.  Click **Save**. Ignore any warnings.

10. Under Work Template Details, click **New**.

11. In the **Work type** field, select 'Counting'.

12. In the **Work class ID** field, enter or select a value.

13. Click **Save**.

14. Click **Work line breaks**.

15. Click **New**.

16. In the **Sequence number** field, enter a number. The sort order is from the
    smallest number to the largest number. The value must be more than 0 (zero).

17. Click **Save**.

18. Close all pages.

Create a cycle counting plan
----------------------------

1.  Go to **Warehouse management \> Setup \> Cycle counting \> Cycle count
    plans**.

2.  Click **New**.

3.  In the **Cycle counting plan ID** field, type a value.

4.  In the **Description** field, type a value.

5.  In the **Maximum number of cycle counts** field, enter a number.

6.  In the **Work template** field, enter or select a value.

7.  In the Cycle count plan product selections area, click **New**.

8.  In the **Sequence number** field, enter a number. The sort order is from the
    smallest number to the largest number. The value must be more than 0 (zero).

9.  In the **Description** field, type a value.

10. Click **Save**.

11. Click **Define product query**.

12. In the **Criteria** field, enter or select a value.

13. Click **OK**.

14. Close the page.

Exercise 4: Perform transfers and replenishment
===============================================

**Set up transfer orders**

You need to perform setup for transfer orders for Contoso Orange Juice. To get
started, you need to create and link a transit warehouse, set up location
directives, and set up a work template.

**Create transit and production warehouses**

1.  Go to entity **USP2**.

2.  Open **Warehouse management \> Setup \> Warehouse \> Warehouses**.

3.  Select **New** to create a new warehouse.

4.  In the **Warehouse** field, enter **31**.

5.  In the **Name** field, enter **Site 3 - Transit Warehouse**.

6.  On the **General** FastTab, select **3** in the **Site** field.

7.  In the **Type** field, select **Transit**.

8.  Expand the **Warehouse** FastTab.

9.  Set the **Use warehouse management processes** slider to **Yes**.

10. Select **Save**.

11. Select **New** to create a new warehouse.

12. In the **Warehouse** field, enter **32**.

13. In the **Name** field, enter **Site 3 - Prod Warehouse**.

14. On the **General** FastTab, select **3** in the **Site** field.

15. Expand the **Warehouse** FastTab.

16. Set the **Use warehouse management processes** slider to **Yes**.

17. Select **Save**.

**Set up a location directive**

1.  Open **Warehouse management \> Setup \> Location directives**.

2.  Select **Transfer issue** in the **Work order type** field.

3.  Select **New** in the **Location directives** FastTab.

4.  Enter **Transfer Issue** in the **Name** field.

5.  On the **Location directives** FastTab, select **Pick** in the **Work type**
    field.

6.  In the **Site** field, select **3**.

7.  In the **Warehouse** field, select **30**.

8.  Click **Save**.

9.  Select **New** on the **Lines** FastTab.

10. Verify that the **Sequence number** field is **1**.

11. Enter **1000** in the **To quantity** field.

12. Select **None** in the **Locate quantity** field.

13. Click **Save**.

14. Expand the **Location Directive Actions** FastTab.

15. Select **New**.

16. Type **Bulk** in the **Name** field.

17. Select **Save**.

18. Select **New**.

19. Enter **Transfer Issue-Put** in the **Name** field.

20. Select **Put** in the **Work type** field.

21. In the **Site** field, select **3**.

22. In the **Warehouse** field, select **31**.

23. Select **New** on the **Lines** FastTab.

24. Verify that the **Sequence number** field is **1**.

25. Enter **1000** in the **To quantity** field.

26. Select **None** in the **Locate quantity** field.

27. Expand the **Location Directive Actions** FastTab.

28. Select **New**.

29. Type **Bulk** in the **Name** field.

30. Select **Save**.

31. In the left-hand pane, select **Transfer Receipt** in the **Work order
    type** field.

32. Select **New** in the Action Pane.

33. Enter **Transfer Issue** in the **Name** field.

34. Select **Pick** in the **Work type** field.

35. In the **Site** field, select **3**.

36. In the **Warehouse** field, select **31**.

37. Click **Save**.

38. Select **New** on the **Lines** FastTab.

39. Verify that the **Sequence number** field is **1**.

40. Enter **1000** in the **To quantity** field.

41. Select **None** in the **Locate quantity** field.

42. Click **Save**.

43. Expand the **Location Directive Actions** FastTab.

44. Select **New**.

45. Type **Bulk** in the **Name** field.

46. Select **Save**.

47. Select **New**.

48. Type **Transfer Issue-Put** in the **Name** field.

49. Select **Put** in the **Work type** field.

50. In the **Site** field, select **3**.

51. In the **Warehouse** field, select **32**.

52. Click **Save**.

53. Select **New** in the **Lines** FastTab.

54. Verify that the **Sequence number** field is **1**.

55. Type **1000** in the **To quantity** field.

56. Select **None** in the **Locate quantity** field.

57. Click **Save**.

58. Expand the **Location Directive Actions** FastTab.

59. Select **New**.

60. Type **Bulk** in the **Name** field.

61. Select **Save**.

Setup Work classes
------------------

1.  Go to **Warehouse management \> Setup \> Work \> Work classes**.

2.  Click **New**.

3.  In the **Work** class ID field, type **'Transfer2'**.

4.  In the Description field, type **'Transfer'**.

5.  In the Work order type field, select **'Transfer issue'**.

6.  Click **Save**.

7.  Close the page.

Set up a work template
----------------------

### Create transfer issues

1.  Open **Warehouse management \> Setup \> Work \> Work templates**.

2.  In the **Work order type** field, select **Transfer issue**.

3.  Select **New**.

4.  Type **Transfer Order Issue** in the **Work template** field.

5.  Type **Transfer Issue** in the **Work template description** field.

6.  Select **Save**.

7.  Select **New** in the **Work Template Details** area.

8.  Select **Pick** in the **Work type** field.

9.  Select the **Mandatory** check box.

10. Select **Transfer2** in the **Work class ID** field.

11. Select **New** in the **Work Template Details** area.

12. Select **Put** in the **Work type** field.

13. Select the **Mandatory** check box.

14. Select **Transfer2** in the **Work class ID** field.

15. Select **Save**.

16. Verify that the **Valid** check box on the **Overview** tab is now selected.

### Create transfer receipts

1.  In the **Work order type** field, select **Transfer receipt**.

2.  Select **New** in the Action Pane.

3.  Type **32 TO Receipt** in the **Work template** field.

4.  Type **Transfer Receipt** in the **Work template description** field.

5.  Select **Save**.

6.  Select **New** in the **Work Template Details** area.

7.  Select **Pick** in the **Work type** field.

8.  Select the **Mandatory** check box.

9.  Select **Transfer** in the **Work class ID** field.

10. Select **New** in the **Work Template Details** area.

11. Select **Put** in the **Work type** field.

12. Select the **Mandatory** check box.

13. Select **Transfer** in the **Work class ID** field.

14. Select **Save**.

15. Verify that the **Valid** check box is now selected.

16. Close the pages.

**Set up replenishment**

You have been asked to perform the replenishment setup for Warehouse 30 for
Contoso Orange Juice.

**Set up mobile device menu items and menu**

1.  Open **Warehouse management \> Setup \> Mobile device \> Mobile device menu
    items**.

2.  Select **New**.

3.  Type **Replenishment** in the **Menu item name** field.

4.  Type **Replenishment** in the **Title** field.

5.  Select **Work** in the **Mode** field.

6.  Set the **Use existing work** slider to **Yes**.

7.  Select **New** on the **Work classes** FastTab.

8.  Select a Work class ID from the list.

9.  Close the page.

10. Open **Warehouse management \> Setup \> Mobile device \> Mobile device
    menu** and select the menu where you would like to add replenishment.

11. Select the **Replenishment** menu item from the **Available menus and menu
    items** pane.

12. Select the right directional arrow to move **Replenishment** to the **Menu
    structure** pane.

13. Close the page.

**Set up a work template**

1.  Open **Warehouse management \> Setup \> Work \> Work templates**.

2.  In the **Work order type** field, select **Replenishment**.

3.  Select **New**.

4.  Type **Replenish** the **Work template** field.

5.  Type **Replenish** in the **Work template description** field.

6.  Click **Save**.

7.  Select **New** in the **Work Template Details** section.

8.  Select **Pick** in the **Work type** field.

9.  Select the **Mandatory** check box.

10. Select **Replenish** in the **Work class ID** field. (If it doesn’t exist,
    create it by right clicking and choose view details.)

11. Select **New** in the **Work Template Details** section.

12. Select **Put** in the **Work type** field.

13. Select the **Mandatory** check box.

14. Select **Replenish** in the **Work class ID** field.

15. Close the page.

**Set up a location directive**

1.  Open **Warehouse management \> Setup \> Location directives**.

2.  Select **Replenishment** in the **Work order type** field.

3.  Select **New**.

4.  Type **Replenish** in the **Name** field.

5.  Select **Pick** in the **Work type** field.

6.  Select **3** in the **Site** field.

7.  Select **32** in the **Warehouse** field.

8.  Click **Save**.

9.  Select **New** on the **Lines** FastTab.

10. Verify that the **Sequence number** is **1**.

11. Type **500** in the **To quantity** field.

12. Type **ea** in the **Unit** field.

13. Refresh the screen.

14. Select **New** on the **Location directive actions** FastTab.

15. Type **Replenish** in the **Name** field.

16. Refresh the screen.

17. Select **Edit query**.

18. Select **Add** on the **Query** page.

19. Select **Locations** in the **Table** column.

20. Select **Location profile ID** in the **Field** column.

21. Select **BULK** in the **Criteria** column.

22. Select **OK**.

23. Select **New** in the action pane.

24. Type **Replenish Put** in the **Name** field.

25. Select **Put** in the **Work type** field.

26. Select **3** in the **Site** field.

27. Select **32** in the **Warehouse** field.

28. Click **Save**.

29. Select **New** on the **Lines** FastTab.

30. Verify that the **Sequence number** is **1**.

31. Type **500** in the **To quantity** field.

32. Type **ea** in the **Unit** field.

33. Refresh the screen.

34. Select **New** on the **Location Directive Actions** FastTab.

35. Type **Replenish Put** in the **Name** field.

36. Refresh the screen.

37. Select **Edit query**.

38. Select **Add** on the **Query** page.

39. Select **Locations** in the **Derived table** column.

40. Select **Location profile ID** in the **Field** column.

41. Select **PRODIN** in the **Criteria** column.

42. Select **OK**.

43. Close the **Location directives** page.

**Set up a wave template**

1.  Open **Warehouse management \> Setup \> Waves \> Wave templates**.

2.  Select **Shipping** in the **Wave template type** field.

3.  Select **New**.

4.  Type **30 Replenish** in the **Wave template name** field.

5.  Type **30 Replenish** in the **Wave template description** field.

6.  Select **3** in the **Site** field.

7.  Select **30** in the **Warehouse** field.

8.  Set the **Automate wave creation**, **Process wave at release to
    warehouse**, **Automate wave release**, and **Automate replenishment work
    release** sliders to **Yes**.

9.  Expand the **Methods** FastTab and verify that the **createLoads**,
    **allocateWave**, and **createWork** methods are selected.

10. Select **Replenish** from the **Remaining methods** pane.

11. Select the right directional arrow to move **Replenish** to the **Selected
    methods** pane.

12. Wave step code can be 4.

13. Close the page.

**Set up a replenishment template**

1.  Open **Warehouse management \> Setup \> Replenishment \> Replenishment
    templates**.

2.  Select **New**.

3.  Enter **Rep Demand** in the **Replenish template** field.

4.  Enter **Replenish Demand** in the **Description** field.

5.  In the **Replenishment type** field, select **Wave demand**.

6.  In the **Wave step code** field, enter **200**.

7.  In the **Replenishment template details** section, select **New**.

8.  In the **Sequence number** field, enter **1**.

9.  In the **Description** field, type **Demand**.

10. In the **Replenishment unit** field, type **ea**.

11. In the **Work template** field, select **Replenish**.

12. Refresh the screen.

13. Select **Select products**.

14. On the **Product query** page, enter **P9500** in the **Criteria** field.

15. Click **OK**.

16. Click **Save**.

17. Open **Warehouse management \> Setup \> Waves \> Wave template**.

18. Select **30 Replenish** from the list of wave templates.

19. Select **Edit**.

20. In the **Selected Methods** pane, select the replenish method and enter
    **200** in the **Wave step code** field.

21. Select **Save**.

22. Close the page.

**Run replenishment for a load demand**

You have been asked to run replenishment for a load demand for Contoso Orange
Juice, once a day on every workday for the next six weeks. Set up the recurring
replenishment.

1.  Open **Warehouse management \> Replenishment \> Load demand replenishment**.

2.  On the **Load demand replenishment** page, select **Rep Demand** in the
    **Replenish template** field.

3.  Expand the **Run in the background** FastTab.

4.  Set the **Batch processing** slider to **Yes**.

5.  Select the **Recurrence** tab.

6.  On the **Define recurrence** page, enter today's date in the **Start date**
    field.

7.  In the **Start time** field, enter **7:00 PM**.

8.  Select the **End by** button and enter a date six weeks from today's date.

9.  In the **Recurrence Pattern** area, select the **Days** button.

10. Select the **Every weekday** button.

11. Select **OK**.

12. Select **OK**.

Exercise 5: Perform outbound operations
=======================================

Create an Outbound Location Directive
-------------------------------------

You work for Contoso Orange Juice, and you have been asked to set up an outbound
location directive to ship items sold to a customer.

Create an outbound location directive.
--------------------------------------

1.  Open **Warehouse management \> Setup \> Location directives.**

2.  In the **Work order type** field, select **Sales orders**.

3.  Click **New.**

4.  Enter **30 Pick2** in the **Name** field.

5.  Select **Pick** in the **Work type** field.

6.  Select **3** in the **Site** field.

7.  Select **30** in the **Warehouse** field.

8.  Click **Save** on the action pane.

9.  In the **Lines** FastTab, click **New**.

10. In the **From quantity** field, enter **0**.

11. In the **To quantity** field, enter **9999**.

12. Leave the Unit field blank.

13. Select **None** in the **Locate quantity** field.

14. Click **Save** in the action pane.

15. In the **Location directive actions** FastTab, click **New**.

16. In the **Name** field, enter **Pick**.

17. In the **Fixed location usage** field, select **Fixed and non-fixed
    locations.**

18. Click **Save** on the action pane.

Create an Outbound Work Template
--------------------------------

You work for Contoso Orange Juice, and you have been asked to set up a work
template for a sales order.

Create an outbound work template.
---------------------------------

1.  Open **Warehouse management \> Setup \> Work \> Work templates**.

2.  Select **Sales order** in the **Work template type** field.

3.  Click **New** in the action pane.

4.  Enter **SO Pick** 2 in the **Work template** field.

5.  Enter **SO Pick** 2 in the **Work template description** field.

6.  Click **Save.**

7.  In the **Work Template Details** section, click **New**.

8.  Select **Pick** in the **Work type** field.

9.  Select the **Mandatory** check box.

10. In the **Work class ID** field, select **SO Pick**.

11. In the **Work Template Details** section, click **New** again.

12. Select **Put** in the **Work type** field.

13. Select the **Mandatory** check box.

14. In the **Work class ID** field, select **SO Pick**.

15. Click **Save** in the action pane.

Create a Sales Order and Release it to the Warehouse
----------------------------------------------------

You work for Contoso Orange Juice and you need to create a sales order for four
bottles of grapefruit juice and release it to the warehouse.

Create a sales order.
---------------------

1.  Open **Sales and marketing \> Sales orders \> All sales orders**.

2.  Click the **New** button to create a new sales order.

3.  In the **Customer account** drop-down list, select **US-027**.

4.  Expand the **General** FastTab.

5.  Select **3** in the **Site** drop-down list.

6.  Select **30** in the **Warehouse** drop-down list.

7.  Click **OK**.

8.  In the **Item number** field, select **P9500**.

9.  Enter **4** in the **Quantity** field.

10. Expand the **Line Details** FastTab.

11. Click the **Setup** tab.

12. Select **Manual** in the **Reservation** drop-down list.

13. On the **Sales order lines** FastTab, select **Inventory** \>
    **Reservation**.

14. Enter **4** in the **Reservation** field.

15. Select the **Inventory status** check box.

16. Click **Reserve lot**.

17. Close the Reservation form.

Release the order to the warehouse.
-----------------------------------

1.  Select the **Warehouse** tab on the action pane.

2.  Click **Release to warehouse** in the **Actions** group.

3.  An information bar confirms that the shipment is created (or not).

4.  Close the information bar.

5.  Close the Sales order details form.

Exercise 6: Perform cluster picking
===================================

Create Cluster Profiles
-----------------------

As a warehouse manager for Contoso Orange Juice, you need to create a cluster
profile, create a menu item for Cluster Picking, and then add the menu item to
the mobile device.

Create a cluster profile.
-------------------------

1.  Open **Warehouse management \> Setup \> Mobile device \> Cluster profiles**.

2.  Click **New** in the action pane.

3.  In the **Cluster profile ID** field, enter **Picking Cluster Profile.**

4.  In the **Name** field, enter **Picking Cluster Profile**.

5.  Expand the **General** FastTab.

6.  Set the **Generate cluster ID** slider to **Yes**.

7.  Set the **Activate positions** slider to **Yes**.

8.  Enter **2** in the **Number of positions** field.

9.  Click **Save** in the action pane.

Create the Cluster Picking menu item.
-------------------------------------

1.  Open **Warehouse management \> Setup \> Mobile device \> Mobile device menu
    items**.

2.  Click **New** in the action pane.

3.  Enter **Cluster Picking** in the **Menu item name** field.

4.  Enter **Cluster Picking** in the **Title** field.

5.  Select **Work** in the **Mode** field.

6.  Select the **Use Existing Work** slider to **Yes**.

7.  Select **Cluster picking** in the **Directed by** field.

8.  In the **Cluster profile ID** field, select **Picking Cluster Prof**

9.  Click **New** in the **Work classes** FastTab.

10. Select **Sales** in the **Work class ID** field.

11. Click **New** in the **Work classes** FastTab again.

12. Select **SO Load** in the **Work class ID** field.

13. Click **New** in the **Work classes** FastTab again.

14. Select **SO Pick** in the **Work class ID** field.

15. Click **Save** in the action pane.

Add the menu item to the mobile device.
---------------------------------------

1.  Open **Warehouse management \> Setup \> Mobile device \> Mobile device
    menu**.

2.  Select **Main** in the left-hand pane.

3.  Click **Edit**.

4.  Select **Cluster Picking** from the **Available menus and menu items** pane.

5.  Click the directional arrow to move the selection to the **Menu structure**
    pane.

6.  Click **Save** in the action pane.

Exercise 7: Perform packing and containerization
================================================

Set up Manual Packing
---------------------

You are asked to set up manual packing for Contoso Orange Juice. You need to
create a container type and packing profile. You will then link the packing
profile to Julia Funderburk.

Create container types.
-----------------------

1.  Open **Warehouse management \> Setup \> Containers \> Container types**.

2.  Click **New** in the action pane.

3.  In the **Container type code** field, enter **PackingBox**.

4.  In the **Description** field, enter **PackingBox**.

5.  In the **Tare weight** field, enter **0.5**.

6.  In the **Maximum net weight** field, enter **15.00**.

7.  In the **Container length** field, enter **12.00**.

8.  In the **Container width** field, enter **16.00**.

9.  In the **Container height** field, enter **10.00**.

10. Click **Save** in the action pane.

Create a packing profile.
-------------------------

1.  Open **Warehouse management \> Setup \> Packing \> Packing profiles**.

2.  Click **New** to create a new profile.

3.  Type **PACK2** in the **Packing profile ID** field.

4.  Type **Packing station 2** in the **Description** field.

5.  Select **Number 1** in the **Container packing policy** field, or create it.

6.  Select **Auto** in the **Container ID mode** field.

7.  In the **Container type** field, select **PackingBox**.

8.  Select the **Autocreate container at container close** check box.

9.  Click **Save** in the action pane.

Link the profile to a work user.
--------------------------------

1.  Open **Warehouse management \> Setup \> Worker**.

2.  Select **Julia Funderburk** from the left-hand pane.

3.  Click **Edit** in the action pane.

4.  Update the **Packing profile ID** field to **PACK2**.

5.  Click **Save** in the action pane.

Set up a wave template
----------------------

1.  Go to **Warehouse management \> Setup \> Waves \> Wave templates**.

2.  Click **New**.

3.  In the **Wave template** name field, type a value.

4.  In the **Wave template description** field, type a value.

5.  In the **Site** field, enter or select a value.

6.  In the **Warehouse** field, enter or select a value.

7.  Click **Save**.

8.  Expand the **Methods** section. The Selected methods pane lists the methods
    for the selected wave template type. The wave template must include the
    containerize method.

9.  In the list, find and select the desired record.

10. In the **Wave step code** field, type a value. Enter a Wave step code for
    the added method, which can be any code. It’s possible to add the method
    more than once and assign different wave step codes. To do this, select
    Repeatable for this method in the Wave process methods page.

11. Click **Save**.

12. Close the page.

Enable license plate label printing
-----------------------------------

This procedure enables the automatic printing of a Serial shipping container
code (SSCC) label after the last item is picked from inventory in a sales
picking work process. You can run this procedure in demo data company USMF.

If you’re running it using your own data, you need to have a number sequence set
up for license plates. You need to set up a label printer before you begin this
task. Go to Organization administration \> Setup \> Network printers. On the
Action pane, click Options, and then click the Download document routing agent
installer button. Run the installer and make sure that you have a working
network printer set to Active before you continue with the procedure.

Set up the GS1 company prefix
-----------------------------

1.  Go to **Warehouse management \> Setup \> Warehouse management parameters**.

2.  In the **GS1 company prefix** field, enter the 7 numbers for your GS1
    company number.

3.  Click **Save**.

4.  Close the page.

Setup the SSCC license plate number sequence
--------------------------------------------

1.  Go to **Organization administration \> Number sequences \> Number
    sequences**.

2.  Click **New \> Number sequence**.

3.  For number sequence code, give it a unique number/alpha.

4.  In the **Scope** field, select **Company**.

5.  In the **Company** field, Select **USMF**.

6.  Expand the **Segments** section.

7.  Select the **Company** row

8.  Click **Remove**.

9.  Select the **Constant** row

10. Click **Remove**.

11. Click **Save**.

12. Close the page.

Create the document route layout
--------------------------------

1.  Go to **Warehouse management \> Setup \> Document routing \> Document
    routing layouts.**

2.  Click **New**.

3.  In the **Layout ID** field, type **GTLLayout**.

4.  In the **Description** field, type any value.

5.  In the list, find and select the desired record.

6.  Click **Insert at end of text**.

7.  Click **Save**.

8.  Close the page.

Set up the document routing
---------------------------

1.  Go to **Warehouse management \> Setup \> Document routing \> Document
    routing.**

2.  In the **Work order type** field, select an option (such as Purchase
    orders).

3.  Click **New**.

4.  In the **Warehouse** field, type a 61.

5.  In the **Name** field, type a value.

6.  Click **New** in the Document routing printers fast tab.

7.  In the **Layout ID** field, enter or select **GTLLayout**.

8.  In the **Name** field, enter the printer name that you want to use.

9.  Click **Save**.

10. Close the page.

Create mobile device menu
-------------------------

1.  Go to **Warehouse management \> Setup \> Mobile device \> Mobile device menu
    items.**

2.  Click **New**.

3.  In the **Menu item name** field, type **GTLMnu**.

4.  In the **Title** field, type a value.

5.  In the **Mode** field, select an option.

6.  Select Yes in the **Use existing work** field.

7.  Select Yes in the **Generate license plate** field.

8.  Expand the **Work classes** section.

9.  Click **New**.

10. In the **Work class ID** field, select a value.

11. Click **Save**.

12. Close the page.

13. Go to **Warehouse management \> Setup \> Mobile device \> Mobile device
    menu.**

14. In the list, find and select the desired record.

15. In the tree, select 'In the tree, select **GTLMnu**.

16. Click **Edit**.

17. Click on the arrow to add the menu item to the menu.

18. Click **Save**.

19. Close the page.

Update a work template
----------------------

1.  Go to **Warehouse management \> Setup \> Work \> Work templates.**

2.  In the list, find and select the desired record.

3.  Click **Edit**.

4.  In the work template details, click **New**.

5.  In the **Work type** field, select 'Print'.

6.  In the **Work class ID** field, enter or select a value.

7.  Click **Save**.

8.  Click **Move up**.

9.  Click **Save**.

10. Close the page.
