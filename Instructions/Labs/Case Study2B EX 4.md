---
lab:
    title: 'Case study 2B Sales and marketing: Customer rebates'
    module: 'Module 3: Implement and manage supply chain processes '
---
Case study 2B Sales and marketing
=================================

Objectives
----------

- *Generate rebates and process rebate claims for payment.*

Exercise \#1 Generate and process customer rebates
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
        be estimated is set to Quantity.

      - The agreement's lines specify the rebate amount type, the actual rebate
        value, and the thresholds. In this example, the customer will qualify
        for a rebate of 20 USD per unit sold, if their weekly purchases of the
        product fall within 1 to 50 units; and a rebate of 40 USD per unit sold,
        if they purchase above 50 units.

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
