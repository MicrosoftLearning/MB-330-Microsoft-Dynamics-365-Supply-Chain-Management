---
lab:
    title: 'Case study 3C Sales and marketing'
    module: 'Module 3: Implement and manage supply chain processes'
---
Case study 3C Sales and marketing
=================================

Objectives
----------

- *Enter a sales order, review the order totals, and confirm the sale*

- *Setup commissions for sales orders.*

- *Create a sales order with commission, and then check the registered sales
    commission on the sales order.*

Exercise \#1 Enter and confirm sales order
------------------------------------------

*Objective: Enter a sales order, review the order totals, and confirm the sale.*

A sales clerk at USMF who is responsible for receiving and recording sales
orders in the system so that customer requests are fulfilled.

She received a request form Customer US-004, who wants to buy 1 of Item T0004
(“Television M120 37”) with a color of black.

She is not sure on the steps enter and confirm the sales order.

**You are called to provide assistance. What would you do?**

### Enter sales order header details

1. Go to **Sales and marketing \> Sales orders \> All sales orders**.

2. Select **New**.

3. In the **Customer account** field, select the drop-down button to open the
    lookup.

4. In the list, find and select the customer **US-004**.

5. Select **OK**.

6. Select the **Sales order line** fast tab then select the chevron icon next to the **Sales order line**.

7. Select **Dimensions**.

8. For this example, on the **Dimensions Display** pane, select the **Color** from the **PRODUCT DIMENSIONS**, **Site** and **Warehouse** from the **STORAGE DIMENSIONS**. The dimensions you select here will appear in the sales order grid. If you want your selections to persist, set the **Save setup** option to **Yes**.

9. Select **OK**.

10. In the **Item number** field, select the drop-down button to open the lookup.

11. For this example, select item number **T0004**.

12. In the **Color** field, select the drop-down button to open the lookup.

13. In the list, find and select **Black**

14. In the **Quantity** field, enter **1**.

### Review the order totals

1. On the Action Pane, select **Sales order**.

2. Select **View \> Totals**.

    > **Note** The Totals page displays details about the entire order. This includes the subtotal amount, which is a sum of all line net amounts adjusted for
    eventual line discounts, the total invoice amount, which is a subtotal
    amount adjusted for eventual order-level discount, charges, and sales tax,
    the customer credit limit situation, and more. The invoice amount is the
    amount that will appear on the customer's invoice document.

3. Select **OK**.

### Confirm Sales order

1. On the Action Pane, select **Sell**.

2. Select **Generate\> Confirm sale order**.

3. On the Confirm sales order screen, access the **Posting** and **Print confirmation** fields by selecting All under the **Parameters** tab. Check that the **Posting** toggle is set to **Yes** and **Print confirmation** toggle is set to **Yes**.

4. Select **OK**.

5. Select **Yes** to post and print the sale order confirmation on the screen.

Exercise \#2 Create and review a sales order for commission
-----------------------------------------------------------

*Objective: Create a sales order with commission, and then check the registered
sales commission on the sales order.*

The sales manager is required to manage the sales commissions for the sales
representative team. Part of this process is to extend the commission
calculation rule that expired. She will need to set up the necessary commission
to ensure the commission for customer US-013 is being calculated for all items.

You will need to help her to create a sales order for customer US-013, who is
requesting 2 units of item D0001. You will proceed with all of the sales order
process until the invoicing step. Then you will check the registered sales
commission on the sales order.

You will have to do the following:

- Set up commission groups and commission rates
- Assign a commission group to a customer and a product
- Invoice a sales order that qualifies a salesperson for a commission.
- Review the registered sales commission.

### Setup customer groups for commission

1. Go to **Sales and marketing** > **Commissions** > **Customer groups for commission**.

2. Select **New**.

3. In the **Group** field, enter **01**.

4. In the **Name** field, type a **NY**.

5. Select **Save**.

6. Close the page.

### Setup commision item groups

1. Go to **Sales and marketing** > **Commissions** > **Item groups**.

2. Select **New**.

3. In the **Group** field, enter **01**.

4. In the **Name** field, type a **New York**.

5. Select **Save**.

6. Close the page.

### Setup commision sales groups

1. Go to **Sales and marketing** > **Commissions** > **Sales groups**.

    > [!NOTE]
    > A Commission sales group specifies the employees in sales representative roles who are eligible to receive a commission when a customer associated with the relevant sales group buys certain items. In the USMF demo data company, the ales group is called "Sales reps US.

2. On the Action Pane, select **General**.

3. Select **Sales rep..**

    > [!NOTE]  
    > The Sales rep. page displays a list of the company's sales people who are associated with a specific commission group. You can assign multiple sales representatives to the same group and define their respective share of the total commission fee as a percentage value. The total commission share across all employees must not exceed 100.

4. In the list, mark the selected row.

5. Select **Edit**.

6. Set **Commission share** to `50`.

7. Select **New**.

8. In the **Name** field, select the drop-down button to open the lookup. Use the Quick Filter to find records. For example, filter on the Name field with a value of 'Susan Burk'.

9. Select **Select**.

10. Set **Commission share** to `50`.

11. Select **Save**.

### Setup commision calculation

1. Go to **Sales and marketing** > **Commissions** > **Commission calculation**.
    > [!NOTE]
    > In the Commission calculation page, you define the commission rate that the employee is to receive for a sales transaction when it contains the pre-set combination of customer and product. As part of the commission rate setup, you must specify the commission calculation basis and whether it should include or exclude discounts. You can also enter a validity period for when the commission rate is active.

2. Select **New**.

3. In the **Item code** field, select **Group**.

4. In the **Item relation** field, select the drop-down button to open the lookup.

5. In the list, find and select the group that you created earlier.

6. In the **Customer code** field, select **Group**.

7. In the **Customer relation** field, select the drop-down button to open the lookup.

8. In the list, select the group that you set up earlier.

9. In the **Sales rep. relation** field, select the drop-down button to open the lookup.

10. In the list, find and select the desired record.

    - Keep the **Before line discount** option.
    - Keep the **Revenue** option as the basis for commission value calculation.

11. In the **Commission percentage** field, enter a number.

12. Select **Save**.

### Invoice a sales order that qualifies a salesperson for a commission

1. Go to **Sales and marketing \> Commissions \> Commission calculation**

2. Select **Edit**.

3. In the **To** field select **12/31/2024**

4. Select **Save.**

5. Close the page.

6. Go to **Sales and marketing \> Sales orders \> All sales orders**.

7. Select **New**.

8. In the **Customer account** field, select the drop-down button to open the
    lookup.

9. In the list, find and select **US-013**.

10. Select **OK**.

11. Select **Header** tab.

12. Expand the **Setup** section.

    > [!NOTE]
    > The value in the **Sales group** field represents a group with one or more sales representatives assigned to it. The people in the group are the ones who will receive commissions when the order is invoiced, as per predefined rates and distribution. The value is copied from the Customer card, but you can change it if you wish. The Sales group is also copied to the sales order line. You can change it so that it can differ from the one in the header and/or between lines.

    > [!NOTE]
    > The value in the **Commission group** field represents a group that you have     created for one or more customers with the purpose of tracking commissions. The value is copied from the Customer card, but you can change it if you wish.

13. Select **Lines** tab.

14. In the **Item number** field, select the drop-down button to open the lookup.

15. In the list, select **D0001/MidRangeSpeaker**.

16. In the **Quantity** field, enter **2**.

    > **TIP**
    > Review the net amount. It represents the sales revenue, which in this example is the basis for commission.

17. Select **Save**.

18. On the Action Pane, select **Sell**.

19. Select **Generate\> Confirm Sale Order**.

20. This will prompt you with a screen where you will check the **Posting** field
    is set to **Yes** and **Print confirmation** is set to **Yes**.

21. Select **OK**.

22. Select **Yes** to post and print the Sale order confirmation on the screen.

23. On the Action Pane, select **Pick and Pack**.

24. Select **Generate\> Post packing Slip**.

25. This will prompt you with a screen where you will check that the Parameter
    **Quantity** Field is set to **ALL** and the **Posting** flag is set to
    **Yes**.

26. Select **OK** twice.

27. Select **OK**.

28. On the Action Pane, select **Invoice**.

29. Under **Generate** field group, select **Invoice**.

30. Expand the **Parameters** section.

31. In the **Quantity** field, select **All**.

32. Select **Yes** in the **Posting** field.

33. Select **OK**.

34. Select **OK**.

    > **Note** It may take a minute or so to post the transaction. Allow the
    processing to complete.

### Assign a commission group to a customer and a product

1. Go to **Sales and marketing** > **Customers** > **All customers**.

2. In the list, find and select the desired record.

3. Click **Edit**.

4. Expand the **Sales order defaults** section.

5. In the **Commission group** field, click the drop-down button to open the lookup.

6. In the list, select the group that you created earlier.

7. In the **Sales group** field, click the drop-down button to open the lookup.

8. In the list, find and select the desired record.

9. Click **Save**.

10. Go to **Product information management > Products > Released products**.

11. Use the Filter to find records. For example, filter on the Item number field with a value of **D0001**.

12. In the list, click the link in the selected row.

13. Click **Edit**.

14. Expand the **Sell** section.

15. In the **Commission group** field, click the drop-down button to open the lookup.

16. In the list, select the commission group that you created earlier.

17. Select **Save**.

### Review the registered sales commissions

1. On the Action Pane, select **Invoice**.

2. Under **Journals** field group, select **Invoice**.

3. Select **Details \> Commission transactions**.

4. Review the details in the **Overview** tab.

    > [!NOTE]
    > The **Overview** tab displays lines representing the commission amounts payable to sales representatives who are associated with the invoiced sales order.

5. Close the page.

6. Select **Voucher**.

    > **Note** You can review the voucher transactions for the
    commission amounts that have been posted to the predefined commission
    expense and commission payable accounts.

7. Close all pages.

Exercise \#3 Create a customer trade agreement
----------------------------------------------

*Objective: Create a customer trade agreement for specific customers, a specific
item and for a certain date range.*

The sales managers always try to standardize the sales price list and discounts
(trade agreements) for products. Sometimes they create special price lists and
discounts for special customers.

The sales manager you are working with decided to create sales price trade
agreement for item A0001 for all retail customers accounts and to set that price
at \$20. she also want to add a validity date for that price.

In order to record this sales price in the system she will use the trade
agreement journal, so that whenever a sales order is created for item A0001 and
the customer is from the retail accounts group, the price will default to \$20.

**What would you do to guide her thru this entry?**

### Create a trade agreement named “Sales price adjustment

1. Go to **Sales and marketing**, then to **Prices and discounts**, and then to
    **Trade agreement journals**.

2. Select **New**.

3. Name: Select **S_Price**, **Sales price adjustment**.

4. Select the **Lines** button to open the journal.

5. Relation: Select **Price (sales)**.

6. Account code or Party code type: Select **Group**.

7. Account selection: Select **03**, **Retail accounts**.

8. Item code or Product code type: Select **Table**.

9. Item Relation: Select **A0001, HDMI 6' Cables**.

10. From: Enter **1**.

11. Amount in currency: Enter **20.00**.

12. Change to the **Details** tab.

13. From date: Select **February 15, 2017**.  

14. Lead time: Enter **2**.

15. Select **Validate** \> **Validate all lines**.

16. Select **OK**.

17. After successful validation, **post** the journal

18. Close all pages.


Exercise \#4 Generate and process customer rebate claimes for payment
----------------------------------------------

*Objective: Generate rebates and process rebate claims for payment.*
----------------------------------------------
Sales manager build better relationships with customers and encourage them to be
loyal to the company\`s products and services by offering them rebates based on
the order volumes or quantities.

Customers can receive balance deductions, trade spending, invoices deductions,
or get paid directly.

The sales manager you are working with asked you to show how this works using
existing rebates for item T0020 and process a claim.

You will have to do the following:

- Generate and process customer rebates.

- Generate rebate claims.

- Process rebate claims.

- Process rebates for payment.

### Generate and process customer rebates

1. In **USMF** navigate to the **Accounts Receivable** \> **Setup** \> **Accounts
    receivable parameters** page, select the **Prices** tab and expand the
    **Price details** tab, and check that the **Enable price** details option is
    set to **Yes**.

2. Navigate to the **Sales and marketing** \> **Customer rebates** \> **Rebate agreements**
    page and select the **customer rebate agreement**: **USMF-000001**.

3. If the Workflow approval status field is not set to **Approved**, you need
    to select **Validation** on the Action pane to approve it.

4. Review a customer rebate agreement

    - The agreement is for an individual customer, in this example customer
    **US-009**.

    - Rebates are given to the customer when they purchase a specific product. In
    this case, the product has item number **T0020**.

    - The customer's sales performance, against which the rebate amounts are
    estimated, is to be accumulated on a weekly basis.  

      - The setting for **Price taken from** is **Gross**, which means that
        line's sales amount on which basis the claim is estimated is not reduced
        by the line discount.

      - The **Rebate line break type** field shows the method for calculating
        rebates. In this case, the sales target against which the rebates are to
        be estimated is set to **Quantity**.

      - The agreement's lines specify the rebate amount type, the actual rebate
        value, and the thresholds. In this example, the customer will qualify
        for a rebate of 20 USD per unit sold, if their weekly purchases of the
        product fall within 1 to 50 units; and a rebate of 40 USD per unit sold,
        if they purchase above 50 units.
5. Select **Validation** from the Action pane and select **OK**.

### Generate rebate claims

1. Navigate to **Sales and marketing \> Sales orders \> All sales orders**.

2. Select **New**.

3. In the **Customer account** field, enter or select **US-009**.

4. Select **OK**.

5. In the **Item number** field, enter or select **T0020**.

6. Set **Quantity** to **40**.

7. Select **Sales order line**.

8. Select **Price details**.

9. Expand the **Rebates** section. The Rebates tab lists all the rebate
    agreements that are applicable to the current order line and shows the
    estimated rebate amount. Note that the displayed amounts are only
    indications of what future rebate claims may be. The actual rebate amounts
    may be different depending on: the total sales volume achieved by the
    customer under a periodic rebate agreement; whether the customer had
    returned all or partial quantities; and whether the applicable sales order
    was invoiced.  

10. Close the page.

11. Select **Save**.

12. On the Action Pane, select **Invoice**.

13. Select **Invoice \> Generate \> Invoice**.

14. Expand the **Parameters** section.

15. In the **Quantity** field, select **All**.

16. Select **OK**.

17. Select **OK**.

18. Close all pages.

### Process rebate claims

The Rebates page acts a workbench in which you can review, approve, and process
rebate claims. You’ll now process the claims that were created as a result of
invoicing a sales order for customer US-009, who is the subject of the rebate
agreement USMF-000001.

The line represents a rebate claim for 800 USD, which is based on the sales of
40 units of product T0020, calculated at 20 USD per unit. This matches the
conditions of the first quantity break in the rebate agreement.

The claim is in the **To be calculated** state. This means that it is associated
with an agreement that tracks the customer's sales performance on periodic basis
and it must be re-calculated to account for the total sales volume within the
respective period.  

1. Navigate to **Sales and marketing \> Customer rebates \> Rebates**.

2. Select **Cumulate**.

3. In the **Customer** field, enter or select **US**-**009**.

4. In the **Start date** field, select today's date.

5. Select **OK**.

6. Select **Approve**.

7. Select **Process**.

8. In the **Customer** field, enter or select **US-009**.

9. Select **OK**.

If you get a message that it cannot create a record in Ledger journal table, it
is because the demo data is out of sync; perform these steps:

1. Select **Close**.

2. Reset the number sequence:

    1. Navigate to **General Ledger \> Ledger setup \> General ledger
        parameters**.

    2. Select **Number sequences** tab.

    3. Select the hyperlink for **Number sequence code** field for Journal batch
        number.

    4. In the **General** FastTab, change the Next number higher.

    5. Set **Continuous** to **No**.

    6. Select **Yes**.

3. Navigate to **Sales and marketing \> Customer rebates \> Rebates**.

4. Resume with step 7 of Process rebate claims.

A message shows that the rebate was processed successfully, and the status of
the claims has been changed to Mark. This means that as a result of a Rebate
accrual journal being posted:  

- the claims have now been transferred to the temporary customer balance as
    deductions;  

- the Rebate accrual account has been credited to represent the future
    liability towards the customer; and  

- the Rebate expense account has been debited, in recognition of the cost
    incurred in connection with the sales.

### Process rebates for payment

The Rebate page lists the rebate claims that you have processed in the customer
rebate workbench and that are in status **Mark**. When you create a credit note,
a message appears to inform you that a journal has been posted.

This is the Accounts receivable consumption journal, as specified in the
Accounts receivable parameters page. This causes the real liability (credit)
amount to be moved to the customer balance. This means that the customer’s
account has been credited, and the Rebate accrual account has been debited.  

1. Navigate to **Accounts receivable\>Customers\>All customers**.

2. In the list, find and select **US-009**.

3. On the Action Pane, select **Collect**.

4. Select **Settle \> Settle transactions**.

5. Select **Functions**.

6. Select **Rebate program**.  

7. Select **Edit**. Set checkmarks in the **Mark** field for the claims that you
    want to include into credit note.

8. Select **Functions**.

9. Select **Create credit note**.  

10. Close the page.

11. Select **Cancel**. This refreshes the page so that you can see the updates.

12. On the Action Pane, select **Collect**.

13. Select **Settle transactions**. Note that a transaction for negative amount,
    representing the total rebate amount, without invoice reference has been
    added to the customer balance.  

14. Select **Cancel**.

15. Close all pages.

