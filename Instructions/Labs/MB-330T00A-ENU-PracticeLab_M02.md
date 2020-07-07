Exercise 1: Use Movement journals
=================================

In **USMF**, you need to update the on-hand inventory manually using an
Inventory movement journal.

It’s also possible to update on-hand inventory by importing transactions in data
entities.

Initialize stock levels in the warehouse
----------------------------------------

1.  Go to **Inventory management \> Journal entries \> Items \> Movement**.

2.  Click **New**.

3.  In the **Name** field, click the drop-down button to open the lookup.

4.  Select **Imov**. It’s a good practice to use different journal name
    templates for the different business purposes.

5.  In the **Offset account** field, specify the values '140200'. This is the
    offset account that will be the default account on the journal lines. It’s
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

Exercise 2: Use Inventory adjustment journals
=============================================

As a warehouse manager in **USMF**, you need to adjust stock levels of products
in the warehouse.

Adjust stock levels in the warehouse
------------------------------------

1.  Go to **Inventory management \> Journal entries \> Items \> Inventory
    adjustment**.

2.  Click **New**.

3.  In the **Name** field, click the drop-down button to open the lookup.

4.  In the list, click on the inventory adjustment journal name you want to use.
    Some other fields will be populated based on the setup of the inventory
    adjustment journal name you select.

5.  Click **OK**.

6.  Click **New** in the **Journal lines** fast tab.

7.  In the **Item number** field, Select 'D0001'.

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

Exercise 3: Use transfer journals
=================================

As a warehouse employee in **USMF**, you need to perform the process of creating
and posting an inventory transfer journal in order to register movement of an
item from one location in a warehouse to another.

Transfer physical inventory within the warehouse.
-------------------------------------------------

1.  Go to **Inventory management\>Journal entries\>Items\>Transfer**.

2.  Click **New**.

3.  In the **Name** field, enter or select **ITrf**.

4.  Click **OK**.

There is the option to specify 'From' and 'To' dimensions for each journal line.
These are essential for this journal type. You can transfer items to locations
using different rules. In this example we’ll transfer an item within the same
warehouse, from a license plate-controlled location to a location that is not
license plate controlled.

1.  Click **New** in the **Journal lines** fast tab.

2.  In the **Item number** field, enter or select 'A0001'.

3.  In the **From site** field, enter or select '2'.

4.  In the **To site** field, enter or select '2'.

5.  In the **From warehouse** field, enter or select '24'.

6.  In the **To warehouse** field, enter or select '24'

7.  In the **From location** field, enter or select 'FL-001'.

8.  In the **To location** field, enter or select 'BULK-001'.

9.  In the **Quantity** field, enter a number.

10. Click the **Inventory dimensions** tab in the **Line details** fast tab.

11. In the **License plate** field in both the **From inventory dimensions** and
    **To inventory dimensions** groups, enter or select '24'

12. Click **Save**.

13. Click **Post**.

14. Click **OK**.

15. Click **Inventory** in the Journal lines fast tab.

16. Click **Transactions** to see the transfer.

17. Close all pages.

Exercise 4: Use counting journals
=================================

As a warehouse worker in **USMF**, you need to perform the process of creating
and posting an inventory counting journal in order to count a specific item at a
location in the warehouse.

1.  Go to **Inventory management \> Journal entries \> Item counting \>
    Counting**.

2.  Click **New**.

3.  In the **Name** field, click the drop-down button to open the lookup.

4.  In the list, click on the inventory counting journal Icnt. Some other fields
    will be populated based on the setup of the inventory counting journal name
    that you select.

5.  In the **Worker** field, click the drop-down button to open the lookup.

6.  In the list, select the worker you want to use.

7.  Click **Select**.

8.  Click **OK**.

9.  Click **New** in the **Journal lines** fast tab.

10. In the **Item number** field, click the drop-down button to open the lookup.

11. In the list, find and select 'A0001'.

12. In the **Site** field, click the drop-down button to open the lookup.

13. In the list, find and select site '2'.

14. In the **Warehouse** field, click the drop-down button to open the lookup.

15. In the list, find and select warehouse '24'.

16. In the **Location** field, click the drop-down button to open the lookup.

17. In the list, find and select location 'BULK-001'

18. In the **Counted** field, enter a number.

19. If you enter a counted number that’s different than the number shown in the
    **On-hand** field, the **Quantity** field is updated to show the
    discrepancy.

20. Click **Save**.

21. Click **Post**. When you post an inventory counting journal, if the counted
    amount differs from amount that’s reported in the On-hand field an inventory
    receipt or issue is posted, the inventory level and value are changed, and
    ledger transactions are generated.

22. Click **OK**.

23. Close all pages.
