---
lab:
    title: 'Case study 1 Product information management and inventory management'
    module: 'Module 2: Implement inventory management'
---

Case study 1 Product information management and inventory management
====================================================================

Objectives
----------

- Create and manage products.

- Manage inventory pricing and costing.

- Configure inventory management.

- Manage and process inventory activities.

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

Exercise \#1 Adding products to a new warehouse using basic inventory management
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

### Set the default location capacity

1. Access the **Microsoft Dynamics 365 Supply Chain Managment** website and log in with your user credentials.

2. On the **Finance and Operations** dashboard page, expand the left navigation pane and select the **Inventory management** under the **Modules** tab.

3. On the **Inventory management** page select the  **Setup \> Inventory and warehouse management
    parameters**.

4. Select the **Locations** tab.

5. In the **Standard width** field, enter `450`.

6. In the **Standard depth** field, enter `250`.

7. In the **Standard height** field, enter `200`.

8. Select **Save**.

9. Close the page.

### Define the location name format

1. On the **Finance and Operations** dashboard page, expand the left navigation pane and select the **Inventory management** under the **Modules** tab. On the **Inventory management** page select  **Setup \> Inventory breakdown \> Warehouses**.

2. Select **New**.

3. In the **Warehouse** field, enter `17`.

4. In the **Name** field, enter `Raw materials`.

5. In the **Site** field, select the drop-down button to open the lookup.

6. In the list, find and select site **1**.

7. Expand the **Location names** section. The options in this section define
    the default format for location names. In our example, we'll include the
    aisle number, rack number and shelf number.

8. Set the **Include aisle** option to **Yes**.

9. Set the **Include rack** option to **Yes**.

10. In the **Format** field, for the rack, enter **-\#\#**

11. Set the **Include shelf** option to **Yes**.

12. In the **Format** field, for the shelf, enter **-\#\#**

13. Select **Save**.

### Define warehouse locations

1. On the Action Pane, select **Warehouse**.

2. Select **Location Wizard**.

3. On the **Welcome** screen, select **Next**.

4. De-select the **Outbound docks** option.

5. De-select the **Bulk locations** option.

6. Select **Next**.

7. On the **Create inventory aisles** screen, select **Next**.

8. On the **Edit and delete aisles** screen, select **Next**.

9. On the **Create inbound docks** screen, select **Next**.

10. On the **Edit and delete inbound docks** screen, select **Next**.

11. On the **Create picking locations** screen, select **Next**.

12. Review the physical dimensions shown on the the **Specify additional information for all your picking locations** screen and select **Next**.
    > **Note** The physical dimensions shown on this page are the ones
    that you set at the start of this procedure.

13. On the **Edit and delete picking locations** screen, select **Next**.

14. Select **Finish**.

15. Close all pages.

Exercise \#2 Creating a standard cost version that uses a specific model group
-------------------------------------------------------------------------------

*Objective: Create a standard cost version to record certain model group
products.*

The warehouse employee at USMF, need to create a standard cost version to record
products that use the item model group with inventory model of Standard. The
items must be grouped based on FIFO inventory model.

**What would you do to help this employee?**

### Create cost version

1. Go to **Cost management \> Predetermined cost policies setup \> Costing
    versions**.

2. Select **New**.

3. In the **Costing type** field, select **Standard cost**.

4. In the **Version** field, enter `SeahorseST`.

5. In the **Name** field, enter `Seahorse Standard Costing`.

6. In the **Block activation** field, select **No**.

7. Select **Save**.

8. Close the page.

### Create item model group

1. Go to **Cost management \> Inventory accounting policies setup \> Item model
    groups**.

2. Select **New**.

3. In the **Item model group** field, enter `STDN`.

4. In the **Name** field, enter `Standard Cost`.

5. In the **Inventory model** field, select **Standard cost**.

6. Expand the **Inventory policies** section.

7. In the **Approved vendor check method** field, select **No check**.

8. Select **New**.

9. In the **Item model group** field, enter `FIFO2`.

10. In the **Name** field, enter `FIFO 2`.

11. Select **Save**.

12. Close the page.

### Create tracking number group

1. Go to **Inventory management \> Setup \> Dimensions \> Tracking number
    groups**.

2. Select **New**.

3. In the **Number group** field, enter `ASer`.

4. In the **Name** field, enter `Auto-Serial`.

5. Turn off the **Date** toggle to **No**.

6. Turn off the **Lot ID** toggle to **No**.

7. Turn on the **Number sequence No.** toggle to **Yes**.

8. Turn on the **Only for inventory transactions** toggle to **Yes**.

9. Turn on the **On physical update** toggle to **Yes**.

10. Select **New**.

11. In the **Number group** field, enter `USer`.

12. In the **Name** field, enter `Unique-Serial`.

13. Turn off the **Date** toggle to **No**.

14. Turn off the **Lot ID** toggle to **No**.

15. Turn on the **Number sequence No.** toggle to **Yes**.

16. In the **Number sequence code** field, choose any number sequence of your
    choice.

17. Turn on the **Only for inventory transactions** toggle to **Yes**.

18. Turn on the **On physical update** toggle to **Yes**.

19. Set **Per qty.** to **1**.

20. Select **New**.

21. In the **Number group** field, enter `Batch`.

22. In the **Name** field, enter `Auto Batch`.

23. Turn off the **Date** toggle to **No**.

24. Turn off the **Lot ID** toggle to **No**.

25. Turn on the **Number sequence No.** toggle to **Yes**.

26. In the **Number sequence code** field, choose any number sequence of your
    choice

27. Turn on the **Only for inventory transactions** toggle to **Yes**.

28. Turn off the **On physical update** toggle to **No**.

29. Close the page.

Exercise \#3 Adding and releasing new products to a warehouse
-------------------------------------------------------------

*Objective: Add new products with and without variants.*

Some new products are introduced by USMF and must be added to the new warehouse.
As supply chain manager, you will have to create 2 new products:

- A V-neck T-shirt with multiple variants that has different colors and sizes.
    This item will be available in size Small, Medium and Large and in colors:
    Black and Red.

- The product type should set to: Product with no variance for the cabinets

**What would you do?**

### Create product masters

1. Navigate to **Product information management\>Products\>Released products**.

2. Select **New**.

3. In the **Product type** field, select **Item**.

4. In the **Product subtype** field, select **Product master**.

5. In the **Product number** field, enter `GTLS001`.

6. In the **Product name** field, enter `V Neck T-Shirt`.

7. In the **Search name** field, enter `VNeckTShirt`.

8. In the **Retail category** field, select **Apparel and Footwear** and select **OK**.

9. In the **Product dimension group** field, select **ColorSize**.

10. In the **Configuration technology** field, select **Predefined variant**.

11. In the **Item model group** field, select **FIFO** (First In-First Out).

12. In the **Item group** field, select **Audio**.

13. In the **Storage dimension group** field, select **SiteWH**.

14. In the **Tracking dimension group** field, select **None**.

15. In the **Inventory unit** field, select **ea**.

16. In the **Purchase unit** field, select **ea**.

17. In the **Sales unit** field, select **ea**.

18. In the **BOM unit** field, select **ea**.

19. In the Sales Taxation, **Item sales tax group** field, select **ALL** (All
    sales tax codes).

20. In the Purchase Taxation, **Item sales tax group** field, select **ALL**
    (All sales tax codes).

21. Select **OK**.

22. Close all pages.

23. Navigate to **Product information management\>Products\>Released products**.

24. Using quick filter search by item number for **GTLS001**.

25. Select item **GTLS001** to open the product master record.

26. On the Action Pane, select the **Product** tab, select **Product dimensions** listed under the **Product master** section.

27. Select the **Sizes** tab.

28. Select **New** in the **Define sizes for a product master** section.

29. In the **Size** field, select **Small**.

30. In the **Name** field, enter `Small`.

31. In the **Description** field, enter `Small Size`.

32. Select **New**.

33. In the **Size** field, select **Medium**.

34. In the **Name** field, enter `Medium`.

35. In the **Description** field, enter `Medium Size`.

36. Select **New**.

37. In the **Size** field, select **Large**.

38. In the **Name** field, enter `Large`.

39. In the **Description** field, enter `Large Size`.

40. Select the **Colors** tab.

41. Select **New** in the **Define colors for a product master** section.

42. In the **Color** field, select **Black**.

43. In the **Name** field, enter `Black`.

44. In the **Description** field, enter `Black color`.

45. Select **New**.

46. In the **Color** field, select **Red**.

47. In the **Name** field, enter `Red`.

48. In the **Description** field, enter `Red color`.

49. Select **Save**.

50. Close the form.

51. Select **Released product variants** listed under the **Product master** section.

52. Select **Variant suggestions** listed under the **Released product Variants** section.

53. Select **Suggest all** from the **Variant suggestions** and then select **Select all** from the **Suggested variants**.

54. Select **Create**.

55. Close all pages.

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

1. Go to **Inventory management \> Journal entries \> Items \> Movement**.

2. Select **New**.

3. In the **Name** field, select the drop-down button to open the lookup.

4. Select **Imov**. It is a good practice to use different journal name
    templates for the different business purposes.

5. In the **Offset account** field, specify the values **140200**. 
    > **Note** This is the offset account that will be the default account on the journal lines. It is
    possible to override the default to assign different offset accounts per line.

6. Select **OK**.

7. Select **New** in the **Journal lines** fast tab.

8. In the **Item number** field, select the drop-down button to open the lookup.

9. Select item **A0001**.

10. In the **Site** field, select the drop-down button to open the lookup.

11. Select site **1**.

12. In the **Warehouse** field, select the drop-down button to open the lookup.

13. Select warehouse **13**.

14. In the **Location** field, select the drop-down button to open the lookup.

15. Select location **13**.

16. In the **Quantity** field, enter a number.

17. Review changes in the **Line details** FastTab.

18. Select **Save**.

19. Select **Post**.

20. Toggle on or toggle off the **Transfer all posting errors to a new journal** field.
    > **Note** If you enable this option, any lines that fail to post will be copied to a new journal. You can use the information in the log to correct the issues and then re-post the lines.

21. Select **OK**.

22. Close all pages.

Exercise \#5 Using the inventory transfer journal to move items to a new location in the warehouse
--------------------------------------------------------------------------------------------------

*Objective: Move items from a plate-controlled location to a location that is
not license plate controlled.*

### Transfer physical inventory within the warehouse using transfer journals

1. Go to **Inventory management\>Journal entries\>Items\>Transfer**.

2. Select **New**.

3. In the **Name** field, enter or select **ITrf**.

4. Select **OK**.

5. Select **New** in the **Journal lines** fast tab.

6. In the **Item number** field, enter or select **A0001**.

7. In the **From site** field, enter or select **2**.

8. In the **To site** field, enter or select **2**.

9. In the **From warehouse** field, enter or select **24**.

10. In the **To warehouse** field, enter or select **24**.

11. In the **From location** field, enter or select **FL-001**.

12. In the **To location** field, enter or select **BULK-001**.

13. In the **Quantity** field, enter a number.

14. Select the **Inventory dimensions** tab in the **Line details** fast tab.

15. In **From inventory dimensions**, enter **24** in the  **License plate** field.

16. Select **Save**.

17. Select **Post**.

18. Select **OK**.

19. Select **Inventory** in the **Journal lines** fast tab.

20. Select **Transactions** to see the transfer.

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

1. Go to **Inventory management \> Journal entries \> Items \> Inventory
    adjustment**.

2. Select **New**.

3. In the **Name** field, select the drop-down button to open the lookup.

4. Select **IAdj**.

5. Select **OK**.

6. Select **New** in the **Journal lines** fast tab.

7. In the **Item number** field, select **D0001**.

8. In the **Site** field, select the drop-down button to open the lookup.

9. In the list, select site **1**.

10. In the **Warehouse** field, select the drop-down button to open the lookup.

11. In the list, select **warehouse 13**. If you have selected an item with Location
    as a mandatory dimension, you would have to specify the location here.

12. In the **Quantity** field, enter a number. The cost price field specifies
    the cost per unit for inventory receipts. If the cost is not specified for
    the item number or if you wanted to change it manually, you would do this
    here.

13. Select **Validate**.

14. Select **OK**.
    > **Note** that the Journal is OK, and select **Post**. When you post this kind of
    journal, an inventory receipt or issue is posted, the inventory level and
    value are changed, and ledger transactions are generated.

15. Select **OK**.

16. Close all pages.

Exercise \#7 Using the inventory counting journal to compare D365 inventory amounts to manually counted quantities
------------------------------------------------------------------------------------------------------------------

*Objective: Use the inventory counting journal to compare manually counted
amounts to the on hand recorded amounts in D365 supply chain and post the
transaction.*

A few days after you have adjusted stock levels, the warehouse manager decide to
manually count the items in that specific area of the warehouse.

The warehouse manager wants to enter the manually counted quantity and not sure
what to use.

**How would you help?**

### Use counting journals

1. Go to **Inventory management \> Journal entries \> Item counting \>
    Counting**.

2. Select **New**.

3. In the **Name** field, select the drop-down button to open the lookup.

4. In the list, select on the inventory counting journal **Icnt**.

5. In the **Worker** field, select the drop-down button to open the lookup.

6. In the list, select the worker you want to use.

7. Select **Select**.

8. Select **OK**.

9. Select **New** in the **Journal lines** fast tab.

10. In the **Item number** field, select the drop-down button to open the lookup.

11. In the list, find and select **A0001**.

12. In the **Site** field, select the drop-down button to open the lookup.

13. In the list, find and select site **2**.

14. In the **Warehouse** field, select the drop-down button to open the lookup.

15. In the list, find and select warehouse **24**.

16. In the **Location** field, select the drop-down button to open the lookup.

17. In the list, find and select location **BULK-001**.

18. In the **Counted** field, enter a number.

19. If you enter a counted number that’s different than the number shown in the
    **On-hand** field, the **Quantity** field is updated to show the
    discrepancy.

20. Select **Save**.

21. Select **Post**. When you post an inventory counting journal, if the counted
    amount differs from the amount that’s reported in the **On-hand** field, an
    inventory receipt or issue is posted, the inventory level and value are
    changed, and ledger transactions are generated.

22. Select **OK**.

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

- 1 qty of M0008 / High End Cabinet / Black

- 2 qty of M0002 / Mid-Range Speaker Unit

- 1 qty of M0009 / Protective Corners

You will:

### Create a BOM in the BOM designer

1. Go to **Product information management \> Bills of materials and formulas \>
    Bills of materials**.

2. Select **New**.

3. In the **Name** field, enter `High Quality Speaker`.

4. In the **Site** field, enter **1**.

5. In the **Item group** field, enter or select **Audio**.

6. On the **Maintain** tab from top, select **Designer**.

7. Select **BOM lines**.

8. Select **Add to component BOM**.

9. In the list, find and select **M0008 / High End Cabinet / Black**.

10. Select **OK**.

11. Select **BOM lines**.

12. Select **Add after line.**

13. In the list, find and select **M0009 / Protective Corners**.

14. Select **OK**.

15. Select **BOM lines**.

16. Select **Add before line**.

17. In the list, find and select **M0002 / Mid-Range Speaker Unit**.

18. Select **OK**.

19. Close the page.

20. Refresh the page. This will allow the BOM lines to appear in the grid for the BOM.

21. In the list of Bill of materials lines, find and select the row for **M0002
    / Mid-Range Speaker Unit**.

22. Set **Quantity** to **2.0000**.

23. In the **Maintain** tab, select **Approval**. Select **000020, Julia Funderburk**.

24. Select **OK**.

25. Close all pages.
