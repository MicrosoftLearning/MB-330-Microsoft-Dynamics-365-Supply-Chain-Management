Exercise 1: Configure Intercompany relations
============================================

Set Up Action Policies
----------------------

You work for **USMF**, and now **USRT** needs the ability to buy products
through an Intercompany relationship from **USMF**. To facilitate this buy/sell
relationship, we need to create an Intercompany trading relationship between
customer **US-002** in **USMF** and vendor **9009** in **USRT**.

This Intercompany trading relationship will include action policies. Use the
following information to set up the appropriate action policies:

Purchase Order Action Policies:
-------------------------------

-   Original sales order (direct delivery)

    -   Post invoice automatically

    -   Print invoice automatically

-   Intercompany purchase order prices

    -   Allow price edit

    -   Allow discount edit

-   Intercompany purchase order =\> Intercompany sales order

    -   Sync customer information on the header

Sales Order Policies:
---------------------

-   Intercompany sales order creation

    -   Use “Company + original number” for the sales order numbering.

    -   Allow summary update of documents for original customer.

    -   Print picking list automatically.

-   Payment

    -   Use the **CustPay** payment journal

    -   Post journal automatically

-   Intercompany sales order prices

    -   Price and discount search

    -   Allow price edit

    -   Allow discount edit

-   Intercompany sales order =\> Intercompany purchase order

    -   Sync customer information on the header

Create a trading relationship with USMF vendor 9009.
----------------------------------------------------

1.  In company **USRT**, go to either the **Accounts payable** module or the
    **Procurement and sourcing** module.

2.  Then, go to **Vendors**, and then to **All vendors**.

3.  Click **NEW** to create a new vendor.

4.  In **Vendor account** field, under **IDENTIFICATION**, enter **9009**.

5.  In **Name** field, under **IDENTIFICATION**, select **Contoso Entertainment
    System USA** (use the filter) and click **Select** button. Use match if
    asked.

6.  In **Group** field, in **IDENTIFICATION** section, select Vendor group **90,
    Intercompany vendors**.

7.  On the **General** tab of the action pane, in the **SET UP** section, click
    **Intercompany**.

8.  Select **Trading relationship** tab.

9.  Under **ACTIVATION**, select **Yes** for Active.

10. Under **PURCHASE RELATION** section, **My Company** field will auto-populate
    with **USRT**. The **Vendor account** field will auto-populate with
    **9009**.

11. In **SALES RELATION** section, **Customer company** field, select **USMF.**
    In **My account** field, select **US-002**.

Configure the purchase order action policies.
---------------------------------------------

1.  Select **Purchase order policies** in the left navigation area.

2.  Select the **Post invoice automatically** checkbox in the **ORIGINAL SALES
    ORDER (DIRECT DELIVERY)** section.

3.  Select the **Print invoice automatically** checkbox in the **ORIGINAL SALES
    ORDER (DIRECT DELIVERY)** section.

4.  Select the **Allow price edit** checkbox in the **INTERCOMPANY PURCHASE
    ORDER PRICES** section.

5.  Select the **Allow discount edit** checkbox in the **INTERCOMPANY PURCHASE
    ORDER PRICES** section.

6.  Select the **Customer information on the header** checkbox in the **ORIGINAL
    SALES ORDER \<-\> INTERCOMPANY PURCHASE ORDER** section.

Configure the sales order action policies.
------------------------------------------

1.  Select **Sales order policies** in the left navigation area.

2.  Select **Company + original number** in the **Sales order numbering**
    drop-down list in the **INTERCOMPANY SALES ORDER CREATION** section.

3.  Select the **Allow summary update of documents for original customer**
    checkbox in the **INTERCOMPANY SALES ORDER CREATION** section.

4.  Select the **Print picking list automatically** checkbox in the
    **INTERCOMPANY SALES ORDER CREATION** section.

5.  Select **CustPay** in the **Payment journal** drop-down list in the
    **PAYMENT** section.

6.  Select the **Post journal automatically** checkbox in the **PAYMENT**
    section.

7.  Select the **Price and discount search** checkbox in the **INTERCOMPANY
    SALES ORDER PRICES** section.

8.  Select the **Allow price edit** checkbox in the **INTERCOMPANY SALES ORDER
    PRICES** section.

9.  Select the **Allow discount edit** checkbox in the **INTERCOMPANY SALES
    ORDER PRICES** section.

10. Select the **Customer information on the header** checkbox in the
    **INTERCOMPANY SALES ORDER -\> INTERCOMPANY PURCHASE ORDER** section.

11. Click **Save** button at top of screen.

Manage Order Agreement Action Policies
--------------------------------------

To facilitate this buy/sell relationship, we have created an Intercompany
trading relationship between customer **US-002** in **USMF** and vendor **9009**
in **USRT**.

This Intercompany trading relationship will include Purchase and sales agreement
policies.

Allow all options for the purchase and sales agreement policies.
----------------------------------------------------------------

1.  Open the **Intercompany** form for vendor Contoso Entertainment Europe:

2.  In **USMF,** go to either the **Accounts receivable** module or the **Sales
    and marketing** module.

3.  Then, go to **Customers**, and then to **All customers**.

4.  Click Account **US-002.**

5.  On the **GENERAL** tab of the action pane (you may need to hit the
    ellipsis), in the **SET UP** section, click **Intercompany**.

### Configure the purchase agreement policies.

1.  Select **Purchase agreement policies** in the left navigation area.

2.  Select the **Allow setting on hold/effective** checkbox in the
    **INTERCOMPANY PURCHASE AGREEMENT** section.

3.  Select the **Allow edit of validity period** checkbox in the **INTERCOMPANY
    PURCHASE AGREEMENT** section.

4.  Select the **Allow price edit** checkbox in the **INTERCOMPANY PURCHASE
    AGREEMENT PRICES** section.

5.  Select the **Allow discount edit** checkbox in the **INTERCOMPANY PURCHASE
    AGREEMENT PRICES** section.

### Configure the sales agreement policies.

1.  Select **Sales agreement policies** in the left navigation area.

2.  Select the **Allow setting on hold/effective** checkbox in the
    **INTERCOMPANY SALES AGREEMENT** section.

3.  Select the **Allow edit of validity period** checkbox in the **INTERCOMPANY
    SALES AGREEMENT** section.

4.  Select the **Allow price edit** checkbox in the **INTERCOMPANY SALES
    AGREEMENT PRICES** section.

5.  Select the **Allow discount edit** checkbox in the **INTERCOMPANY SALES
    AGREEMENT PRICES** section.

6.  Click **Save**.

Configure Value Mapping
-----------------------

Now you must define the value mapping for this relationship. Configure the
purchase and sales value mapping for the Intercompany trading relationship
between **USRT** and **USMF**, vendor **9009**.

### Create an external code.

1.  In **USRT**, go to **Procurement and sourcing\>Setup\>Distribution\>Modes of
    delivery**.

2.  Click **External codes** at top of form.

3.  Click **NEW** (if necessary) to create a new External code.

4.  Enter **USMF01** for **Code**, ‘Contoso Entertainment System,’ for
    **External code definition**, check **Standard code** checkbox, and enter
    ‘**USMF’** for **Description**.

5.  Under **VALUE** section enter **USMF1** in **Value** field.

6.  Click **Save**.

**In USRT, open the Intercompany form for vendor Contoso Entertainment System
USA.**

1.  Go to either the **Accounts payable** module or the **Procurement and
    sourcing** module.

2.  Then, go to **Vendors**, and then to **All vendors**.

3.  Select **Contoso Entertainment System USA** (vendor 9009).

4.  On the **General** tab of the action pane, in the **Set Up** section, click
    **Intercompany**.

### Configure the Purchase value mapping.

1.  Select **Purchase value mapping** in the left navigation area.

2.  Select **External code** in the drop-down list for **MODE OF DELIVERY
    CODE**.

3.  Select **USMF01** in the adjacent drop-down list.

4.  Select **Our** in the drop-down lists for:

    -   **Delivery terms codes**

    -   **Charges code**

    -   **Return reason code**

    -   **Disposition code**

    -   **Classification**

### Configure the Sales value mapping.

1.  Select **Sales value mapping** in the left navigation area.

2.  Select **External code** in the drop-down list for **MODE OF DELIVERY
    CODE**.

3.  Select **USMF01** in the adjacent drop-down list.

4.  Select **Our** in the drop-down lists for:

    -   **Delivery terms codes**

    -   **Charges code**

    -   **Return reason code**

    -   **Disposition code**

    -   **Classification**

### Save the Intercompany trading agreement.

1.  Click **Save** button.

Exercise 2: Process a purchase order-Initiated Intercompany chain
=================================================================

Create a Purchase Order-Initiated Intercompany Chain
----------------------------------------------------

You are the purchasing assistant in **USRT**, and you must purchase 10 units of
the new item **D0001** from the production plant **USMF**. You start the
Intercompany chain with a purchase order for a quantity of 10 units of **D0001**
from **USMF**.

In this exercise, you will perform updates in both USRT and the vendor company
USMF until the Intercompany purchase order is completely invoice-updated. In a
business scenario, the purchasing assistant would not typically perform updates
in both companies.

Create the Intercompany purchase order in USRT.
-----------------------------------------------

1.  Start in **USRT** and navigate to **Accounts Payable \> Purchase orders \>
    All purchase orders**. You can also access the **All purchase orders** form
    by navigating to **Procurement and sourcing \> Purchase orders \> All
    purchase orders**.

2.  Click **NEW** in the **All purchase orders** form to create a new purchase
    order.

3.  In the **Create purchase order form,** select Vendor account **9009**. In
    the **General tab,** in **Storage Dimensions**, verify **Site** = ‘1’ and
    **Warehouse** = ’11.’ Under **INTERCOMPANY**, verify **Intercompany** is set
    to ‘Yes.’

4.  Click the **OK** button.

5.  In **Purchase order lines**, add item number **D0001**.

6.  Verify the following: **Site 1**, **Warehouse 11**. In **Quantity** field
    enter ’10.’ **Unit price** should default to **240.08**.

7.  Click **Save**.

8.  Click **PURCHASE** on the action pane and, under **ACTIONS**, click
    **Confirm**, to confirm the purchase order.

9.  Close the Purchase order.

Verify the Intercompany sales order in USMF.
--------------------------------------------

1.  In **USMF**, navigate to **Sales and marketing\>Sales orders\>Intercompany
    orders.**

2.  Verify that the new Intercompany sales order was created. The prefix of
    sales order number is **usrt.**

3.  Double-click the Intercompany sales order.

4.  Verify the site and warehouse that you are trading from.

Generate Picking Lists, Packing Slips and Product Receipts
----------------------------------------------------------

You are the purchasing assistant in **USRT**, and you purchased 10 units of the
new item **D0001** from the production plant (**USMF**).

You have started the Intercompany chain with a purchase order for a quantity of
10 units of **D0001** from **USMF**.

### Generate the packing slip and product receipt associated with this purchase order.

1.  In **USMF**, navigate to **Sales and marketing \> Sales orders \>
    Intercompany orders.**

2.  Select the Intercompany sales order to generate the packing slip.

3.  In the **PICK AND PACK** tab of the action pane, under the **GENERATE**
    group, click **Generate picking list.**

4.  In the **Posting picking list** form, under **PARAMETER,** verify **All** is
    selected in the **Quantity** field.

5.  Click the **OK** button. Click **OK** when prompted to post document without
    printing it.

6.  On sales order form, in the **PICK AND PACK** tab of the action pane, under
    the **GENERATE** group, click **Post packing slip.**

7.  In the **Packing slip posting** form under **PARAMETER,** verify **Picked**
    is selected in the **Quantity** field.

8.  Click the **OK** button. Click **OK** if prompted to post document without
    printing it.

9.  In the **INTERCOMPANY ORDERS** form, verify sales order status is updated to
    **Delivered.**

### Generate a product receipt

1.  In **USRT** navigate to **Procurement and sourcing \> Purchase orders \> All
    purchase orders**:

2.  Select the Intercompany purchase order to generate the product receipt.

3.  In the **RECEIVE** tab of the action pane, under the **GENERATE** group,
    click **Product receipt**.

4.  In the **Posting product receipt** form, under **PARAMETERS,** verify
    **Ordered quantity** is selected in the **Quantity** field.

5.  Click **OK,** at bottom of form.

6.  In the **Purchase order** form, verify purchase order status is updated to
    **Received.**

Generate Invoices
-----------------

Now you need to generate the sales order invoice in **USMF** and then post the
purchase order invoice in **USRT**, associated with this Intercompany sales
order.

### Generate the sales order invoice in USMF.

1.  Navigate to **Sales and marketing \> Sales orders \> Intercompany orders**

2.  Select the Intercompany sales order to generate the invoice.

3.  In the **INTERCOMPANY ORDERS** form, click the **INVOICE** tab. Under the
    **GENERATE** group, click **Invoice.**

4.  In the **Posting invoice** form, under **PARAMETER**, verify **Packing
    slip** is selected in the **Quantity** field.

5.  Verify the information in the **Lines** FastTab, and then click the **OK**
    button.

6.  Click **OK** when prompted to post document without printing it.

7.  In the **INTERCOMPANY ORDERS** form, verify sales order status has been
    updated to **Invoiced.**

### Post the purchase order invoice in USRT.

1.  Navigate to **Procurement and sourcing \> Purchase orders \> All purchase
    orders**.

2.  Select the Intercompany purchase order to generate the invoice.

3.  In the **INVOICE** tab of the action pane, under the **GENERATE** group,
    click **Invoice.**

4.  In the **VENDOR INVOICE** form **Lines** section, under **INVOICE DATES**,
    enter an invoice date in the **Invoice date** field.

5.  From the action pane, click the **Match product receipts** button to match
    the product receipts to the invoice.

6.  In the **Match product receipts to invoice** form, click the **OK** button
    at the bottom of the screen.

7.  To finish, click **Post** on the action pane, and the invoice posts.

8.  In the **ALL PURCHASE ORDERS** form, verify purchase order status is updated
    to **Invoiced.**

Exercise 3: Process a sales order-Initiated Intercompany chain
==============================================================

Create a Sales Order-Initiated Intercompany Chain
-------------------------------------------------

Contoso Retail Miami **3005** has ordered items from **USRT**. Unfortunately,
there is no on-hand inventory available. Therefore, these items must be ordered
from **USMF**.

An original sales order for Northwind Traders customer is created. The sales
representative creates a purchase order directly from the Sales order form.
Because an Intercompany vendor 9009 (which is linked to the USMF company through
the Intercompany setup), is set up as a standard vendor for the ordered item, an
Intercompany sales order is created in USMF company account for customer 3005
(which is the customer in the USMF company that is linked to the USRT company
through the Intercompany setup).

Create a sales order-initiated Intercompany chain.
--------------------------------------------------

1.  Start in **USRT** and navigate to **Modules** \> **Sales and marketing \>
    Common \> Sales orders \> All sales orders**.

2.  Click **NEW** on the action pane to create a new sales order.

3.  Select Customer account **3005 Contoso Retail Miami** in the **Create sales
    order** form.

4.  Click the **OK** button, in the **Create sales order** form.

5.  In **Sales order lines**, select the item to be sold, item **D0001**, in the
    **Item number** drop-down.

6.  Type the value “4” in the **Quantity** field.

7.  **Site 1** and **Warehouse 11** should default.

8.  **Unit price** of **329.00** should default. Click the **Save** button to
    save the sales order.

9.  Select the **SALES ORDER** tab.

10. Click **Purchase order,** in the **NEW** group of the action pane.

11. Select the **Include** checkbox in the line with the item.

12. Verify that vendor **9009** is selected in the **Vendor account** field.

13. Click **OK**. ‘Automatic purchase creation’ message should appear.

14. Message indicating Intercompany sales order was created should appear.

15. Message indicating purchase order was created should appear.

16. Close all pages.

Process the Intercompany Purchase Order
---------------------------------------

This Intercompany sales order must now be processed. As part of the sales order
processing, update the ordered quantity to **4.00.**

Process the Intercompany sales order for customer US-002 in USMF.
-----------------------------------------------------------------

1.  Navigate to **Sales and marketing \> Sales orders \> Intercompany orders**.

2.  Select the Intercompany order (e.g., usrt000183) to packing slip update.

3.  Click the **PICK AND PACK** tab in the **Sales order** form.

4.  Under the **GENERATE** group, click **Post packing slip**.

5.  Under the **PARAMETER** group, verify **Packing slip** is selected in the
    **Quantity** field.

6.  Quantity of **4.00** should default in **Lines** section **Update** field.

7.  Click **OK** button, and click **OK** when prompted to post document without
    printing it.

8.  Verify sales order status has been updated to **Delivered.**

Process the original sales order for customer Northwind Traders in USRT.
------------------------------------------------------------------------

1.  Navigate to **Sales and marketing \> Sales orders \> All sales orders.**

2.  Select the sales order for customer Northwind Traders (e.g., 000183).

3.  In the action pane, click **PICK AND PACK**. Under **GENERATE,** click
    **Post packing slip**.

4.  In the **Packing slip posting** form **PARAMETER** group, verify **Packing
    slip** is selected in the **Quantity** field.

5.  In the **Packing slip posting** form, verify the quantity of **4.00**
    defaults in the **Lines** section **Update** field.

6.  Click **OK** button, and click **OK** when prompted to post document without
    printing it.

7.  Verify sales order status is updated to **Delivered.**

Manually Create an Intercompany Chain
-------------------------------------

USRT's customer, Football Stadium (1002), calls and orders two units of item
number D0001.

Because **USRT** has no on-hand inventory available for this item, you must
create an Intercompany purchase order from the Intercompany vendor 9009
**USMF**.

Create the Intercompany purchase order in USRT.
-----------------------------------------------

1.  Navigate to **Accounts Payable \> Purchase orders \> All purchase orders**.

2.  Click **NEW** in the **All purchase orders** form to create a new purchase
    order.

3.  In the **Create purchase order** form, select Vendor account **9009.** In
    the **General** tab Storage Dimensions, verify **Site** = ‘1’ and
    **Warehouse** = ’11.’ Under **INTERCOMPANY**, verify **Intercompany** is set
    to **Yes**.

4.  Click the **OK** button.

5.  In **Purchase order lines,** add item number **D0001**.

6.  Verify the following: Site 1, Warehouse 11. In the **Quantity** field, enter
    ’10.’.

7.  Click **Save.**

8.  Click **PURCHASE** on the action pane and, under **ACTIONS**, click
    **Confirm** to confirm the purchase order.

9.  Close the Purchase order.

10. In **USMF**, navigate to **Sales and marketing \>Sales orders \>
    Intercompany orders**.

11. Verify that the new Intercompany sales order was created.

Update the Intercompany sales order packing slip in USMF.
---------------------------------------------------------

1.  Start in **USMF** and navigate to **Modules** \> **Sales and marketing \>
    Sales orders \> Open orders \> Intercompany orders.**

2.  Select the Intercompany sales order to generate the packing slip.

3.  In the **PICK AND PACK** tab of the action pane, under the **GENERATE**
    group, click **Generate picking list.**

4.  In the **Posting picking list** form, under **PARAMETER,** verify **All** is
    selected in the Quantity field.

5.  Click the **OK** button. Click **OK** when prompted to post document without
    printing it.

6.  On sales order form, in the **PICK AND PACK** tab of the action pane, under
    the **GENERATE** group, click **Post packing slip.**

7.  In the **Packing slip posting** form, under **PARAMETER,** verify **Picked**
    is selected in the **Quantity** field.

8.  Click the **OK button**. Click **OK**, if prompted to post document without
    printing it.

9.  In **INTERCOMPANY ORDERS** form, verify sales order status is updated to
    **Delivered.**

Update the purchase order packing slip in USRT.
-----------------------------------------------

1.  Start in **USRT** and navigate to **Modules \> Procurement and sourcing \>
    Purchase orders \> All purchase orders**:

2.  Select the Intercompany purchase order to generate the product receipt.

3.  In the **RECEIVE** tab of the action pane, under the **GENERATE** group,
    click **Product receipt**.

4.  In the **Posting product receipt** form, under **PARAMETERS,** verify
    **Ordered quantity** is selected in the **Quantity** field.

5.  Click the **OK** button at bottom of form.

6.  In the **Purchase order** form, verify purchase order status is updated to
    **Received.**

Update the Intercompany sales order invoice in USMF.
----------------------------------------------------

1.  Start in **USMF**, and navigate to **Modules \> Sales and marketing \> Sales
    orders \> Open orders \> Intercompany orders.**

2.  Select the Intercompany sales order to generate the invoice.

3.  In the **INTERCOMPANY ORDERS** form, click the **INVOICE** tab. Under the
    **GENERATE** group, click **Invoice.**

4.  In the **Posting invoice** form, under **PARAMETER**, verify **Packing
    slip** is selected in the **Quantity** field.

5.  Verify the information in the **Lines** FastTab (i.e., Site = 1, Warehouse =
    13, Update = 10), and then click the **OK** button.

6.  Click **OK** when prompted to post document without printing it.

7.  In the **INTERCOMPANY ORDERS** form, verify sales order status has been
    updated to **Invoiced.**

Update the purchase order invoice in USRT.
------------------------------------------

1.  Navigate to **Procurement and sourcing \> Purchase orders \> All purchase
    orders**.

2.  Select the Intercompany **Purchase order** to generate the invoice.

3.  In the **INVOICE** tab of the action pane, under the **GENERATE** group,
    click **Invoice.**

4.  In the **VENDOR INVOICE** form **Lines** section, under **INVOICE DATES**,
    enter an invoice date in the **Invoice date** field.

5.  From the action pane, click the **Match product receipts** button to match
    the product receipts to the invoice.

6.  In the **Match product receipts to invoice** form, click the **OK** button
    at the bottom of the screen.

7.  To finish, click **Post** on the action pane, and the invoice posts.

8.  In the **ALL PURCHASE ORDERS** form, verify purchase order status is updated
    to **Invoiced.**

Auto-Create an Intercompany Order
---------------------------------

Football Stadium **1002** is the only customer who orders the item number
**D0001** (MidRangeSpeaker). You have no on-hand inventory available, and must
purchase this item from your Intercompany vendor **9009**.

Set up the customer for the automatic creation of Intercompany orders.
----------------------------------------------------------------------

1.  Start in **USRT**, and navigate to **Modules \> Sales and marketing \>
    Customers \> All customers,** and select Account **1002 Football Stadium.**

2.  In the **Miscellaneous details** FastTab, under the **AUTOMATIC NOTIFICATION
    AND CANCELLATION PROCESSING** group, verify **Yes** is selected for **Create
    Intercompany orders** and **Yes** is selected for **Direct delivery**.

Set up a primary vendor for item D0001.
---------------------------------------

1.  Navigate to **Product information management \> Customers \> All
    customers,** and select Account **1002 Football Stadium.**

2.  In the **RELEASED PRODUCT DETAILS** form, click the **Edit** button, and go
    to the **Purchase** FastTab.

3.  Under the **ADMINISTRATION** group, in the **Vendor** field, select
    **9009**.

4.  Click the **Save** button to save the changes.

Automatically create the Intercompany chain.
--------------------------------------------

1.  In **USRT** navigate to **Sales and marketing \> Sales orders \> All sales
    orders**.

2.  Click the **NEW** button on the action pane to create a new sales order.

3.  Select Customer account **1002 Football Stadium,** in the **Create sales
    order** form.

4.  Click the **OK** button in the **Create sales order** form.

5.  In **Sales order lines**, select the item to be sold, item **D0001**, in the
    **Item number** drop-down.

6.  Type the value “4” in the **Quantity** field.

7.  **Site** 1 and **Warehouse** 11 should default.

8.  **Unit price** field value should default. Click the **Save** button to save
    the sales order.

9.  Select the **SELL** tab. Under **GENERATE,** click **Confirm sales order**.
    Click **OK,** in the **Confirm sales order** form. Click **OK** when
    prompted to post without printing.

10. Notification in **MESSAGES** displays, stating “Intercompany sales order
    usrtXXX has been created.”

11. Notification in **MESSAGES** displays, stating “Purchase order 0000XX has
    been created.”

12. In **USRT**, navigate to **Accounts payable \> Purchase orders \> All
    purchase orders**. Verify a new purchase order for vendor **9009** has been
    created for **4.00 pieces** of **item D0001**.

13. In **USMF**, navigate to **Sales and Marketing \> Sales orders \> All sales
    orders \>Intercompany orders**.

14. Verify new Intercompany order has been created for customer **US-002** for
    **4.00** pieces of item **D0001**.

Set Up an Intercompany Chain with Automatic Picking List Creation
-----------------------------------------------------------------

The sales company **USMF** and the production company **USRT** are working
closely together. After you create a new Intercompany chain, the picking
procedure in **USMF** must be started without any manual interaction. Therefore,
the picking list must be generated and printed automatically.

Create an Intercompany chain with automatic picking and printing of picking list
--------------------------------------------------------------------------------

1.  In **USMF**, navigate to **Sales and Marketing \> Customers \> All
    customers**.

2.  Select the Customer account, **USRT US-002**.

3.  Click **Edit**.

4.  In the **ALL CUSTOMERS** form **GENERAL** tab, under the **SET UP** group,
    click **Intercompany** on the action pane.

5.  Click **Sales order policies.**

6.  Select the **Print picking list automatically** parameter and click
    **Save**.

7.  In **USMF,** navigate to **Accounts receivable \> Setup \> Accounts
    receivable parameters.**

8.  Click **General.** In **Sales default values**, select **Automatic** in the
    **Reservation** field.

9.  In the **Accounts receivable parameters** form, click **Updates.** In the
    **Picking list** FastTab, select **Completed** for the **Picking route
    status.**

Create a sales order line item.
-------------------------------

1.  In **USMF**, navigate to **Sales and Marketing \> Sales Orders** \> **All
    sales orders.**

2.  Click **New** to create a new sales order.

3.  In the **Create sales order** form, select Customer account **US-002**.

4.  In the **General** FastTab, verify **Yes** is selected, under the
    **INTERCOMPANY** group.

5.  In the **Sales order lines** on the **SALES ORDER** form, select **D0001**
    in the **Item number** field. **Quantity** should default to 1.00.

6.  Click **Header**. In the **Intercompany settings** FastTab, select **Yes**
    for **Autocreate Intercompany orders** and **Yes** for **Direct delivery**.

7.  On the **SELL** tab, under the **GENERATE** group, click **Confirm sales
    order.** Click the **OK** button in the **Confirm sales order** form, and
    click **OK** when prompted, to post without printing.

8.  On **PICK AND PACK** tab, under the **GENERATE** group, select **Generate
    picking list.**

9.  Click the **OK** button in the **Posting picking list** form.

10. A notification appears stating that an Intercompany purchase order has been
    created in **USRT**

**Work with the Intercompany On-Hand Form**

Football Stadium (1002) is the only customer who orders the item number D0001
(MidRangeSpeaker). **USRT** needs to know the amount of their own on-hand
inventory, as well as the on-hand inventory with their Intercompany vendor
Contoso Entertainment Systems USA (9009).

View the company’s on-hand inventory in the Intercompany chain, for all item and
inventory dimensions

1.  Navigate to **Inventory management \> Inquiries and reports \> On-hand
    list**.

2.  Filter by item number D0001 and click the **Apply** button.

3.  Click **Intercompany on-hand** button.

4.  Physical inventory, Physical reserved, Available physical, Total available,
    etc., is displayed for **USRT** and **USMF.**

Configure Intercompany Information Flow
---------------------------------------

A representative from Football Stadium 1002 has called and inquired about the
status of the order, so you must view the status of the corresponding sales or
purchase order, to determine whether it has already been picked or delivered or
received

View related orders.

1.  In **USRT**, navigate to **Sales and marketing \> Sales orders \> All sales
    orders**.

2.  Open the desired Sales order

3.  Select the **MANAGE** tab.

4.  Under the **INTERCOMPANY TRACKING** group, select either **Intercompany
    sales order** or **Purchase order.**
