Exercise 1: Configure Warehouse management Setup
================================================

Create a Storage Dimension Group
--------------------------------

As a warehouse manager in Seahorse Retailers, you have to create a new storage
dimension group to use with Warehouse Management.

Create a new storage dimension group.

1.  Open **Product information management \> Setup \> Dimension and variant
    groups \> Storage dimension groups**.

2.  Click **New** to create a new storage dimension group.

3.  Type **LASD** in the **Name** field.

4.  Type **Los Angeles storage dimension** in the **Description** field.

5.  Enable the **Use warehouse management processes** option to enable Warehouse
    management.

6.  Click **Save** in the action pane and verify that the Site, Warehouse,
    Location, Inventory status, and License plate dimensions are active.

7.  Close the form.

Create a Tracking Dimension Group
---------------------------------

As a warehouse manager in Seahorse Retailers, you have to create a new tracking
dimension group that will not track serial numbers or batch numbers.

Create a new tracking dimension group.

1.  Open **Product information management \> Setup \> Dimension and variant
    groups \> Tracking dimension groups**.

2.  Click **New** to create a new Tracking dimension group.

3.  Type **LANT** in the **Name** field.

4.  Type **Los Angeles no tracking** in the **Description** field.

5.  Select **None** in the **Capture serial** field.

6.  Click **Save.**

7.  Make sure the **Active** check box is not selected for any dimensions.

8.  Close the form.

Create a Unit Sequence Group
----------------------------

As a warehouse manager in Seahorse Retailers, you have to create a new unit
sequence group for each, box, and pallet (EA, BOX, PL), which will have license
plate grouping.

Create a new unit sequence group.

1.  Open **Warehouse management \> Setup \> Warehouse \> Unit sequence groups**.

2.  Click **New** to create a unit sequence group.

3.  Type **EBP** in the **Unit sequence group ID** field.

4.  Type **EachBoxPallet** in the **Name** field.

5.  In the **Unit** field, select **ea**.

6.  Select the **License plate grouping** check box.

7.  Select the **Default unit for purchase and transfer** check box.

8.  Click **New** on the **Line details** FastTab to add a line.

9.  In the **Unit** field, select **Box**.

10. Select the **License plate grouping** check box.

11. Click **New** on the **Line details** FastTab to add a line.

12. In the **Unit** field, select **PL**.

13. Select the **License plate grouping** check box.

14. Click **Save** and close the form.

Create a Warehouse
------------------

As a warehouse manager in Seahorse Retailers, you have to configure a new
warehouse named “MainDC” in Site “1” for use within company USP2.

Create a new warehouse and assign a name and site.

1.  Open **Warehouse management \> Setup \> Warehouse \> Warehouses**.

2.  Click **New** to create a new warehouse.

3.  Type **MAINDC** for the warehouse and Name.

4.  Select Site **1** to relate the warehouse to.

Assign warehouse management attributes.

1.  Expand the **Master planning** FastTab and select the **24hr** Calendar for
    the warehouse.

2.  Expand the **Warehouse** FastTab.

3.  Select the **Use warehouse management processes** check box.

4.  Select the **Allow license plate moves during cycle counting** check box.

5.  Select the **Decrement load line** check box.

6.  Close the forms.

Create Location Types
---------------------

As a warehouse manager in Seahorse Retailers, you have to create new location
types for the warehouse, which you will name “RCV,” “PICKING,” and “FRESH.”

Create three new location types.

1.  Open **Warehouse management \> Setup \> Warehouse \> Location types**.

2.  Click **New** to create a new location type.

3.  Type **PICKING** as the identifier in the **Location type** field.

4.  Type **Picking** in the **Description** field.

5.  Click **New** to create another new location type.

6.  Type **RCV** as the identifier in the **Location type** field.

7.  Type **Receiving** in the **Description** field.

8.  Click **New** to create another new location type.

9.  Type **FRESH** as the identifier in the **Location type** field.

10. Type **Fresh** in the **Description** field.

11. Close the forms.

Create Location Formats
-----------------------

As a warehouse manager in Seahorse Retailers, you have to create a new location
format for Aisle-Rack-Shelf, Aisle-Shelf, and Bay door

Create the new location format.

1.  Open **Warehouse management \> Setup \> Warehouse \> Location formats**.

2.  Click **New** to create a new location format.

3.  Type **ARS** in the **Location format** field.

4.  Type **Aisle – Rack – Shelf** in the **Name** field.

Add segments to the location format.

1.  On the **Details** FastTab, click **New** to create a new line.

2.  In the **Segment description** field, type **Aisle Prefix**.

3.  Type **1** in the **Length** field.

4.  On the **Details** FastTab, click **New** to create a new line.

5.  In the **Segment description** field, type **Aisle Number**.

6.  Type **2** in the **Length** field.

7.  On the **Details** FastTab, click **New** to create a new line.

8.  In the **Segment description** field, type **Rack Number**.

9.  Type **2** in the **Length** field.

10. On the **Details** FastTab, click **New** to create a new line.

11. In the **Segment description** field, type **Shelf Prefix**.

12. Type **1** in the **Length** field.

13. On the **Details** FastTab, click **New** to create a new line.

14. In the **Segment description** field, type **Shelf Number**.

15. Type **2** in the **Length** field.

16. Create another location format.

17. Click **New** at the top to create a new location format.

18. Type **RS** in the **Location format** field.

19. Type **Rack - Shel**f in the Name field.

20. Add segments to the second location format.

21. On the **Details** FastTab, click **New** to create a new line.

22. In the **Segment description** field, type **Rack Prefix**.

23. Type **1** in the **Length** field.

24. On the **Details** FastTab, click **New** to create a new line.

25. In the **Segment description** field, type **Rack Number**.

26. Type **2** in the **Length** field.

27. On the **Details** FastTab, click **New** to create a new line.

28. In the **Segment description** field, type **Shelf Prefix**.

29. Type **1** in the **Length** field.

30. On the **Details** FastTab, click **New** to create a new line.

31. In the **Segment description** field, type **Shelf Number**.

32. Type **2** in the **Length** field.

33. Create a third location format:

34. Click **New** at the top to create a new location format.

35. Type **BaydoorOnly** in the **Location format** field.

36. Type **Baydoor Only** in the **Name** field.

37. Add segments to the third location format.

38. On the **Details** FastTab, click **New** to create a new line.

39. In the **Segment description** field, type **Baydoor Prefix**.

40. Type **1** in the **Length** field.

41. On the **Details** FastTab, click **New** to create a new line.

42. In the **Segment description** field, type **Baydoor Number**.

43. Type **2** in the **Length** field.

44. Close the forms.

Create a Dock Management Profile
--------------------------------

As a warehouse manager in Seahorse Retailers, you have to set up a new dock
management profile.

1.  Open **Warehouse management \> Setup \> Warehouse \> Dock management
    profiles**.

2.  Click **New** to create a dock management profile.

3.  Type **SHIPSTAGE** in the **Dock management profile ID** field.

4.  Type **Staging locations unique per shipment** in the **Description** field.

5.  Select **Shipment ID** in the **Inventory types that should not be mixed**
    field.

6.  Select the **Assume empty location** check box to ensure that the location
    is empty before adding new items to the location.

7.  Close the forms.

Create New Location Profiles
----------------------------

As a warehouse manager in Seahorse Retailers, you have to create new location
profiles for Picking, Staging, Receiving, Bulk, and Fresh.

1.  Open **Warehouse management \> Setup \> Warehouse \> Location profiles**.

2.  Click **New** to create a new Location profile.

3.  In the **Location profile ID**, enter **PICKING.**

4.  In the **Name** field, enter **Picking Locations**.

5.  On the **General** FastTab select **ARS** in the **Location format** field.

6.  On the **General** FastTab select **Picking** from the **Location type**
    field.

7.  Select the **Use license plate tracking** check box.

8.  Select the **Allow mixed items** check box.

9.  Select the **Allow cycle counting** check box.

Create a new location profile for Staging.

1.  Click **New** to create a new Location profile.

2.  In the L**ocation profile ID** enter **STAGING.**

3.  In the **Name** field, enter **Staging locations**.

4.  On the **General** FastTab select **Baydoor** in the **Location format**
    field.

5.  On the **General** FastTab select **Staging STAGE** in the **Location type**
    field.

6.  Select the **Use license plate tracking** check box.

7.  Select the **Allow mixed items** check box.

Create a new location profile for Receiving:

1.  Click **New** to create a new Location profile.

2.  In the **Location profile ID** field, enter **RECEIVING.**

3.  In the **Name** field, enter **Receiving locations**.

4.  On the **General** FastTab select **Baydoor** in the **Location format**
    field.

5.  On the **General** FastTab select **Recv** in the **Location type** field.

6.  Select the **Use license plate tracking** check box.

7.  Select the **Allow mixed items** check box.

Create a new location profile for Bulk:

1.  Click **New** to create a new Location profile.

2.  In the **Location profile ID** field enter **BULKLOCATIONS**.

3.  In the **Name** field, enter **Bulk Locations**.

4.  On the **General** FastTab select **RS** in the **Location format** field.

5.  Select the **Use license plate tracking** check box.

6.  Select the **Allow mixed items** check box.

Create a new location profile for Fresh.

1.  Click **New** to create a new Location profile.

2.  In the **Location profile ID** field, enter **FRESH**.

3.  In the **Name** field, enter **Fresh locations**.

4.  On the **General** FastTab select **ARS** in the **Location format** field.

5.  On the **General** FastTab select **Fresh** from the **Location type**
    field.

6.  Select the **Use license plate tracking** check box.

7.  Select the **Allow mixed items** check box.

8.  Close the forms.

Exercise 2: Configure Reservation hierarchies
=============================================

Create a Reservation Hierarchy
------------------------------

As a member of the Microsoft Dynamics 365 for Finance and Operations project
team for Contoso Orange Juice Company, you need to create a new reservation
hierarchy to help you manage the oranges. The oranges will be tracked using
site, warehouse, location, and batch numbers. Use the information provided to
create a new reservation hierarchy.

Create a reservation hierarchy.
-------------------------------

1.  In **USP2**, Open **Warehouse management** \> **Setup** \> **Inventory** \>
    **Reservation hierarchy**.

2.  Click **New** to create a new reservation hierarchy.

3.  Enter **Oranges** in the **Name** field.

4.  Enter **Orange reservations** in the **Description** field.

Select dimensions for the reservation hierarchy.
------------------------------------------------

1.  In the **Selected** pane, select the **Serial number** check box.

2.  Click the left directional button to move the dimensions to the Available
    pane.

3.  Repeat steps a-b for **Owner.**

4.  Click **OK**.

5.  Close the forms.

Create Products
---------------

As a member of the Microsoft Dynamics 365 for Finance and Operations project
team for Contoso Orange Juice Company, you need to create a new product in
company USP2 called Low Sugar Orange Juice, number B0004. The new item will
track Site, Warehouse, Location, and Batch numbers. The costing for the product
will use the FEFO methodology and the posting will use the standard orange juice
postings. Use the information provided to create a new item.

Create a product.
-----------------

1.  In **USP2**, Open **Product information management \> Products \> Released
    products.**

2.  Click **New** to create a new product.

3.  Enter the following information in the entry fields:

    -   **Product number** – B0004

    -   **Product name** – Low Sugar Orange Juice

    -   **Item model group** – FEFO

    -   **Item group** – OrgJuice

    -   **Storage dimension group** – Ware

    -   **Tracking dimension group** – Batch-Phy

    -   **Reservation hierarchy** – Oranges

4.  Click **OK**.

Configure advanced warehousing settings.
----------------------------------------

1.  Expand the **Warehouse** FastTab on the Released product details form.

2.  Select **GAL** in the **Unit sequence group ID** field.

3.  Click **Validate** in the **Maintain** group of the action pane.

4.  Close the forms.

Exercise 3: Configure Location Directives and Disposition codes
===============================================================

Create Disposition Codes
------------------------

You are asked to set up two new Disposition codes. The first will be called
“Ready,” which will be Available, and the second will be called “Not Ready,”
which will be blocked for use with Warehouse management.

Create two new disposition codes.
---------------------------------

1.  In USP2, Open **Warehouse management \> Setup \> Mobile device \>
    Disposition codes**.

2.  Click **New** to create a disposition code.

3.  In the **Disposition code** field, enter **Ready**.

4.  In the **Inventory status** field, select **Available**.

5.  Click **New** to create a disposition code.

6.  In the **Disposition code** field, enter **Not Ready**.

7.  In the **Inventory status** field, select **Blocked**.

8.  Close the forms.

Notes:

-   In the Work template code field, you can select a work template code that is
    associated with a work order type, return order, or purchase order. You
    assign a work template to a disposition code only when you want to override
    the work template.

-   In the Return disposition code field, you can select a return disposition
    code for a sales return order. After you select a return disposition code,
    the disposition code is only applicable for the sales order return process.

Create Inbound Location Directives
----------------------------------

You have to configure a new inbound location directive that will receive goods
to the warehouse and then one that will put away goods in bulk locations.

Create a new Purchase order put location directive.
---------------------------------------------------

1.  Open **Warehouse management \> Setup \> Location directives**.

2.  Select **Purchase orders** in the **Work order type** field.

3.  Click **New** in the action pane to create a new location directive.

4.  Type **MAIN DC** in the **Name** field.

5.  Select **Put** in the Work type field. This is because we want to put the
    received items on purchase orders away.

6.  Select **3** in the **Site** field.

7.  Select **30** in the **Warehouse** field.

8.  Select **Stage** in the **Directive code** field.

9.  Click **Save**.

Add lines to the location directive.
------------------------------------

1.  Click **New** in the **Lines** FastTab.

2.  Verify the Sequence number is 1.

3.  Type **200** in the **To quantity** field.

4.  Type **ea** in the **Unit** field.

5.  Select **None** in the **Locate quantity** field.

6.  Click **Save** in the action pane.

7.  Click **New** in the **Location directive actions** FastTab.

8.  Type **Fresh** in the **Name** field.

9.  Click **Save** in the action pane.

Add location directive actions to the location directive.
---------------------------------------------------------

1.  Click **Edit query** in the action pane.

2.  Click **Add** on the Query form.

3.  Select **Purchase Orders** in the **Table** column.

4.  Select **Location** in the **Field** column.

5.  Select **30** in the **Criteria** column.

6.  Click **OK**.

7.  Close the Location directives form.
