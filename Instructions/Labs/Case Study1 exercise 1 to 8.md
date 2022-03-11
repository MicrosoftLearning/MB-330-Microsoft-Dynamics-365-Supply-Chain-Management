---
lab:
    title: 'Case study 1 Product information management and inventory management'
    module: 'Module 2: Implement inventory management '
---

Case study 1 Product information management and inventory management
====================================================================

Objectives
----------

-   Create and manage products.

-   Manage inventory pricing and costing.

-   Configure inventory management.

-   Manage and process inventory activities.

Scenario 
---------

**Company Information**

USMF is a United States company that manufactures products for several different
industries and has a diverse portfolio of products.

**Business Challenges and Requirements**

USMF recently implemented Dynamics 365 Supply Chain Management. They hired a new
full-time team to manage the warehouse and inventory, the new staff doesn’t have
Dynamics 365 Supply Chain management knowledge.

**Your Role**

You are the Dynamics 365 Supply Chain Management functional consultant that
implemented the solution. You are called to help the new staff in multiple
areas.

Exercise \#1 Adding products to a new warehouse using basic inventory management.
---------------------------------------------------------------------------------

*Objective: Add products to a new warehouse using basic inventory management.* 

You are the supply chain management functional consultant on a project team
advising your customer on best way to create new warehouse to store the overflow
of new products.

Your customer is managing a small warehouse that does not require the full
capabilities of warehouse management systems (WMS).

you and the Solution architect are in favor of using basic inventory management
to help them creating the new warehouse.

**What would you do?**

### Set the default location capacity.

1.  Go to **Inventory management \> Setup \> Inventory and warehouse management
    parameters**.

2.  Click the **Locations** tab.

3.  In the **Standard width** field, enter 450.

4.  In the **Standard depth** field, enter 250.

5.  In the **Standard height** field, enter 200.

6.  Click **Save**.

7.  Close the page.

### Define the location name format.

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

8.  Set the **Include aisle** option to **Yes**.

9.  Set the **Include rack** option to **Yes**.

10. In the **Format** field, for the rack, type -\#\#

11. Set the **Include shelf** option to **Yes**.

12. In the **Format** field, for the shelf, type -\#\#

13. Click **Save**.

### Define warehouse locations

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

12. On the **Specify additional information for all your picking locations**
    screen, note that the physical dimensions shown on this page are the ones
    that you set at the start of this procedure. Click **Next**.

13. On the **Edit and delete picking locations** screen, click **Next**.

14. Click **Finish**.

15. Close all pages.

Exercise \#2 Creating a standard cost version that uses a specific model group.
-------------------------------------------------------------------------------

*Objective: Create a standard cost version to record certain model group
products.* 

The warehouse employee at USMF, need to create a standard cost version to record
products that use the item model group with inventory model of Standard. The
items must be grouped based on FIFO inventory model.

**What would you do to help this employee?**

### Create cost version

1.  Go to **Cost management \> Predetermined cost policies setup \> Costing
    versions**.

2.  Click **New**.

3.  In the **Costing type** field, select **Standard cost**.

4.  In the **Version** field, type **SeahorseST**.

5.  In the **Name** field, type **Seahorse Standard Costing**.

6.  In the **Block activation** field, select **No**.

7.  Click **Save**.

8.  Close the page.

### Create item model group

1.  Go to **Cost management \> Inventory accounting policies setup \> Item model
    groups**.

2.  Click **New**.

3.  In the **Item model group** field, type **STDN**.

4.  In the **Name** field, type **Standard Cost**.

5.  In the **Inventory model** field, select **Standard cost**.

6.  Expand the **Inventory policies** section.

7.  In the **Approved vendor check** method field, select **No check**.

8.  Click **New**.

9.  In the **Item model group** field, type **FIFO2**.

10. In the **Name** field, type **FIFO 2**.

11. Click **Save**.

12. Close the page.

### Create tracking number group

1.  Go to **Inventory management \> Setup \> Dimensions \> Tracking number
    groups**.

2.  Click **New**.

3.  In the **Number group** field, type **ASer**.

4.  In the **Name** field, type **Auto-Serial**.

5.  Select No in the **Date** field.

6.  Select No in the **Lot ID** field.

7.  Select Yes in the **Number sequence No.** field.

8.  Select Yes in the **Only for inventory transactions** field.

9.  Select Yes in the **On physical update** field.

10. Click **New**.

11. In the **Number group** field, type **USer**.

12. In the **Name** field, type **Unique-Serial**.

13. Select No in the **Date** field.

14. Select No in the **Lot ID** field.

15. Select Yes in the **Number sequence No**. field.

16. In the **Number sequence code** field, choose any number sequence of your
    choice.

17. Select Yes in the **Only for inventory transactions** field.

18. Select Yes in the **On physical update** field.

19. Set **Per qty.** to **1**.

20. Click **New**.

21. In the **Number group** field, type **Batch**.

22. In the **Name** field, type **Auto Batch**.

23. Select No in the **Date** field.

24. Select No in the **Lot ID** field.

25. Select Yes in the **Number sequence No**. field.

26. In the **Number sequence code** field, choose any number sequence of your
    choice

27. Select Yes in the **Only for inventory transactions** field.

28. Select No in the **On physical update** field.

29. Close the page.

Exercise \#3 Adding and releasing new products to a warehouse
-------------------------------------------------------------

*Objective: Add new products with and without variants.* 

Some new products are introduced by USMF and must be added to the new warehouse.
As supply chain manager, you will have to create 2 new products:

-   A V-neck T-shirt with multiple variants that has different colors and sizes.
    This item will be available in size Small, Medium and Large and in colors:
    Black and Red.

-   The product type should set to: Product with no variance for the cabinets

**What would you do?**

### Create product masters

1.  Navigate to **Product information management\>Products\>Released products**.

2.  Click **New**.

3.  In the **Product type** field, select **Item**.

4.  In the **Product subtype** field, select **Product master**.

5.  In the **Product number** field, type **GTLS001**.

6.  In the **Product name** field, type **V Neck T-Shirt**.

7.  In the **Search name** field, type **VNeckTShirt**.

8.  In the **Retail category** field, select **Apparel and Footwear**.

9.  In the **Product dimension group** field, select **ColorSize**.

10. In the **Configuration technology** field, select **Predefined variant**.

11. In the **Item model group** field, select **FIFO** (First In-First Out).

12. In the Item group field, select **Audio**.

13. In the **Storage dimension group** field, select **SiteWH**.

14. In the **Tracking dimension group** field, select **None**.

15. In the **Inventory unit** field, select **ea** (Each).

16. In the **Purchase unit** field, select **ea** (Each).

17. In the **Sales unit** field, select **ea** (Each).

18. In the **BOM unit** field, select **ea** (Each).

19. In the Sales Taxation, **Item sales tax group** field, select **ALL** (All
    sales tax codes).

20. In the Purchase Taxation, **Item sales tax group** field, select **ALL**
    (All sales tax codes).

21. Click **OK**.

22. Close all pages.

23. Navigate to **Product information management\>Products\>Released products**.

24. Using quick filter search by item number for **GTLS001**.

25. Click item **GTLS001** to open the product master record.

26. Click the **Product dimensions** button from the **Product** action pane.

27. Select the **Sizes** tab.

28. Click **New** in the **Define sizes for a product master** section.

29. In the **Size** field, enter **Small**.

30. In the **Name** field, enter **Small**.

31. In the **Description** field, enter **Small Size**.

32. Click **New**.

33. In the **Size** field, enter **Medium**.

34. In the **Name** field, enter **Medium**.

35. In the **Description** field, enter **Medium Size**.

36. Click **New**.

37. In the **Size** field, enter **Large**.

38. In the **Name** field, enter **Large**.

39. In the **Description** field, enter **Large Size**.

40. Select the **Colors** tab.

41. Click **New** in the **Define sizes for a product master** section.

42. In the **Color** field, enter **Black**.

43. In the **Name** field, enter **Black**.

44. In the **Description** field, enter **Black color**.

45. Click **New**.

46. In the **Color** field, enter **Red**.

47. In the **Name** field, enter **Red**.

48. In the **Description** field, enter **Red color**.

49. Click **Save**.

50. Close the form.

51. Click **Released Product variants** button from the **Product** action pane.

52. Click **Variant suggestions** from the **Product Variant** action pane.

53. Click **Suggest all**.

54. Click **Create**.

Close all pages.

Exercise \#4 Using the inventory movement journal to initialize stock levels in a warehouse
-------------------------------------------------------------------------------------------

*Objective: Initialize stock levels in a warehouse by using movement journals.* 

USMF company has some inventory opening balance for one of its products and is
it necessary to add to that stock. There are no specific purchase order
references for the items, so the opening balance will have to be forced into the
system.

The warehouse manager, will have to use the inventory movement journal to add
the opening balance and use an offset account to balance the transaction in the
general ledger.

In USMF, its possible to update the on-hand inventory manually using an
Inventory movement journal.

It is also possible to update on-hand inventory by importing transactions in
data entities.

**What would you do to guide the warehouse manager?**

### Initialize stock levels in the warehouse using movement journals

1.  Go to **Inventory management \> Journal entries \> Items \> Movement**.

2.  Click **New**.

3.  In the **Name** field, click the drop-down button to open the lookup.

4.  Select **Imov**. It is a good practice to use different journal name
    templates for the different business purposes.

5.  In the **Offset account** field, specify the values **140200.** This is the
    offset account that will be the default account on the journal lines. It is
    possible to override the default to assign different offset accounts per
    line.

6.  Click **OK**.

7.  Click **New** in the **Journal lines** fast tab.

8.  In the Item number field, click the drop-down button to open the lookup.

9.  Select item **A0001**.

10. Click the **Inventory dimensions** tab.

11. In the **Site** field, click the drop-down button to open the lookup.

12. Select site **1**.

13. In the **Warehouse** field, click the drop-down button to open the lookup.

14. Select warehouse **13**.

15. In the **Location** field, click the drop-down button to open the lookup.

16. Select location **13**.

17. In the **Quantity** field, enter a number.

18. Click **Save**.

19. Click **Post**.

20. Check or uncheck the **Transfer all posting errors to a new journal** check
    box. If you enable this option, any lines that fail to post will be copied
    to a new journal. You can use the information in the log to correct the
    issues and then re-post the lines.

21. Click **OK**.

22. Close all pages.

Exercise \#5 Using the inventory transfer journal to move items to a new location in the warehouse
--------------------------------------------------------------------------------------------------

*Objective: Move items from a plate-controlled location to a location that is
not license plate controlled.* 

### Transfer physical inventory within the warehouse using transfer journals

1.  Go to **Inventory management\>Journal entries\>Items\>Transfer**.

2.  Click **New**.

3.  In the **Name** field, enter or select **ITrf**.

4.  Click **OK**.

5.  Click **New** in the **Journal lines** fast tab.

6.  In the **Item number** field, enter or select **A0001**.

7.  In the **From site** field, enter or select **2**.

8.  In the **To site** field, enter or select **2**.

9.  In the **From warehouse** field, enter or select **24**.

10. In the **To warehouse** field, enter or select **24**.

11. In the **From location** field, enter or select **FL-001**.

12. In the **To location** field, enter or select **BULK-001**.

13. In the **Quantity** field, enter a number.

14. Click the **Inventory dimensions** tab in the **Line details** fast tab.

15. In the **License plate** field, in **From inventory dimensions**, enter or select **24**.

16. Click **Save**.

17. Click **Post**.

18. Click **OK**.

19. Click **Inventory** in the **Journal lines** fast tab.

20. Click **Transactions** to see the transfer.

21. Close all pages.

Exercise \#6 Adjusting stock levels using the inventory adjustment journal
--------------------------------------------------------------------------

*Objective: Adjust stock levels after an error by using the inventory adjustment
journal.* 

During the transfer journal processing a user recorded the wrong number of items
moved to the new location.

You were asked to use the inventory adjustment journal to fix quantity.

You will also need to adjust the stock levels of products in the warehouse.

**How would you perform this?**

### Adjust stock levels in the warehouse

1.  Go to **Inventory management \> Journal entries \> Items \> Inventory
    adjustment**.

2.  Click **New**.

3.  In the **Name** field, click the drop-down button to open the lookup.

4.  In the list, click on the inventory adjustment journal name you want to use.
    Some other fields will be populated based on the setup of the inventory
    adjustment journal name you select.

5.  Click **OK**.

6.  Click **New** in the **Journal lines** fast tab.

7.  In the **Item number** field, select **D0001**.

8.  In the **Site** field, click the drop-down button to open the lookup.

9.  In the list, select a site 1.

10. In the **Warehouse** field, click the drop-down button to open the lookup.

11. In the list, select warehouse 13. If you have selected an item with Location
    as a mandatory dimension, you would have to specify the location here.

12. In the **Quantity** field, enter a number. The cost price field specifies
    the cost per unit for inventory receipts. If the cost is not specified for
    the item number or if you wanted to change it manually, you would do this
    here.

13. Click **Validate**.

14. Click **OK**.

15. Note that the Journal is OK, and click **Post**. When you post this kind of
    journal, an inventory receipt or issue is posted, the inventory level and
    value are changed, and ledger transactions are generated.

16. Click **OK**.

17. Close all pages.

Exercise \#7 Using the inventory counting journal to compare D365 inventory amounts to manually counted quantities
------------------------------------------------------------------------------------------------------------------

*Objective: Use the inventory counting journal to compare manually counted
amounts to the on hand recorded amounts in D365 supply chain and post the
transaction.* 

A few days after you have adjusted stock levels, the warehouse manager decide to
manually count the items in that specific area of the warehouse.

The warehouse manager wants to enter the manually counted quantity and not sure
what to use.

**how would you help?**

### Use counting journals

1.  Go to **Inventory management \> Journal entries \> Item counting \>
    Counting**.

2.  Click **New**.

3.  In the **Name** field, click the drop-down button to open the lookup.

4.  In the list, click on the inventory counting journal **Icnt**. Some other
    fields will be populated based on the setup of the inventory counting
    journal name that you select.

5.  In the **Worker** field, click the drop-down button to open the lookup.

6.  In the list, select the worker you want to use.

7.  Click **Select**.

8.  Click **OK**.

9.  Click **New** in the **Journal lines** fast tab.

10. In the **Item number** field, click the drop-down button to open the lookup.

11. In the list, find and select **A0001**.

12. In the **Site** field, click the drop-down button to open the lookup.

13. In the list, find and select site **2**.

14. In the **Warehouse** field, click the drop-down button to open the lookup.

15. In the list, find and select warehouse **24**.

16. In the **Location** field, click the drop-down button to open the lookup.

17. In the list, find and select location **BULK-001**.

18. In the **Counted** field, enter a number.

19. If you enter a counted number that’s different than the number shown in the
    **On-hand** field, the **Quantity** field is updated to show the
    discrepancy.

20. Click **Save**.

21. Click **Post**. When you post an inventory counting journal, if the counted
    amount differs from the amount that’s reported in the **On-hand** field, an
    inventory receipt or issue is posted, the inventory level and value are
    changed, and ledger transactions are generated.

22. Click **OK**.

23. Close all pages.

Exercise \#8 Creating a BOM in the BOM designer (Bonus)
-------------------------------------------------------

*Objective:  Create a BOM in the BOM designer with a title, item group, site and
quantities.*

The designer at USMF has received a new specification for the enclosure
side of a cabinet. and she has requested your assistance. You see that an item
is not set up for this specification, so you only need to create a simple BOM
with component lines. Use employee 000020, Julia Funderburk, to approve the BOM.

Create a BOM titled “High Quality Speaker” and assign it to the Audio item group
at site 1. Use the BOM designer to add items with warehouse 11 and the following
quantities:

-   1 qty of M0008 / High End Cabinet / Black

-   2 qty of M0002 / Mid-Range Speaker Unit

-   1 qty of M0009 / Protective Corners

You will:

### Create a BOM in the BOM designer.

1.  Go to **Product information management \> Bills of materials and formulas \>
    Bills of materials**.

2.  Click **New**.

3.  In the **Name** field, type **High Quality Speaker**.

4.  In the **Site** field, type **1**.

5.  In the **Item group** field, enter or select **Audio**.

6.  Click **Designer**.

7.  Click **Formula lines**.

8.  Click **Add to component BOM**.

9.  In the list, find and select **M0008 / High End Cabinet / Black** (the
    checkbox on the left should be checked).

10. Click **OK**.

11. Click **Formula lines**.

12. Click **Add after line.**

13. In the list, find and select **M0009 / Protective Corners**.

14. Click **OK**.

15. Click **Formula lines**.

16. Click **Add before line**.

17. In the list, find and select **M0002 / Mid-Range Speaker Unit**.

18. Click **OK**.

19. Close the page.

20. Refresh the page.

21. In the list of Bill of materials lines, find and select the row for **M0002
    / Mid-Range Speaker Unit**.

22. Set **Quantity** to **2.0000**.

23. In the Maintain action group, click **Approval**. Select **000020**, Julia Funderburk.

24. Click **OK**.

25. Close all pages.
