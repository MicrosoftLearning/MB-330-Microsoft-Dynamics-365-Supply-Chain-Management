---
lab:
    title: 'Case study 3 Warehouse management and transportation management'
    module: 'Module 4: Implement warehouse management and transportation management '
---
Case study 3 Warehouse management and transportation management
===============================================================

Objectives
----------

1.  Configure warehouse management

2.  Perform warehouse management processes

3.  Implement transportation management

Exercise \#1 Configure warehouse management
-------------------------------------------

*Objective: Create and define the components of warehouse management and
configure inventory statuses using unit sequence groups and reservation
hierarchies.*

You were asked to help the warehouse manager for SRHQ Seahorse Retailers. He is
responsible for building and designing the structure for the warehouse
management system.

You will need to guide him on performing some setup and configuration activities
before being able to use the warehouse management systems.

-   Configure warehouse management setup.

-   Create a storage dimension group.

-   Create a tracking dimension group.

-   Create a unit sequence group.

-   Create a warehouse.

-   Create location types.

-   Create location formats.

-   Create a dock management profile.

-   Create new location profiles.

### Create a Storage Dimension Group

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

### Create a Tracking Dimension Group

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

### Create a Unit Sequence Group

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

### Create a Warehouse

As a warehouse manager in Seahorse Retailers, you have to configure a new
warehouse named “MainDC” in Site “1” for use within company USP2.

Create a new warehouse and assign a name and site.

1.  Open **Warehouse management \> Setup \> Warehouse \> Warehouses**.

2.  Click **New** to create a new warehouse.

3.  Type **MAINDC** for the warehouse and Name.

4.  Select Site **1** to relate the warehouse to.

### Assign warehouse management attributes.

1.  Expand the **Master planning** FastTab and select the **24hr** Calendar for
    the warehouse.

2.  Expand the **Warehouse** FastTab.

3.  Select the **Use warehouse management processes** check box.

4.  Select the **Allow license plate moves during cycle counting** check box.

5.  Select the **Decrement load line** check box.

6.  Close the forms.

### Create Location Types

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

### Create Location Formats

As a warehouse manager in Seahorse Retailers, you have to create a new location
format for Aisle-Rack-Shelf, Aisle-Shelf, and Bay door

### Create the new location format.

1.  Open **Warehouse management \> Setup \> Warehouse \> Location formats**.

2.  Click **New** to create a new location format.

3.  Type **ARS** in the **Location format** field.

4.  Type **Aisle – Rack – Shelf** in the **Name** field.

### Add segments to the location format

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

19. Type **Rack - Shelf** in the Name field.

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

### Create a Dock Management Profile

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

### Create New Location Profiles

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

### Create a new location profile for Staging

1.  Click **New** to create a new Location profile.

2.  In the **Location profile ID** enter **STAGING.**

3.  In the **Name** field, enter **Staging locations**.

4.  On the **General** FastTab select **Baydoor** in the **Location format**
    field.

5.  On the **General** FastTab select **Staging STAGE** in the **Location type**
    field.

6.  Select the **Use license plate tracking** check box.

7.  Select the **Allow mixed items** check box.

### Create a new location profile for Receiving:

1.  Click **New** to create a new Location profile.

2.  In the **Location profile ID** field, enter **RECEIVING.**

3.  In the **Name** field, enter **Receiving locations**.

4.  On the **General** FastTab select **Baydoor** in the **Location format**
    field.

5.  On the **General** FastTab select **Recv** in the **Location type** field.

6.  Select the **Use license plate tracking** check box.

7.  Select the **Allow mixed items** check box.

### Create a new location profile for Bulk:

1.  Click **New** to create a new Location profile.

2.  In the **Location profile ID** field enter **BULKLOCATIONS**.

3.  In the **Name** field, enter **Bulk Locations**.

4.  On the **General** FastTab select **RS** in the **Location format** field.

5.  Select the **Use license plate tracking** check box.

6.  Select the **Allow mixed items** check box.

### Create a new location profile for Fresh

1.  Click **New** to create a new Location profile.

2.  In the **Location profile ID** field, enter **FRESH**.

3.  In the **Name** field, enter **Fresh locations**.

4.  On the **General** FastTab select **ARS** in the **Location format** field.

5.  On the **General** FastTab select **Fresh** from the **Location type**
    field.

6.  Select the **Use license plate tracking** check box.

7.  Select the **Allow mixed items** check box.

8.  Close the forms.

Exercise \#2 Create a reservation hierarchy (Bonus)
---------------------------------------------------

*Objective: Create a reservation hierarchy and use it to manage a product.*

A warehouse manager at SRHQ requested to be a member of the Microsoft Dynamics
365 for Finance and Supply chain project team for Contoso Orange Juice Company,
one of Seahorse Retailers sister companies.

He wants to create a new reservation hierarchy to manage the oranges.

The oranges will be tracked using site, warehouse, location, and batch numbers.

He is not sure how to create the new reservation hierarchy and to create a new
product that uses the new hierarchy.

### Create a reservation hierarchy.

1.  In **USP2**, Open **Warehouse management** \> **Setup** \> **Inventory** \>
    **Reservation hierarchy**.

2.  Click **New** to create a new reservation hierarchy.

3.  Enter **Oranges** in the **Name** field.

4.  Enter **Orange reservations** in the **Description** field.

### Select dimensions for the reservation hierarchy.

1.  In the **Selected** pane, select the **Serial number** check box.

2.  Click the left directional button to move the dimensions to the Available
    pane.

3.  Repeat steps a-b for **Owner.**

4.  Click **OK**.

5.  Close the forms.

### Create a new product and link it to the new reservation hierarchy

As a member of the Microsoft Dynamics 365 for Finance and Operations project
team for Contoso Orange Juice Company, you need to create a new product in
company USP2 called Low Sugar Orange Juice, number B0004. The new item will
track Site, Warehouse, Location, and Batch numbers. The costing for the product
will use the FEFO methodology and the posting will use the standard orange juice
postings. Use the information provided to create a new item.

### Create a product.

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

### Configure advanced warehousing settings.

1.  Expand the **Warehouse** FastTab on the Released product details form.

2.  Select **GAL** in the **Unit sequence group ID** field.

3.  Click **Validate** in the **Maintain** group of the action pane.

4.  Close the forms.

Exercise \#3 Create disposition codes and inbound location directives
---------------------------------------------------------------------

*Objective: Create and use disposition codes and inbound location directives.*

You have been assigned to assist one of the sister company’s USP2 teams in the
setup and implementation of a warehouse management system.

You must set up two new **disposition codes**. The first will be called “Ready,”
which will be Available, and the second will be called “Not Ready,” which will
be blocked for use with warehouse management. Next, you will configure a new
inbound location directive that will receive goods to the warehouse, and another
one that will put away goods in bulk locations.

You will need to do the following:

-   Create new disposition codes.

-   Create an inbound location directive.

### Create disposition codes

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

### Create an inbound location directive

*Create a new purchase order put location directive*

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

### Add lines to the location directive

1.  Click **New** in the **Lines** FastTab.

2.  Verify the Sequence number is 1.

3.  Type **200** in the **To quantity** field.

4.  Type **ea** in the **Unit** field.

5.  Select **None** in the **Locate quantity** field.

6.  Click **Save** in the action pane.

7.  Click **New** in the **Location directive actions** FastTab.

8.  Type **Fresh** in the **Name** field.

9.  Click **Save** in the action pane.

### Add location directive actions to the location directive.

1.  Click **Edit query** in the action pane.

2.  Click **Add** on the Query form.

3.  Select **Purchase Orders** in the **Table** column.

4.  Select **Location** in the **Field** column.

5.  Select **30** in the **Criteria** column.

6.  Click **OK**.

7.  Close the Location directives form.

Exercise \#4 Configure mobile devices
-------------------------------------

*Objective: Configure mobile devices for warehouse workers.*

You must configure the mobile device menus that the warehouse workers will view
and use during their day to day activities. You are assisting in the setup of
the menus for the mobile devices for companies **USMF** and **SRHQ**.

You will need to do the following:

-   Configure the mobile devices.

-   Create a mobile device menu item and menu.

-   Create mobile device users.

-   Set up a mobile device menu item for completing work of type Purchase order.

### Configure mobile devices

In preparation for setting up the mobile device for your warehouse, you are
asked to first set up a work class, which you will name Purch-Orders. It will
have the put location types of Bay-door, Bulk, and Pick. 

### Add a work class

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

### Create a mobile device menu item and menu

You will be setting up two functions: Purchase order receive and Purchase order
put away. You will then add them to your mobile device menu.

### Set up mobile device menu items

1.  Open **Warehouse management \> Setup \> Mobile device \> Mobile device menu
    items**.

2.  Click on **New.**

3.  For **Menu item name**, enter **PO Receive.**

4.  For **Title**, enter **PO Receive.**

5.  For **Mode**, select **Work.**

6.  Set the **Use existing work** slider to **No**.

7.  On the **General** FastTab, on **Work creation process**, select **Purchase
    order line receiving.**

8.  Set the **License plate grouping policy option** to **License plate
    grouping**.

9.  Set the **Generate license plate** slider to **Yes.**

10. Set all other sliders to No.

11. Click **Save** in the action pane.

12. Click **New** in the action pane.

13. For **Menu item name**, enter **PO Putaway.**

14. For **Title**, enter **PO Putaway.**

15. For **Mode**, select **Work.**

16. Set the **Use existing work** slider to **Yes**.

17. On the **General** FastTab, for Directed by, select User grouping.

18. Set the **Group put away** slider to Yes.

19. Set all remaining sliders to **No**.

20. On **Work classes** FastTab, click **New.**

21. For **Work class ID**, select **P-Orders.**

22. Click **Save** in the action pane.

23. Close the page.

### Set up a mobile device menu

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

### Set up a mobile device menu item for completing work of type Purchase order

Create a menu item that is used for performing work of type Purchase order. The
work class that is associated with the menu item determines which work is valid.

### Create a mobile device menu item

1.  **Go** to **Warehouse management \> Setup \> Mobile device \> Mobile device
    menu items.**

2.  Click **New**.

3.  In the **Menu item name** field, enter a unique value. For example, you
    could type POMove. Remember the value; you'll need it later.

4.  In the **Title** field, type PO Move. This is the title which will be
    displayed on the mobile device.

5.  In the **Mode** field, select 'Work'.

6.  Select **Yes** in the **Use existing work** field.

7.  The **Display inventory status** field determines whether the inventory
    status of the on-hand inventory will be displayed to the warehouse worker on
    the mobile device. Select **Yes**.

8.  In the **Directed by** field, select **System grouping**. When you select
    something in the **Directed by** field, additional fields appear in the
    **General** section on this page. The fields that appear depend on what you
    selected. When you select **System grouping**, two new fields are added.

9.  In the **System grouping** field, select **WorkPoolId**. When warehouse
    workers open this menu item, they’ll be asked to scan a work pool ID. All
    work orders with this work pool ID and open work order lines with one of the
    work classes added to this menu item will be pushed to the user.

10. In the **System grouping label** field, type **Work pool**. This is the text
    displayed to the user on the mobile device.

11. Select **Yes** in the **Override license plate during put** field. This
    option allows warehouse workers to override the target license plate when
    items are put down on a license plate-controlled location.

12. Select **Yes** in the **Group put away** field. If all the Put lines on the
    work order share the same location, the user will receive one combined Put
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
    asked to perform a confirmation scan of the location when the item is put
    down.

7.  Click **Save**.

8.  Close the work confirmation page.

9.  Close the Mobile menu item page.

### Add the menu item to a mobile device menu

1.  Go to the **Mobile device** menu.

2.  Click **Edit**.

3.  Use the Quick Filter to find records. For example, filter on the Name field
    with a value of 'inbound'. You want to find the menu you use for inbound
    menu items. In **USMF** this is called Inbound.

4.  In the tree, select 'a value' POMove.

5.  Click on the arrow that points to the right.

6.  Click **Save**.

7.  Close the mobile device menu page.

Exercise \#5 Configure purchase orders
--------------------------------------

Exercise \#5 Configure purchase orders

*Objective: Create and process a purchase order.*

The warehouse manager for USMF wants to process a purchase order receipt using a
mobile device.

He ordered 10 Pcs of HDMI 6’ Cables.

These will be from Vendor US-111 and shipped to Warehouse 11.

The unit price will be \$20 per Piece.

He is not sure how to record this and asked you to help.

You will need to do the following:

-   Create a purchase order.

-   Create a purchase order receipt using the mobile device.

Create a purchase order

1.  In **USP2,** Navigate to **Accounts payable \> Purchase orders \> All
    purchase orders.**

2.  Click **New** in the action pane.

-   Select **Vendor US-112**.

-   On the **General** FastTab, enter storage dimensions of Site **3** and
    Warehouse **30**.

-   Click **OK**.

1.  On the **Purchase order lines** FastTab, select **Item number P9500**.

*Note*

*You will get a message that the vendor is not authorized for this product. This
is a warning only. You may continue after closing the message.*

-   Enter a **Quantity** of **1**.

-   Enter a **Unit price** of **2.50**.

-   Expand the **Line details** fast tab.

-   Select the **Financial dimensions** tab.

-   In the **Financial dimensions**, the **Product Group** field, select **OJ
    B2B**.

1.  Under **Purchase Tab** in Action Pane. In the **Actions** group,
    select **Confirm** and note your purchase order number.

2.  Note your purchase order number.

3.  Close the form.

4.  Navigate to **Warehourse Management \> Setup \> Worker.**

5.  Click on **New.**

    1.  Select **Ted Howard** under **Worker**

    2.  Click on **New** User ID under **Users** fast Tab. Enter **toward**
        under **User ID** and **User name.**

    3.  **Default Warehouse – 30**

    4.  **Menu name – Main**

    5.  Click on **Save.**

6.  Set the **Password – 12345, Confirm Password – 12345.** Click on **Set
    Password.**

7.  Close the Page.

Create a purchase order receipt using the mobile device

**Create a purchase order receipt by using the mobile device - Prerequisite**

*To practice using the mobile device, you must enable a mobile device emulator
in the Virtual machine. You may need to expand the right bar in the lab
environment to see all content in the instructions. Perform the following
steps.*

1.  Right-click on the tab of your normal system default dashboard and
    select **Duplicate tab**.

2.  The URL on your new tab will be:
    <https://usnconeboxax1aos.cloud.onebox.dynamics.com/?cmp=USP2&mi=defaultdashboard>

3.  Delete all characters on the new tab after dynamics.com (i.e. delete
    /?cmp=USP2&mi=defaultdashboard)

4.  Replace those characters with **/?mi=action%3awhsWorkExecute&cmp=USP2**

**Sign into the Mobile Emulator**

1.  The emulator will now launch, and you can sign in to the mobile device
    emulator.

2.  Log in to the mobile device with the user you have enabled.

3.  Click **Inbound**.

4.  Click **Purchase receive**.

5.  Enter the purchase order number in the **PONUM** field. Click on **OK**.

6.  Enter Item number **P9500**. Click on **OK**.

7.  Enter a quantity of **1** in the **Qty** field. Click **OK** Twice.

8.  Enter LP number **LP951**. Select **OK**

9.  Enter **today’s date** as the vendor batch date. Click **OK**.

-   Enter a date six months from the current date as the Expiry date. Click
    **OK.**

-   Select the **Use as expiration date** arrow. Select **No** and select
    **OK**.

-   For **Country/Region of Origin 1**, enter **USA**. Select **OK.**

1.  Select the green check mark again to bypass the second Country/region entry.

2.  Note the work completed notification.


Exercise \#6 Configure wave processing (Bonus)
----------------------------------------------

*Objective: Set up templates and queries that specify how waves should be
processed.*

You want to configure wave processing by setting up the criteria that determine
what work is generated for a warehouse when a wave is processed, and whether
waves are processed manually or automatically.

You will specify the criteria by setting up wave templates and queries that
match a wave with released lines in sales orders, production orders, or kanban
orders.

When you set up a wave template, you specify the sequence in which the templates
will be matched to released lines on sales orders, production orders, or kanban.

When a line is released to the warehouse or to production, it uses the first
wave template that it meets the criteria for.

Its recommended that you put templates with the most specific criteria at the
top of the list. The broader the criteria, the more likely it is for a line to
meet the criteria, and this could lead to lines being assigned to the wrong
wave. You will set up the wave templates for **USMF**.

You will need to do the following:

Configure wave processing.

### Configure wave processing

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

9.  Set the **Automate wave release** option to **Yes**. Select this option to
    automatically release the wave. The picking work is created and made
    available on mobile devices.

10. Set the **Assign to open waves** option to **Yes**. Lines are assigned to
    waves based on the query filter for the wave template.

11. Set the **Process wave automatically at threshold** option to **Yes**.
    Select this option to automatically process the wave when its values reach
    the thresholds for weight, shipment, and lines specified in the **Wave
    thresholds** field group. This option is available only if **Shipping** is
    selected in the **Wave template type** field.

12. Set the **Automate replenishment work release** option to **Yes**. Select
    this option to create demand-based replenishment work and release it
    automatically. You must add the replenishment wave method to the wave
    template and create a replenishment template of the type **Wave demand**.

13. Expand the **Methods** section. Wave template methods allow you to control
    the sequence of activities that each wave is going through when it is
    processed. For example, you might have a method for wave replenishment. When
    you add a method, it is automatically listed in the appropriate location in
    the sequence of steps. If you have set the **Automate replenishment work
    release** option to **Yes**, you need to add the replenish method here. Wave
    attributes act as filters, to restrict the kind of items that can use the
    wave. For example, you could specify an item group.

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

Exercise \#7 Configure cycle counting (Bonus)
---------------------------------------------

*Objective: Set up cycle counting and add a cycle count to the mobile device.*

To be able to create cycle counting for **USP2**, you need to set up a cycle
count for the mobile device.

You will need to do the following:

-   Set up the cycle counting adjustment type.

-   Set up warehouse parameters for cycle counting.

-   Set up a spot cycle counting menu item.

-   Add the spot count menu item to the mobile device menu.

### Set up a cycle counting adjustment type

1.  In USP2, open **Warehouse management \> Setup \> Inventory \> Adjustment
    types**.

2.  Click **New** on the action pane.

3.  In the **Inventory adjustment type** field, enter **New Cycle Count**.

4.  In the **Description** field, enter **New Cycle Count.**

5.  In the **Name** field, select **Counting**

6.  Select the **Remove reservations** check box.

### Set up warehouse management parameters for cycle counting

1.  Open **Warehouse management \> Setup \> Warehouse management parameters**.

2.  Click the **Cycle counting** tab on the left pane.

3.  In the **Default cycle counting adjustment type code** field, select **New
    Cycle Count**.

4.  In the **Default cycle count work class ID** field, make a selection.

5.  In the **Default cycle count work priority** field, enter **1**.

### Set up a spot cycle counting menu item

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

### Add the spot count menu item to the mobile device menu

1.  Open **Warehouse management \> Setup \> Mobile device \> Mobile device
    menu**.

2.  Select **Inbound** in the left-hand pane.

3.  Click **Edit** in the action pane.

4.  In the **Mobile device menus** section, select **Spot Cycle Count** from the
    **Available menus and menu items** list.

5.  Click the right directional arrow to add the menu item to the **Menu
    structure** list.

6.  Click **Save** in the action pane.

Exercise \#8 Define cycle counting (Bonus)
------------------------------------------

*Objective: Define cycle counting parameters for mobile devices.*

Cycle counting is a warehouse process that you can use to audit on-hand
inventory items. Typically, This task is performed by a warehouse manager. You
will go through this procedure for the **USMF** company to do the cycle counting
setups as well.

You will need to do the following:

-   Set the priority of counting work.

-   Enable the mobile device.

-   Create a counting threshold.

-   Create a cycle count plan.

### Set the priority of counting work

1.  Go to **Warehouse management \> Setup \> Warehouse management parameters**.

2.  Click the **Cycle counting** tab.

3.  In the **Default cycle count work priority** field, enter a number. This
    step changes the priority of cycle counting work compared to other types of
    work in the warehouse. By entering a number that is lower than the number
    for other types of work, you raise the priority of the cycle counting work.

4.  Click **Save**.

5.  Close the page.

### Enable the mobile device

1.  Go to **Warehouse management \> Setup \> Mobile device \> Mobile device menu
    items**.

2.  Click **New**.

3.  In the **Menu item name** field, type a value.

4.  In the **Title** field, type a value.

5.  In the **Mode** field, select **Work**.

6.  Set the **Use existing work** option to **Yes**. When you set this option to
    Yes, the system will look for existing work when the mobile device menu item
    is used.

7.  In the **Directed by** field, select 'System directed'. When "System
    directed" is selected, the warehouse worker will be directed to open work
    that is in defined work classes. (You will create these work classes next.)

8.  Expand or collapse the **Work classes** section.

Next, you will create two work classes that will be used with this mobile device
menu item. When the menu item is used, these work classes will be queried, and
the work that has the highest priority will be shown to the user.

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

### Create a counting threshold

1.  Go to **Warehouse management \> Setup \> Cycle counting \> Cycle count
    thresholds**.

2.  Click **New**.

3.  In the **Cycle counting threshold ID** field, type a value.

4.  Set the **Process cycle counting immediately** option to **Yes**.

5.  In the **Description** field, type a value.

6.  Click **Save**.

7.  Click **Select locations**.

8.  In the **Criteria** field, select a value.

9.  Click **OK**.

10. Close the page.

### Create a cycle count plan

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

Exercise \#9 Define a partial location cycle counting process (Bonus)
---------------------------------------------------------------------

*Objective: Create a work pool, cycle counting work template, and cycle counting
plan.*

When you use cycle count plans to create counting work, you can guide the actual
counting operations by requesting that only specific products and product
variants be counted instead of all on-hand inventory at the location.

By filtering on specific products, the warehouse manager can reduce review
overhead, help prevent consolidation mistakes, and save time.

Typically, a warehouse manager performs the setup tasks. You will perform this
procedure for the **USMF** company.

You will need to do the following:

-   Create a work pool.

-   Create a cycle counting work template.

-   Create a cycle counting plan.

### Create a work pool

1.  In USP2, Go to **Warehouse Management \> Setup \> Work \> Work pools**.

2.  Click **New**.

3.  For Work Pool ID, enter **WP001.**

4.  For description, enter **Work pool 001.**

5.  Click **Save**.

###  Create a cycle counting work template

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

### Create a cycle counting plan

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

Exercise \#10 Transfer orders and replenishments

*Objective: Set up a warehouse, create a location directive, and create work
templates.*

As a functional consultant assisting the warehouse manager assisting during the
implementation for **USP2**, you have been asked to perform setup for transfer
orders.

You will need to do the following:

-   Create and link transit and production warehouses.

-   Set up a location directive.

-   Set up work classes.

-   Create transfer issues.

-   Create transfer receipts.

### Create transit and production warehouses 

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

### Set up a location directive

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

32. Select **New** in the action pane.

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

### Setup Work classes

1.  Open **Warehouse management \> Setup \> Work \> Work classes**.

2.  Click **New**.

3.  In the **Work** class ID field, type **'Transfer2'**.

4.  In the Description field, type **'Transfer'**.

5.  In the Work order type field, select **'Transfer issue'**.

6.  Click **Save**.

7.  Close the page.

### Set up a work template

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

Exercise \#11 Setup replenishment (Bonus)
-----------------------------------------

*Objective: Configure replenishment to run once a day every workday for the next
six weeks.*

you have been asked to perform the replenishment setup for Warehouse 30. under
**USP2** company.

You will need to do the following:

-   Set up mobile device menu items and menu.

-   Set up a work template for replenishment.

-   Set up a location directive for replenishment.

-   Set up a wave template.

-   Set up a replenishment template.

-   Run replenishment for a load demand.

### Set up mobile device menu items and menu

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

### Set up a work template

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

### Set up a location directive

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

### Set up a wave template

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

### Set up a replenishment template

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

### Run replenishment for a load demand

1.  You have been asked to run replenishment for a load demand for Contoso
    Orange Juice, once a day on every workday for the next six weeks. Set up the
    recurring replenishment.

2.  Open **Warehouse management \> Replenishment \> Load demand replenishment**.

3.  On the **Load demand replenishment** page, select **Rep Demand** in the
    **Replenish template** field.

4.  Expand the **Run in the background** FastTab.

5.  Set the **Batch processing** slider to **Yes**.

6.  Select the **Recurrence** tab.

7.  On the **Define recurrence** page, enter today's date in the **Start date**
    field.

8.  In the **Start time** field, enter **7:00 PM**.

9.  Select the **End by** button and enter a date six weeks from today's date.

10. In the **Recurrence Pattern** area, select the **Days** button.

11. Select the **Every weekday** button.

12. Select **OK**.

13. Select **OK**.

Exercise \#12 Configure outbound processing
-------------------------------------------

*Objective: Create an outbound location directive and a work template.*

you have been asked to help with the outbound processing setups for sales order.

To test the setups, you will create a sales order and release to the warehouse
for shipping.

You will need to do the following:

-   Create an outbound location directive to ship items sold to a customer.

-   Create an outbound work template.

-   Create a sales order and release it to the warehouse.

### Create an outbound location directive

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

### Create an Outbound Work Template

Set up a work template for a sales order.

### Create an outbound work template.

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

### Create a Sales Order and Release it to the Warehouse

You must create a sales order for four bottles of grapefruit juice and release
it to the warehouse.

### Create a sales order

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

17. Close the reservation form.

### Release the order to the warehouse.

1.  Select the **Warehouse** tab on the action pane.

2.  Click **Release to warehouse** in the **Actions** group.

3.  An information bar confirms that the shipment is created (or not).

4.  Close the information bar.

5.  Close the Sales order details form.

Exercise \#13 Configure cluster picking
---------------------------------------

*Objective:* enable mobile devices to group picking into clusters

You were asked to setup cluster picking to enable workers to use their mobile
devices to group picking work into clusters.

This will allow them to pick items from a single location for multiple work
orders at the same time.

This should be enabled for **USP2**

You will need to do the following:

-   Create a cluster profile.

-   Create the cluster picking menu item.

-   Add the menu item to the mobile device.

### Create a cluster profile

1.  Open **Warehouse management \> Setup \> Mobile device \> Cluster profiles**.

2.  Click **New** in the action pane.

3.  In the **Cluster profile ID** field, enter **Picking Cluster Profile.**

4.  In the **Name** field, enter **Picking Cluster Profile**.

5.  Expand the **General** FastTab.

6.  Set the **Generate cluster ID** slider to **Yes**.

7.  Set the **Activate positions** slider to **Yes**.

8.  Enter **2** in the **Number of positions** field.

9.  Click **Save** in the action pane.

### Create the Cluster Picking menu item

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

### Add the menu item to the mobile device

1.  Open **Warehouse management \> Setup \> Mobile device \> Mobile device
    menu**.

2.  Select **Main** in the left-hand pane.

3.  Click **Edit**.

4.  Select **Cluster Picking** from the **Available menus and menu items** pane.

5.  Click the directional arrow to move the selection to the **Menu structure**
    pane.

6.  Click **Save** in the action pane.

Exercise \#14 Setup manual packing (Bonus)
------------------------------------------

*Objective: Set up manual packing by configuring packing types, packing
profiles, and wave templates.*

You have been asked to set up manual packing for **USP2**.

You need to create a container type and packing profile.

You will then link the packing profile to Julia Funderburk.

You will need to do the following:

-   Create container types.

-   Create a packaging profile.

-   Link the profile to a work user.

-   Set up a wave template.

### Create container types

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

### Create a packing profile

1.  Open **Warehouse management \> Setup \> Packing \> Packing profiles**.

2.  Click **New** to create a new profile.

3.  Type **PACK2** in the **Packing profile ID** field.

4.  Type **Packing station 2** in the **Description** field.

5.  Select **Number 1** in the **Container packing policy** field, or create it.

6.  Select **Auto** in the **Container ID mode** field.

7.  In the **Container type** field, select **PackingBox**.

8.  Select the **Autocreate container at container close** check box.

9.  Click **Save** in the action pane.

### Link the profile to a work user

1.  Open **Warehouse management \> Setup \> Worker**.

2.  Select **Julia Funderburk** from the left-hand pane.

3.  Click **Edit** in the action pane.

4.  Update the **Packing profile ID** field to **PACK2**.

5.  Click **Save** in the action pane.

### Set up a wave template

1.  Go to **Warehouse management \> Setup \> Waves \> Wave templates**.

2.  Click **New**.

3.  In the **Wave template** name field, type a value.

4.  In the **Wave template description** field, type a value.

5.  In the **Site** field, enter or select a value.

6.  In the **Warehouse** field, enter or select a value.

7.  Click **Save**.

8.  Expand the **Methods** section. The **Selected methods** pane lists the
    methods for the selected wave template type. The wave template must include
    the containerize method.

9.  In the list, find and select the desired record.

10. In the **Wave step code** field, type a value. Enter a Wave step code for
    the added method, which can be any code. It’s possible to add the method
    more than once and assign different wave step codes. To do this, select
    **Repeatable** for this method in the **Wave process methods** page.

11. Click **Save**.

12. Close the page.

Exercise \#15 Configure carriers
--------------------------------

*Objective: Set up a new carrier and add a carrier service.*

**USMF** in the United States has a new customer located in Europe.

The Transportation coordinator at Contoso Entertainment, has determined that a
new company will be used for transporting the products to this customer.

You will need to do the following:

-   Set up a new ocean carrier.

-   Add a carrier service to the carrier.

### Set up a new carrier

1. In USMF, Open **Transportation management** \> **Setup** \> **Carriers** \> **Shipping
carriers**.  

2.  In the action pane, click **New** to create a new shipping carrier.  

3.  In the **Shipping carrier** field, type **Ocean Carrier 2**. 

4.  In the **Name** field, type **Secondary ocean carrier**. 

5.  In the **Mode** field, select **Ocean**.  

6.  Expand the **Overview** FastTab.   

7.  Set the **Activate shipping carrier** slider to **Yes**. 

8.  Select vendor account **1002** from the **Vendor** drop-down menu.  

9.  In the **SCAC** field, type **2005.** 

10.  Set the **Activate carrier rating** slider to **Yes.** 

11. On the **Addresses** FastTab, click **New**. 

12. In the **New address** form, type **Ocean carrier location** in the **Name**
    field. 

13. Select **Business** from the **Purpose** drop-down list. 

14. Select USA in the Country/region drop-down list. 

15. In the **ZIP/postal code** field, type **11251**. 

16. In the **Street** field, type **1577 Madison Blvd**. 

17. Set the **Primary** slider to **Yes**. 

18. Click **OK.** 

19. Close the **Shipping carriers** form. 

### Add a carrier service to the carrier

1.  Open **Transportation management \> Setup \> Carriers \> Shipping
    carriers.** 

2.  Select **Ocean Carrier 2** in the left-hand pane. 

3.  Expand the **Services** FastTab. 

4.  Click **New.** 

5.  In the **Carrier service** field, type **Ocean**.  

6.  In the **Name** field, type **Ocean**. 

7.  In the **Transportation method** field, select **Ocean**. 

8.  Select **Freight** from the **Billing group ID** drop-down menu. 

9.  Close the form. 

Exercise \#16 Configure rate masters
------------------------------------

*Objective: Configure a rate master and base.*

To support the logistics & transportation manager for **USMF**, you were asked
to record the rates for an air carrier.

This is done by setting up the rate masters according to the contracts signed
with the carriers

You will need to do the following:

-   Setup the rate master.

-   Set up the rate base.

-   Assign the rate base.

### Set up rate master

1.  Go to **Transportation management \> Setup \> Rating \> Rate master.**

2.  Click **New**.

3.  In the Rate master field, type **AtlantaMaster**.

4.  In the Name field, type **Atlanta rate master**.

5.  In the Rating metadata ID field, click the drop-down button to open the
    lookup.

    -   The rating metadata ID will determine the data needed for the rate
        master, as it defines the metadata expected by the TMS engine using this
        rate master.

6.  For this example, select the **P2P** option.

7.  Click Save.

### Set up rate base

1.  Click **Rate base**.

    -   The rate base determines the rate of the carrier and can be used to set
        up a tariff structure as it structures the rates in the breakpoints
        defined in the break master.

2.  Click **New**.

3.  In the **Rate base** field, type **AtlantaBase**.

4.  In the **Name field**, type **Atlanta rate base**.

5.  In the **Break master** field, click the drop-down button to open the
    lookup.

    -   Break masters are used to define the pricing structure and its
        breakpoints. The pricing structure uses tiered pricing that is based on
        physical dimensions.

For this example, use **weight.**

1.  Toggle the expansion of the **Details** section.

2.  Click **New**.

3.  In the **Drop-off Postal Code From** field, type **30301**.

4.  In the **Drop-off Postal Code To** field, type **30318**.

5.  In the **Drop-off Country Region** field, type **USA**.

6.  In the **\<1.00 Lbs** field, type **100**.

    -   Insert the rate per lbs if the total weight of the load is less than 1
        pound.

7.  In the **\<5.00 Lbs** field, type **300**.

    -   Insert the rate per lbs if the total weight of the load is less than 5
        pounds.

8.  In the **\<20.00 Lbs** field, type **500**.

    -   Insert the rate per lbs if the total weight of the load is less than 20
        pounds.

9.  In the **\<100.00** Lbs field, type **1000**.

    -   Insert the rate per lbs if the total weight of the load is less than 100
        pounds.

10. In the **\<1,000.00** Lbs field, type **3000**.

    -   Insert the rate per lbs if the total weight of the load is less than
        1000 pounds.

11. Click **Save**.

12. Close the page.

### Assign rate base

1.  Toggle the expansion of the **Rate base assignments** section.

2.  Click **New**.

    -   You can have several rate base assignments for each rate master. This
        makes it possible to create several different price points for each
        carrier depending on destinations, services, or different rate bases. In
        this procedure you will only create one rate base assignment.

3.  In the Name field, type **AtlantaRateAssignment**.

4.  In the Rate base field, click the drop-down button to open the lookup.

5.  In the list, select **AtlantaBase**.

6.  In the Service field, click the drop-down button to open the lookup.

7.  In the list, find and select **Truck**.

8.  In the Pick-up Postal Code field, type **98052**.

    -   Specify which postal code this rate base assignment should be valid
        from.

9.  In the **Pick-up Country Region** field, type **USA**.

10. Click **Save**.

Exercise \#17 Setup route plans and route guides (Bonus)
--------------------------------------------------------

*Objective: Configure a route pan, hub, and route guide.*

You were asked to help the logistics manager at **USMF** to setup route plans
and route guides.

You will need to do the following:

-   Configure a new route plan for Georgia to Los Angeles.

-   Create a new hub for the warehouses at Georgia and Los Angeles. 

-   Add details to the route plan.

-   Create a route guide for Georgia to Los Angeles.

### Create a new route plan named “GA to LA” 

1.  Open **USMF \> Transportation management \> Setup \> Routing \> Route
    plans.**  

2.  Click **New**. 

3.  In the **Route plan** field, enter **GA to LA**. 

4.  In the **Name** field, enter **Georgia to Los Angeles**. 

5.  Close the form. 

### Create a new hub for Georgia and one for Los Angeles

1.  Open **Transportation management \> Setup \> Routing \> Hub masters**.  

2.  Click **New**.  

3.  In the **Hub** field, enter **Georgia 3**. 

4.  In the **Name** field, enter **Savannah GA**. 

5.  Expand the **Codes** FastTab. 

6.  In the **Hub type** field, select Hub. 

7.  In the **Rate master** field, select **TruckRateMaster**.  

8.  Expand the **Effective dates** FastTab. 

9.  In the **Effective start date and time** field, select **Today**. 

10. In the **Effective end date and time** field, select **12/31/2025**. 

11. Expand the **Address** FastTab. 

12. Click **Add**. 

13. In the **Name or description** field, enter **Georgia 3**. 

14. In the **Zip/postal code** field, enter **31302**. 

15. In the **Street** field, enter **123 ABC Street**. 

16. Click **OK**. 

17. Click **New**.  

18. In the **Hub** field, enter **Los Angeles 2**. 

19. In the **Name** field, enter **Los Angeles CA 2**. 

20. Expand the **Codes** FastTab. 

21. In the **Hub type** field, select Hub. 

22. In the **Rate master** field, select **TruckRateMaster**.  

23. Expand the **Effective dates** FastTab. 

24. In the **Effective start date and time** field, select **Today**. 

25. In the **Effective end date and time** field, select **12/31/2025**. 

26. Expand the **Address** FastTab. 

27. Click **Add**. 

28. In the **Name or description** field, enter **Los Angeles 2**. 

29. In the **Zip/postal code** field, enter **90001**. 

30. In the **Street** field, enter **987 XYZ Avenue**. 

31. Click **OK**. 

32. Close the form. 

### Add details to the route plan.

1.  Open **Transportation management \> Setup \> Routing \> Route plans.**  

2.  Select the **GA to LA** route plan. 

3.  On the **Details** FastTab, click **New**.  

4.  In the **Origin hub** field, select **Georgia 3**. 

5.  In the **Destination hub** field, select **Los Angeles 2**. 

6.  In the **Shipping carrier** field, select **TruckCarrier**. 

7.  In the **Carrier service** field, select **Truck**. 

8.  Close the form. 

 

### Create a route guide 

You must configure a new routing guide for Georgia to Los Angeles. The routing
guide should use a particular shipping carrier, TruckCarrier, with the carrier
service Truck.  

### Create a new routing guide named “GA to LA”. 

1.  Open **USMF \> Transportation management \> Setup \> Routing \> Route
    guides.**  

2.  Click **New**. 

3.  In the **Routing guide** field, enter **GA to LA**. 

4.  In the **Name** field, enter **Georgia to Los Angeles**.  

### Add Information, Origin, Destination, and Result entities to the routing guide. 

1.  Expand the **Information** FastTab. 

2.  In the **Direction** field, select **Outbound**.  

3.  Set the **Active** slider to the **Yes** position. 

4.  In the **Effective start date and time** field, select **Today**. 

5.  In the **Effect end date and time** field, enter **12/31/2025**. 

6.  Expand the **Origin** FastTab. 

7.  In the **Zip/postal code** field, enter **31302**. 

8.  In the **Hub** field, select **Los Angeles 2**. 

9.  In the **Country/region** field, enter **USA**. 

10. Expand the **Destination** FastTab. 

11. In the **Zip/postal code from** field, enter **31302**. 

12. In the **Zip/postal code to** field, enter **90001**. 

13. In the **Hub** field, select **Georgia 3**. 

14. In the **Country/region** field, enter **USA**. 

15. Expand the **Result** FastTab. 

16. In the **Shipping carrier** field, select **TruckCarrier**. 

17. In the **Carrier service** field, select **Truck**. 

18. Click **Save**.

Exercise \#18 Process inbound shipments (Bonus)
-----------------------------------------------

*Objective: Configure a route and manage inbound shipments.*

You were asked to help the logistics manager at USMF, to manage the inbound
shipments from Ade Supply Company.

You will need to do the following:

-   Complete the prerequisite steps.

-   Create a hub, route plan, and route guide.

-   Initiate an inbound shipment.

-   Process an inbound shipment.

-   Confirm an inbound shipment.

### Add a vendor address for the Ade Supply Company. 

1.  Open **Accounts payable \> Vendors \> All vendors**. 

2.  Select vendor **1003** from the list of vendors. 

3.  In the action pane, click **Edit**. 

4.  In the **Addresses** FastTab, click **Add**. 

5.  In the **Name or description** field, type **Ade Supply Main Location**. 

6.  In the **Zip/postal code** field, enter **00210**. 

7.  In the **Street** field, enter **123 Main Street**. 

8.  Set the **Primary** slider to **Yes**. 

9.  Click **OK**. 

10. In the **Invoice and delivery** FastTab, in the **Mode of delivery** field,
    select **Parce-STD**. 

11. Close the forms. 

### Modify the CFR terms of delivery. 

1.  Open **Accounts payable \> Setup \> Terms of delivery**. 

2.  Select **CFR** from the left-hand panel. 

3.  Click **Edit** in the action pane. 

4.  In the **Transportation** FastTab, set the **Add transportation charges to
    retail sales orders** slider to **Yes**. 

5.  Close the form. 

 

### Create a Hub, Route Plan, and Route Guide 

You have been asked to set up a hub for the Ade Supply Company and create a
route plan and guide between the Ade Supply Company and USMF’s Warehouse 61. 

### Create a hub for the Ade Supply Company. 

1.  Open **Transportation management \> Setup \> Routing \> Hub masters**. 

2.  Click **New** in the action pane. 

3.  In the **Hub** field, enter **Ade Supply.** 

4.  In the **Name** field, enter **Ade Supply NH**. 

5.  In the **Codes** FastTab, in the **Hub type** field, select **Hub**. 

6.  In the **Rate master** field, select **ParcelRateMaster**. 

7.  In the **Address** FastTab, click **Add**. 

8.  In the **New address** form, in the **Name or description** field, enter
    **Ade Supply NH**. 

9.  In the **ZIP/postal code** field, enter **00210**. 

10. In the **Street** field, enter **123 Main Street**. 

11. Click **OK**. 

12. Close the form. 

### Create a route plan from New Hampshire to Washington. 

1.  Open **Transportation management \> Setup \> routing \> Route plans**. 

2.  Click **New** in the action pane. 

3.  In the **Route plan** field, enter **NH to WA**. 

4.  In the **Name** field, enter **New Hampshire to Washington**. 

5.  In the **Details** FastTab, click **New**. 

6.  In the **Origin hub** field, select **Ade Supply**. 

7.  In the **Destination hub** field, select **Own WHS**. 

8.  In the **Shipping carrier** field, select **ParcelCarrier**. 

9.  In the **Carrier service** field, select **STD**. 

10. In the **Vendor** field, select **1003**. 

11. Close the form. 

### Create a route guide from New Hampshire to Washington. 

1.  Open **Transportation management \> Setup \> Routing \> Route guides**. 

2.  Click **New** in the action pane. 

3.  In the **Routing guide** field, enter **NH to WA**. 

4.  In the **Name** field, enter **New Hampshire to Washington**. 

5.  In the **Origin** FastTab, in the **ZIP/postal code** field, enter
    **00210**. 

6.  In the **Destination** FastTab, in the **ZIP/postal code** field, enter
    **98052**. 

7.  In the **Result** FastTab, in the **Route plan** field, select **NH to
    WA**. 

8.  Close the form. 

### Initiate an Inbound Shipment 

You have been asked to create a new purchase order for 10 mini-speakers from the
Ade Supply Company. After creating the purchase order, you will need to create
an inbound shipment and then rate shop for the inbound load to find the cheapest
transportation rate. 

### Create a new purchase order. 

1.  Open **Accounts payable \> Purchase orders \> All purchase orders**. 

2.  Click **New** in the action pane. 

3.  On the **Create purchase order** form, in the **Vendor account** field,
    select **1003**. 

4.  In the **General** FastTab, in the **Site** field, select **6**. 

5.  In the **Warehouse** field, select **61**. 

6.  Click **OK**. 

7.  In the **Purchase order lines** FastTab, in the **Item number** field, enter
    **L0101**. 

8.  In the **Quantity** field, enter **10**. 

9.  In the **Unit price** field, enter **50**. 

10. In the **Purchase** tab on the action pane, click **Confirm**. 

### Create an inbound shipment. 

1.  In the **Warehouse** tab on the action pane, click **Load planning
    workbench**. 

2.  Select the check mark column for the purchase order line. 

3.  In the **Supply and demand** tab on the action pane, click **To new load**. 

4.  In the **Load template assignment** form, in the **Load template ID** field,
    select **Stnd Load template**. 

5.  Click **OK**. 

### Rate shop for the inbound load. 

1.  In the **Loads** tab of the Load planning workbench, select **Rate route
    workbench** from the **Rating and routing** drop-down menu. 

2.  In the action pane of the Rate route workbench, click **Rate shop**. 

3.  In the Route results FastTab, clear the **Hide exceptions** check box. 

4.  Select the **Route result** line for the route guide. 

5.  Click **Assign**. 

### Process an Inbound Shipment 

Now that the inbound shipment has been created and rated, you need to schedule
an appointment for the mini-speaker shipment. You’ve also been asked to schedule
driver Tim Smith in and out of the appointment. 

### Schedule an appointment. 

1.  Open **Transportation management \> Planning \> Load planning workbench**. 

2.  In the **Loads** tab, select the load ID for the purchase order created in
    the earlier practice. 

3.  Select **Appointment scheduling** from the **Transportation** drop-down
    menu. 

4.  In the **Appointment scheduling** form, click **New** in the action pane. 

5.  In the **Appointment details** FastTab, in the **Appointment rule** field,
    select **Inbound docks 61**. 

6.  Click **Save**.

7.  In the action pane, click the **Update status** drop-down arrow and select
    **Firm**. 

### Check the driver in

1.  In the action pane, click the **Update status** drop-down arrow and select
    **Driver check-in**. 

2.  In the **Driver check-in details** form, in the **Driver name** field, enter
    **Tim Smith**. 

3.  In the **Driver license** field, enter **123**. 

4.  Click **OK**. 

5.  Close the **Appointment scheduling** form. 

### Check the driver out 

1.  Select **Appointment scheduling** in the **Transportation** drop-down menu. 

2.  In the **Appointment scheduling** form, in the action pane, click the
    **Update status** drop-down arrow and select **Driver check-out**. 

3.  In the **The driver’s information** form, click **OK** to accept the default
    information. 

4.  Close the form. 

### Confirm an Inbound Shipment 

You now need to confirm the inbound load. 

### Confirm the inbound load. 

1.  Open **Transportation management \> Planning \> Load planning workbench**. 

2.  In the **Loads** tab, clear the **Hide shipped and received** check box. 

3.  Click the load ID. 

4.  In the **Load details** form, click the **Ship and receive** tab in the
    action pane, and then select **Inbound shipment** in the **Confirm** area. 

5.  Close the form. 

Exercise \#19 Process outbound shipments
----------------------------------------

*Objective: Manage an outbound shipment and a consolidated shipment*

The logistics manager at USMF, would like to process an outbound shipment for
Desert Wholesales.

This involves receiving and confirming the sales order, reserving stock for the
order, and creating an outbound transportation load.

In addition, Desert Wholesales wants to add another line to their sales order.

They requested that both sales order lines arrive in one consolidated load.

You have been asked to help creating the consolidated load and confirming it. 

You need do the following:

 

-   Initiate an outbound shipment.

-   Create a consolidated shipment.

### Initiating an Outbound Shipment 

You have been asked to confirm a sales order for Desert Wholesales, reserve
stock for the order, and create an outbound transportation load. 

### Receive and confirm the sales order. 

1.  Open **Sales and marketing \> Customers \> All customers**.  

2.  In the list of customers, select the line for account **US-007**. 

3.  In the action pane, click the **Sell** tab. 

4.  In the **New** area, click **Sales order**. 

5.  In the **Sales order** form, expand the **Sales order lines** FastTab, if
    not expanded already. 

6.  In the existing sales order line, in the **Item number** field, enter
    **A0001**. 

7.  In the **Quantity** field, enter **5**. 

8.  In the **Site** field, enter **6**. 

9.  In the **Warehouse** field, enter **62**. 

10. In the **Unit price** field, enter **15**.  

11. In the action pane, click **Save**. 

12. In the action pane, click the **Sell** tab. 

13. In the **Generate** area, click **Confirm sales order**. 

14. Confirm the information on the **Confirm sales order** form and click
    **OK**. 

15. Click **OK** to post without printing. 

### Reserve stock for the order. 

1.  In the **Sales order details** form, select the order line in the **Sales
    order lines** FastTab. 

2.  Click the **Inventory** drop-down arrow and select **Reservation**. 

3.  In the **Reservation** form, in the **Reservation** field, enter **5**. 

4.  In the action pane, click **Reserve lot**. 

5.  Close the form. 

### Create an outbound transportation load. 

1.  In the **Sales order details** form, click the **Warehouse** tab in the
    action pane. 

2.  In the **Loads** area, click **Load planning workbench**. 

3.  In the **Sales lines** tab, select the line for your current sales order. 

4.  In the action pane, click **Supply and demand**. 

5.  In the **Add** area, click **To new load**. 

6.  In the **Load template assignment** form, select **Stnd Load Template** from
    the **Load template ID** drop-down menu. 

7.  Click **OK**. 

8.  Click **OK** to confirm exceeding capacity. 

 

### Creating a Consolidated Shipment 

Desert Wholesales wants to add another line to their sales order. They request
that both sales order lines arrive in one consolidated load. You have been
tasked with creating the consolidated load and confirming it. 

### Set up parameters for consolidated shipments. 

1.  Open **Transportation management \> Setup \> Transportation management
    parameters**. 

2.  Click the **General** tab. 

3.  In the **In transit planning** FastTab, set the **In transit planning**
    slider to **Yes**. 

4.  Close the form. 

### Add a new line to a sales order. 

1.  Open **Accounts receivable \> Orders \> All sales orders**. 

2.  Select the current sales order for Desert Wholesales. 

3.  In the **Sales order details** form, in the **Sales order lines** FastTab,
    click **Add line**. 

4.  In the **Item number** field, enter **A0002**. 

5.  In the **Quantity** field, enter **5**. 

6.  For **Site**, select **5**.

7.  In the action pane, click the **Sell** tab. 

8.  In the **Generate** area, click **Confirm sales order**. 

9.  Confirm the information on the Confirm sales order form and click **OK**. 

10. Click **OK** to post without printing. 

### Reserve stock for the order. 

1.  In the **Sales order details** form, select one of the order lines in the
    **Sales order lines** FastTab. 

2.  Click the **Inventory** drop-down arrow and select **Reservation**. 

3.  In the **Reservation** form, in the **Reservation** field, enter **5**. 

4.  In the action pane, click **Reserve lot**. 

5.  Close the form. 

### Create and confirm a new outbound load. 

1.  In the **Sales order details** form, click the **Warehouse** tab in the
    action pane. 

2.  In the **Loads** area, click **Load planning workbench**. 

3.  In the **Sales lines** tab, select a line for your current sales order. 

4.  In the action pane, click **Supply and demand**. 

5.  In the **Add** area, click **To new load**. 

6.  In the **Load template assignment** form, select **Stnd Load Template** from
    the **Load template ID** drop-down menu. 

7.  Click **OK**. 

8.  Click **OK** to confirm exceeding capacity. 

### Add hub consolidation and rate both loads. 

1.  In the **Load planning workbench**, select the first load you created in the
    **Loads** tab. 

2.  Select **Hub consolidation** in the **Transportation** drop-down menu. 

3.  In the **Override location** form, click the **Hub** drop-down arrow and
    select **Los Angeles**. 

4.  Click **OK**. 

5.  Select the load line in the **Loads** tab. 

6.  Select **Rate route workbench** from the **Rating and routing** drop-down
    menu. 

7.  In the **Rate route workbench**, click **Route with rate** in the action
    pane. 

8.  In the **Route Results** FastTab, select route guide **Wh 61 to Cust 003 004
    019**. 

9.  Click **Assign**. 

10. Close the **Routes** form and the **Rate route workbench**. 

11. Repeat steps **1–10** for the second load. 

### Create the consolidated load. 

1.  In the **Transportation request lines** tab, select both lines. 

2.  In the action pane, click the **Supply and demand** tab. 

3.  In the **Add** area, click **To new load**. 

4.  In the **Load template assignment** form, select **Stnd Load Template** from
    the **Load template ID** drop-down menu. 

5.  Click **OK**. 

6.  Click **OK** to confirm exceeding capacity. 

*Note:* The consolidated load may take several minutes to appear in the Loads
tab. 

### Rate the consolidated load. 

1.  In the **Loads** tab, select the consolidated load line. 

2.  Select **Rate route workbench** from the **Rating and routing** drop-down
    menu. 

3.  In the **Rate route workbench**, click **Route with rate** in the action
    pane. 

4.  In the **Route Results** FastTab, select route guide **Wh 61 to Cust 003 004
    019**. 

5.  Click **Assign**. 

6.  Close the **Routes** form and the **Rate route workbench**. 

### Confirm the consolidated load shipment. 

1.  On the **Load planning workbench**, in the **Loads** tab, select the
    consolidated load line. 

2.  Select **Outbound load** in the **Ship and receive** drop-down menu. 

Exercise \#20 Configure freight reconciliation (Bonus)
------------------------------------------------------

*Objective: Configure and manage freight reconciliation.*

You were asked to help the logistics manager at **USMF**, to setup the system
for Desert Wholesales for freight reconciliation.

You will need to do the following:

-   Create the freight reconciliation reason code for overtime.

-   Verify that the fright bill type is configured.

-   Create a freight bill type assignment for the truck carrier service.

-   Create a billing group named Duties.

-   Create an audit master for overtime.

### Create a freight reconciliation reason code for Overtime

1.  Open **Transportation management \> Setup \> Freight reconciliation \>
    Reconciliation reasons**. 

2.  Click **New**. 

3.  Type **OT** in the **Reconciliation reason code** field. 

4.  Type **Overtime** in the **Description** field. 

5.  Type **211650** in the **Debit account** field. 

6.  Select the **Pay the freight vendor** check box. 

7.  Close the form. 

### Verify the Freight bill type is configured

1.  Open **Transportation management \> Setup \> Freight reconciliation \>
    Freight bill type**. 

2.  Select the TL **Freight bill type**. 

3.  Verify the **Engine assembly** field is populated. 

4.  Verify that two records exist, one for Billing group ID and one for External
    code. 

5.  Close the form. 

### Create a freight bill type assignment for the Truck Carrier service. 

1.  Open **Transportation management \> Setup \> Freight reconciliation \>
    Freight bill type assignments**. 

2.  Click **New**. 

3.  Select **None** in the **Direction** field. 

4.  Select **Ground** in the **Mode** field. 

5.  Select **TruckCarrier** in the **Shipping carrier** field. 

6.  Select **TL** in the **Freight bill type** field. 

7.  Close the form. 

### Create a billing group named Duties. 

1.  Open **Transportation management \> Setup \> Freight reconciliation \>
    Billing Group**. 

2.  Click **New**. 

3.  Type **Duties** in the **Billing group** field. 

4.  Type **Duties** in the **Name** field. 

5.  Close the form. 

### Create an audit master for overtime. 

1.  Open **Transportation management \> Setup \> Freight reconciliation \> Audit
    master**. 

2.  Click **New**. 

3.  Enter **Overtime** in the **Audit master ID** field. 

4.  Select **TruckCarrier** in the **Shipping carrier** field. 

5.  Select **TL** in the **Freight bill type** field. 

6.  In the **Result** FastTab, select **OT** in the **Overpayment reason code**
    field. 

7.  Select **Damage claim** in the **Underpayment reason code** field. 

8.  Close the form. 
