---
lab:
    title: 'Case study 2A Procurement and sourcing '
    module: 'Module 3: Implement and manage supply chain processes '
---

Case study 2A Procurement and sourcing
======================================

Objectives
----------

-   *Create a purchase requisition using a procurement category and then submit
    and approve the purchase requisition*

-   *Create a request for quotation, reply and accept a vendor’s reply.*

-   *Create a purchase requisition permission policy with a new requester name
    and create an office supplies purchasing policy.*

-   *Create a purchase order for two different items, each to be delivered to a
    different site.*

-   *Create a charge code for vendor transport charges on various items.*

-   *Create a vendor charge group and assign it to two vendors.*

-   *Create an item charges group and use it to create an automatic charge.*

-   *Set up change management so purchase orders are approved prior to
    confirmation.*

-   *Create a purchase order from on a trade agreement based on value or
    quantity.*

-   *Create a trade agreement for domestic vendors that specifies a fixed price
    for a certain item.*

-   *Create a guest user for a supplier so they can access the system.*

Exercise \#1 Create, submit, and approve a purchase requisition
---------------------------------------------------------------

*Objective: Create a purchase requisition using a procurement category and then
submit and approve the purchase requisition.*

An employee of the IT department of USMF wants a longer HDMI cables for the new
office and meeting rooms. a purchase requisition will have to go through the
internal approval process before the items are purchased.

The employee must identify a vendor for the request and the quantity required.
The employee do not know the actual part number, so you will use a procurement
category instead.

**The IT employee asked you to help. What system features you would show and
help her to use?**

### Create and process a purchase requisition

1.  Go to **Procurement and sourcing**, then to **Purchase requisitions**, and
    then to **All purchase requisitions**.

2.  Click **New**.

3.  Name: Enter **New HDMI Cables**.

4.  Click **OK**.

5.  Reason: Select **General** (General supplies).

6.  Details: Enter **New, longer HDMI cables**.

### Add an item to the purchase requisition.

1.  Click **Add products** in the **Purchase requisition lines** FastTab.

2.  Select the **Computers** procurement category (a subcategory of Office
    Machines).

3.  Click **Add unlisted product to lines**.

4.  Product name: Enter **24in HDMI Cable**.

5.  Unit: Enter **ea**.

6.  Click **OK**.

7.  Change to the **Line details** tab.

8.  Product name: enter **24-inch HDMI cable**.

9.  Quantity: Enter **5**.

10. Unit price: Enter **41.49**.

11. Vendor Account: Select **1001** (Acme Office Supplies).

12. Click **OK**.

13. Click **Save**.

### Submit the purchase requisition created in the previous practice for approval, and perform the approval process.

1.  Go to **Procurement and sourcing**, then to **Purchase requisitions**, and
    then to **All purchase requisitions**.

2.  Open the draft purchase requisition created in the previous practice.

3.  Click **Workflow** at the top, and then click **Submit**.

4.  Comment: Enter **Request for longer HDMI cables.**

5.  Click **Submit**.

6.  Click **Workflow\>Workflow history**

7.  Click **Refresh a** few times and wait until the work items shows records.

8.  Click **Reassign** button.

9.  Select **Admin** in the **User field.**

10. Click **Reassign**.

11. Click **Refresh.**

12. Close the **Workflow history** page.

### Approve the purchase requisition.

1.  Click **Workflow** at the top, and then click **Approve**.

2.  Comment: Enter **Approved.**

3.  Click **Approve**

Exercise \#2 Create, reply and accept a request for quotation (Bonus)
---------------------------------------------------------------------

*Objective: Create a request for quotation, reply and accept a vendor’s reply.*

After the Purchase requestion was approved, the Procurement department found
that there were a lot of other requests for the same type of cables, so they
have decided to buy a larger quantity to benefit from bulk pricing.

The purchase clerk must create and process a request for quotation for a
quantity of 500 of A0001 HDMI 6 foot cables that will be sent to two different
vendors, US-111 (Contoso Office Supply) and US-103 (Rain Projectors), and it
should be set to update vendor replays in order to choose the best offer.

You will have to do the following:

-   Create the request for quotation and send to the appropriate suppliers

-   Add a line to the request for quotation.

-   Reply to a request for quotation.

-   Accept a vendor’s reply.

### Create the request for quotation and send to the appropriate suppliers.

1.  Go to **Procurement and sourcing**, then to **Requests for quotations**, and
    then to **All requests for quotations**.

2.  Click **New**.

3.  Purchase type: Select **Purchase order**.

4.  Document title: Enter **HDMI Cables**.

5.  Site: Select **1** (Home speakers production).

6.  Warehouse: Select **13** (Site 1 – Finished Goods).

7.  Click **OK**.

### Add a line to the request for quotation.

1.  If necessary, click **Add line** to add a line to the list.

2.  Line type: Select **Item**.

3.  Item number: Select **A0001** (HDMI 6’ Cables).

4.  Quantity: Enter **500**.

5.  Click **Save**.

6.  Send the request for quotation to the vendors.

7.  Click **Options** at the top, click **Change view**, and then select
    **Header view**.

8.  Open the **Vendor** FastTab.

9.  If necessary, click **Add** to add a line to the list.

10. Vendor account: Select **US-111** (Contoso office supply).

11. Click **Add**.

12. Vendor account: Select **US-103** (Rain Projectors).

13. Click **Save**.

14. Click **Quotation** at the top, and then select **Send** under the
    **Process** section.

15. Make sure both vendors appear.

16. Click **OK**.

### Reply to a Request for Quotation

Update the request for the quotation created in the previous practice with the
vendor responses.

1. Make sure that the permission to edit vendor bids is setup. Go to the **Procurement and sourcing** module, then to **Setup**, and then to **Procurement and sourcing parameters**. On the **Request for quotations** tab, set the **Purchaser can edit vendors bid** option to **Yes**. Select **Save** 

### Process the quotation for US-103. Enter the vendors’ replies to the request for quotation. 

1.  Go to the **Procurement and sourcing** module, then to **Requests for
    quotations**, and then to **All requests for quotations**.

2.  Open the request for quotations created in the previous practice.

3.  Click **Header**.

4.  Click the **Vendor** FastTab.

5.  Click the **Request for quotation** number for **US-111** (Contoso office
    supply).
    
6. Select the **Edit** at the top, from the drop-down menu select **Edit RFQ reply**  

7.  Quantity: Enter **500**.

8.  Unit: Enter **ea**.

9.  Unit price: Enter **10.00**.

10.  Click **Save**.

11. Close the **Request for Quotation Reply** form.

12. Click the **Request for quotation** number for **US-103** (Rain Projectors).

13. Navigate back to **Vendor** FastTab. Click the **Request for quotation** number for **US-103** (Rain Projectors). Select the **Edit** at the top, from the drop-down menu select **Edit RFQ reply**

14. Quantity: Enter **500**.

15. Unit: Enter **ea**.

16. Unit price: Enter **8.00**.

17. Click **Save**.

18. Close the **Request for Quotation Reply** form.

### Accept a vendor’s reply.

1.  Go to the **Procurement and sourcing** module, then to **Requests for quotations**, and then to **All requests for quotations**.

2.  Open the request for quotations created in the previous practice.

3.  Click **Options** at the top, click **Change view**, and then select
    **Header view**.

4.  Click the **Vendor** FastTab.

5.  Click the **Request for quotation** number for **US-103** (Rain Projectors). 

6.  Select the **Edit** at the top, from the drop-down menu select **Edit RFQ reply**

7.  Select **Submit** form the top menu.

8.  Select **Accept** under the **Process** section.

9.  Click **OK**.

Exercise \#3 Create purchase requisition and purchasing policies (Bonus)
------------------------------------------------------------------------

*Objective:  Create a purchase requisition permission policy with a new
requester name and create an office supplies purchasing policy.*

The purchasing manager decided to make some updates.

He wants to update the requisitions permission policy with a new requester name
and create a new purchasing policy for office supplies with an additional
category.

He reached out for help and you will have to do the following:

-   Create a purchase requisition permission policy.

-   Create a purchasing policy.

### Create a purchase requisition permission policy.

1.  Go to **Procurement and sourcing**, then to **Setup**, then to **Policies**,
    and then to **Purchase requisition permissions**.

2.  Select **Mike Danseglio** in the list of workers.

3.  Change to the **Requester** FastTab.

4.  Click **Add**.

5.  Name: Search for **Susan Burk** and then **Select**.

6.  Click **Save**.

### Create a purchasing policy

1.  Go to the **Procurement and sourcing** module, then to **Setup**, then to
    **Policies**, and then to **Purchasing policies**.

2.  Click **Procurement Policy USMF**.

3.  Click the **Policy rules** FastTab.

4.  Click **New**, then **Policy**.

5.  Name: Enter **Office Supplies**.

6.  Description: Enter **Office supplies policies**.

7.  Policy rule type: Select **Category access policy rule**.

8.  Click **Create policy rule** in the **Policy rules** section on the right.

9.  Select **Office and Desk Accessories** in the **Available Categories** list.

10. Click the right arrow button.

11. Click **OK**.

12. Click **Save**.

Exercise \#4 Create a purchase order for delivery to multiple sites
-------------------------------------------------------------------

*Objective: Create a purchase order for two different items, each to be
delivered to a different site.*

The purchasing clerk at USMF wants to create one purchase order for a quantity
of 5 of item T0003 (surround sound receiver) from Acme Office Supplies, to be
delivered today to Site 1, and a quantity of 5 of item M1101 (foam reacting
agent) to be delivered to the Quality Testing Center, 123 W. Cherry Street, zip
code 83642.

He is not clear how to perform this using the system and asking your help

**What would you do?**

### Create a purchase order

1.  Go to the **Procurement and sourcing** module, then to **Purchase orders**,
    and then to **All purchase orders**.

2.  Click **New**.

3.  Vendor account: Select **1001** (Acme Office Supplies).

4.  Delivery date: Expand the **General** tab, verify the current date in the **Delivery date** field (this
    should be the default value). 

5.  Click **OK**.

6.  Add items to the purchase order:

    1.  Item number: Select **T0003** (SurroundSoundReceive).

    2.  Quantity: Enter **5**.

    3.  Unit: Enter **ea**.

    4.  Click **Add line**.

    5.  Item number: Select **M1101** (Foam reacting agent).

    6.  Quantity: Enter **5**.

    7.  Unit: Enter **PL**.

7.  Select delivery addresses for the items:

    1.  Select the line for item **T0003** (SurroundSoundReceive) in the
        **Purchase order lines** FastTab.

    2.  Open the **Line details** FastTab.

    3.  Change to the **Address** tab.

    4.  Delivery address: Select **Contoso Entertainment System USA**.

    5.  Select the line for item **M1101** (Foam reacting agent) in the
        **Purchase order lines** FastTab.

    6.  Change to the **Line details** FastTab.

    7.  Click the **Add address** button (**+**) to the right of the Delivery
        address field.

    8.  Name or description: Enter **Quality Testing Center**.

    9.  Zip/postal code: Enter **83642**.

    10. Street: Enter **123 W. Cherry Street**.

    11. Click **OK**.

8.  Click **Save**.

9.  On the Action pane, click **Purchase**

10. Click **Actions > Confirm**.

9.  On the Action Pane, click **Receive**.

10. Click Generate \> **Product receipt**.

11. Change Quantity to Registered quantity.

12. In the **Product receipt** field, enter the product receipt number. For
    example, enter **PR123**.

13. Click **OK** to post the product receipt.

14. Close all pages.

Exercise \#5 Create a charges code
----------------------------------

*Objective:  Create a charge code for vendor transport charges on various
items.*

The accounts payable coordinator at Contoso Entertainment Systems USA must
complete some setups for transport charges added to various items by the vendor.

She can do this in the system by creating a charges code with the following
specifications:

-   Name of the charges code: TRANSTO

-   Description: Transportation Fee to our sites

-   Account: 411400

-   This fee does not require an item sales tax group.

>   **She asked for your help to show her how this charges can be configured.
>   What would you do?**

### Create a charges code

1.  Go to the **Accounts payable** module, then to **Charges setup**, and then
    to **Charges code**.

2.  Click **New**.

3.  Charges code: Enter **TRANSTO**.

4.  Description: Enter **Transportation Fee to our sites**.

5.  Change to the Debit section.

6.  Type: Select **Ledger account**.

7.  Posting: Select **Payment fee**.

8.  Account: Select **411400**.

9.  Change to the Credit section.

10. Type: Select **Customer/Vendor**.

11. Click **Save**.

Exercise \#6 Create a vendor charges group and assign to vendors (Bouns)
------------------------------------------------------------------------

*Objective:  Create a vendor charge group and assign it to two vendors.*

The accounts payable administrator at Contoso Entertainment Systems USA, wants
to make updates for Fabrikam supplier, that has two vendor accounts from which
Contoso purchases items.

Fabrikam recently imposed an additional 15 percent freight charges for all
purchase orders.

He is not sure how to set up a new charges and not quite sure how to assign to
the supplier accounts.

You will have to do the following:

-   Create a vendor charges group.

-   Update vendors to use the new vendor charges group

### Create a Vendor Charges Group

1.  Go to the **Accounts payable** module, then to **Charges setup**, and then
    to **Vendor charges group**.

2.  Click **New**.

3.  Charges group: Enter **06**.

4.  Description: Enter **Freight 15%**.

5.  Click **Save**.

### Update vendors to use the new vendor charges group.

1.  Go to the **Accounts payable** module, then to **Vendors**, and then to
    **All vendors**.

2.  Open the vendor record for vendor **US-101** (Fabrikam Electronics).

3.  Click **Edit**.

4.  Open the **Purchase order defaults** FastTab.

5.  Charges group: Select **06** (Freight 15%).

6.  Click **Save**.

7.  Close the vendor record.

8.  Open the vendor record for vendor **US-104** (Fabrikam Supplier).

9.  Click **Edit**.

10. Open the **Purchase order defaults** FastTab.

11. Charges group: Select **06** (Freight 15%).

12. Click **Save**.

13. Close the vendor record

Exercise \#7 Create an automatic charge (Bonus)
-----------------------------------------------

*Objective:  Create an item charges group and use it to create an automatic
charge.*

The accounts payable coordinator at Contoso Entertainment Systems USA, wants to
make updates to vendor charges.

Datum Receivers (US-105) applies a 15 percent freight charge for all orders due
to the large quantity and weight of items we buy.

Since this charge only applies to US-105 and it will apply to every order, you
need to help the coordinator to set up an automatic charge for vendor group (06)
and the item charges group (123).

You will have to do the following:

-   Create an item charges group.

-   Create an automatic charge.

### Create an item charges group

1.  Go to the **Accounts payable** module, then to **Charges setup**, and then
    to **Item charge groups**.

2.  Click **New**.

3.  Charges group: Enter **123**.

4.  Description: Enter **15% Freight Charge**.

5.  Click **Save**.

### Create an automatic charge

1.  Go to the **Accounts payable** module, then to **Charges setup**, and then
    to **Automatic charges**.

2.  Level: Select **Line**.

3.  Click **New**.

4.  Account code: Select **Group**.

5.  Vendor relation: Select **06** (Freight 15%).

6.  Item code: Select **Group**.

7.  Item Relation: Select **123** (15% Freight Charge).

8.  Click **Save**.

9.  Click **Add** in the **Lines** FastTab.

10. Charges code: Select **TRANSTO** (Transportation Fee).

11. Category: Select **Percent**.

12. Charges value: Enter **15.00**.

13. Click **Save**.

Exercise \#8 Approve purchase orders prior to confirmation (Bonus)
------------------------------------------------------------------

*Objective:  Set up change management so purchase orders are approved prior to
confirmation.*

Contoso has decided that all office supply purchase orders from supplier 1001
should be approved prior to confirmation. They asked you to activate the change
management feature for Supplier 1001.

You will have to do the following:

-   Set up change management against Supplier 1001 only.

-   Configure change management for a vendor.

### Set up change management against Supplier 1001 only

1.  Go to **Procurement and sourcing**, then to **Setup**, and then to
    **Procurement and sourcing parameters**.

2.  Select the **General** tab on the left.

3.  Change to the **Change Management for Purchase Orders** section.

4.  Allow override of settings per vendor: Select **Yes**.

5.  Click **Save**.

### Configure change management for a vendor

1.  Go to **Procurement and sourcing**, then to **Vendors**, and then to **All
    vendors**.

2.  Open the vendor record for vendor **1001** (Acme Office Supplies).

3.  Open the **Purchase order defaults** FastTab.

4.  Click **Edit**.

5.  Go to the **Change Management for Purchase Orders** section.

6.  Override settings: Select **Yes**.

7.  Activate change management: Select **Yes**.

8.  Click **Save**.

Exercise \#9 Create trade agreements for vendors
------------------------------------------------

*Objective: Create a trade agreement for domestic vendors that specifies a fixed
price for a certain item.*

The company managed to standardize the purchase price for item A0001 with all
domestic vendors to be \$8.26. You needto help the purchase manager to record
this purchase price using a trade agreement journal, so that whenever a purchase
order is created for item A0001 and the vendor is from the domestic vendors, the
price will default to \$8.26.

### Create a Trade agreement for a vendor. 

1.  Go to **Procurement and sourcing**, then to **Prices and discounts**, and
    then to **Trade agreement journals**. 

2.  Click **New**. 

3.  Name: Select **S_Price** for Sales price adjustment

4.  Click the **Lines** button to open the journal. 

5.  Relation: Select **Price (purch.)**. 

6.  Account code or Party code type: Select **Group**. 

7.  Account selection: Select **Domestic** vendors. 

8.  Item code/Product code type: Select **Table**. 

9.  Item Relation: Select **A0001, HDMI 6' Cables**. 

10. Site: Enter **1**. 

11. Warehouse: Enter **13**. 

12. From: Enter **1**. 

13. Amount in currency: Enter **8.26**. 

14. Change to the **Details** tab. 

15. From date: Select **February 15, 2017**.  

16. Select **Validate** \> **Validate all lines**. 

17. Click **OK**.

18. After successful validation, **post** the journal.

19. Close all pages.

Exercise \#10 Create a purchase order based on a trade agreement
----------------------------------------------------------------

*Objective: Create a purchase order from on a trade agreement based on value or
quantity.*

The purchasing manager always try to negotiate with vendors and create an
agreed-upon purchasing price list, discounts, and agreements for products that
are frequently purchased from a specific vendor.

Often contracts with vendors can be created to get the best prices for a
specific commitment either based on value or quantity.

In this case the purchase manager made an agreement on a price for 100 of item
number D0002 and would like to use the system to record this agreement.

**You were asked to help the purchase manager and show how this can be recorded.
What would you do?**

### Create a purchase agreement

1.  Go to the **Procurement and sourcing** module, then to **Purchase
    agreements**, and then to **Purchase agreements**. 

2.  Click **New**. 

3.  Vendor account: Select **US-104** (Fabrikam Supplier). 

4.  Purchase agreement classification: Select **General purchases**. 

5.  Open the **General** FastTab. 

6.  Document title: Enter **General Purchase**. 

7.  Default commitment: Select **Product quantity commitment**. 

8.  Click **OK**. 

### Add an item to the purchase agreement

1.  Click **Add line** in the **Purchase agreement lines** FastTab to create a
    line. 

2.  Item number: Select **D0002** (Cabinet). 

3.  Site: Select **1** (Home speakers production). 

4.  Warehouse: Select **13** (Finished Goods). 

5.  Quantity: Enter **100**. 

6.  Unit price: Enter **145.50**. 

7.  Expiration date: Select the end of the next month. 

8.  Click **Save**. 

### Confirm the purchase agreement

1.  Click **Purchase Agreement** at the top, and then select **Confirmation**
    under the **Generate** section. 

2.  Select **Yes** in the **Print report** field. 

3.  Click **OK**. 

4.  Close all pages
