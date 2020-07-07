Exercise 1: Create a purchase order
===================================

Create one purchase order for Acme Office Supplies, to be delivered today, with
5 of item number T0003 to be delivered to Site 1, and 5 of M1101 Foam Reacting
Agent to be delivered to the Quality Testing Center,123 W. Cherry Street, Zip
Code 83642.

1.  Go to the **Procurement and sourcing** module, then to **Purchase orders**,
    and then to **All purchase orders**.

2.  Click **New**.

3.  Vendor account: Select **1001** (Acme Office Supplies).

4.  Delivery date: Verify the current date in the **Delivery date** field (this
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

9.  On the Action Pane, click **Receive**.

10. Click Generate \> **Product receipt**.

11. Change Quantity to Registered quantity.

12. In the **Product receipt** field, enter the product receipt number. For
    example, enter **PR123**.

13. Click **OK** to post the product receipt.

14. Close all pages.

Exercise 2: Manage charges
==========================

Create a Charges Code
---------------------

You are the Accounts Payable Coordinator at Contoso Entertainment Systems USA,
and you must create a new charges code for transport charges that will be added
to various items and charged by the vendor.

Create a new charge for transportation fees with the following specifications:

-   Name of the charges code: TRANSTO

-   Description: Transportation Fee to our sites

-   Account: 411400

This fee does not require an item sales tax group.

1.  Go to the **Accounts payable** module, then to **Charges setup**, and then
    to **Charges code**.

2.  Click **New**.

3.  Charges code: Enter **TRANSTO**

4.  Description: Enter **Transportation Fee to our sites**

5.  Change to the Debit section

6.  Type: Select **Ledger account**

7.  Posting: Select **Payment fee**

8.  Account: Select **411400**

9.  Change to the Credit section

10. Type: Select **Customer/Vendor**

11. Click **Save**.

Create a Vendor Charges Group
-----------------------------

Vendor Fabrikam has two vendor accounts that we purchase items from. They have
decided to add an additional 15 percent freight charges for all our purchase
orders.

As the Accounts Payable Administrator, you are asked to set up a new vendor
charges group and assign the code to vendors US-101 and US-104. The name of the
new charges group is "06" and the description is "Freight 15%".

1.  Go to the **Accounts payable** module, then to **Charges setup**, and then
    to **Vendor charges group**.

2.  Click **New**.

3.  Charges group: Enter **06**

4.  Description: Enter **Freight 15%**

5.  Click **Save**.

Update vendors to use the new vendor charges group.
---------------------------------------------------

1.  Go to the **Accounts payable** module, then to **Vendors**, and then to
    **All vendors**.

2.  Open the vendor record for vendor **US-101** (Fabrikam Electronics).

3.  Click **Edit**.

4.  Open the **Purchase order defaults** FastTab.

5.  Charges group: Select **06** (Freight 15%)

6.  Click **Save**.

7.  Close the vendor record.

8.  Open the vendor record for vendor **US-104** (Fabrikam Supplier).

9.  Click **Edit**.

10. Open the **Purchase order defaults** FastTab.

11. Charges group: Select **06** (Freight 15%)

12. Click **Save**.

13. Close the vendor record.

Create an Item Charges Group
----------------------------

Because of the large quantity and weight of items bought, Datum Receivers
(US-105) applies a 15 percent freight charge for all orders.

1.  Go to the **Accounts payable** module, then to **Charges setup**, and then
    to **Item charge groups**.

2.  Click **New**.

3.  Charges group: Enter **123**

4.  Description: Enter **15% Freight Charge**

5.  Click **Save**.

Create an Automatic Charge
--------------------------

You have a certain set of charges that apply on all purchases from certain
vendors.

Set up an automatic charge that will apply automatically to all purchases, where
it will charge 15% delivery charge to all orders at the line level, and applies
for only a certain vendor charges group (06) and a certain item charges group
(123).

1.  Go to the **Accounts payable** module, then to **Charges setup**, and then
    to **Automatic charges**.

2.  Level: Select **Line**

3.  Click **New**.

4.  Account code: Select **Group**

5.  Vendor relation: Select **06** (Freight 15%)

6.  Item code: Select **Group**

7.  Item Relation: Select **123** (15% Freight Charge)

8.  Click **Save**.

9.  Click **Add** in the **Lines** FastTab.

10. Charges code: Select **TRANSTO** (Transportation Fee)

11. Category: Select **Percent**

12. Charges value: Enter **15.00**

13. Click **Save**.

Set Up Change Management
------------------------

Contoso has decided that all office supply purchase orders from supplier 1001
should be approved prior to confirmation.

### Set up change management against Supplier 1001 only.

1.  Go to **Procurement and sourcing**, then to **Setup**, and then to
    **Procurement and sourcing parameters**.

2.  Select the **General** tab on the left.

3.  Change to the **Change Management for Purchase Orders** section.

4.  Allow override of settings per vendor: Select **Yes**.

5.  Click **Save**.

6.  Configure change management for a vendor.

7.  Go to **Procurement and sourcing**, then to **Vendors**, and then to **All
    vendors**.

8.  Open the vendor record for vendor **1001** (Acme Office Supplies).

9.  Open the **Purchase order defaults** FastTab.

10. Click **Edit**.

11. Go to the **Change Management for Purchase Orders** section.

12. Override settings: Select **Yes.**

13. Activate change management: Select **Yes**.

14. Click **Save**.
