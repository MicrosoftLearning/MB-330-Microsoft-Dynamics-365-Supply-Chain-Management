---
lab:
    title: 'Case study 2A Inventory management'
    module: 'Module 2: Implement inventory and asset management'
---

Case study 2A Inventory management
====================================================================

Objectives
----------

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

Exercise \#1 Using the inventory movement journal to initialize stock levels in a warehouse
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
    > **Note**This is the offset account that will be the default account on the journal lines. It is
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

Exercise \#2 Using the inventory transfer journal to move items to a new location in the warehouse
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

Exercise \#3 Adjusting stock levels using the inventory adjustment journal
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

Exercise \#4 Using the inventory counting journal to compare D365 inventory amounts to manually counted quantities
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

