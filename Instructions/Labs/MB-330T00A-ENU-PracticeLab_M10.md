Exercise: Configure and use commissions
=======================================

Register sales commissions
--------------------------

In **USMF** you need to extend the commission calculation rule which was expired
on 12/31/2017. You need to have all the necessary commission calculation setup
to ensure the commission for customer US-013 for all items are being calculated.

Take note of the customer and item numbers that you have chosen for the
commission process and use them when asked to create a sales order in this
guide.

### Invoice a sales order that qualifies a salesperson for a commission

1.  Go to **Sales and marketing \> Commissions \> Commission calculation**

2.  Click **Edit**.

3.  In the To field select **12/31/2020**

4.  Click **Save.**

5.  Close the page.

6.  Go to **Sales and marketing \> Sales orders \> All sales orders**.

7.  Click **New**.

8.  In the **Customer account** field, click the drop-down button to open the
    lookup.

9.  In the list, find and select **US-013**.

10. Click **OK**.

11. On the Action Pane, click **Options**.

12. Click **Change view**.

13. Click **Header view**.

14. Expand the **Setup** section.

15. The value in the **Sales group** field represents a group with one or more
    sales representatives assigned to it. The people in the group are the ones
    who will receive commissions when the order is invoiced, as per predefined
    rates and distribution. The value is copied from the Customer card, but you
    can change it if you wish. The Sales group is also copied to the sales order
    line. You can change it so that it can differ from the one in the header
    and/or between lines.

16. The value in the **Commission group** field represents a group that you have
    created for one or more customers with the purpose of tracking commissions.
    The value is copied from the Customer card, but you can change it if you
    wish.

17. On the Action Pane, click **Options**.

18. Click **Change view**.

19. Click **Line view**.

20. In the **Item number** field, click the drop-down button to open the lookup.

21. In the list, select **D0001**.

22. In the Quantity field, enter **2**.

23. Take note of the line's Net amount. It represents the sales revenue, which
    in this example is the basis for commission calculation.

24. Click **Save**.

25. On the Action Pane, click **Invoice**.

26. Under **Generate** field group, click **Invoice**.

27. Expand the **Parameters** section.

28. In the **Quantity** field, select **'All'**.

29. Select **Yes** in the **Posting** field.

30. Click **OK**.

31. Click **OK**. It may take a minute or so to post the transaction. Allow the
    processing to complete and don’t close the page until it’s done.

### Review the registered sales commissions

1.  On the Action Pane, click **Invoice**.

2.  Under **Journals** field group, click **Invoice**.

3.  On the Action Pane, click **Invoice**.

4.  Click **Details \> Commission transactions**.

5.  The **Overview** tab displays lines representing the commission amounts
    payable to sales representatives who are associated with the invoiced sales
    order. Let's review the details.

6.  Close the page.

7.  Click **Voucher**. You can review the voucher transactions for the
    commission amounts that have been posted to the predefined commission
    expense and commission payable accounts.

8.  Close all pages.

Create sales orders
-------------------

This procedure shows you how to create a sales order. You can use the procedure
in demo data company USMF. Sales orders are typically created by a sales order
processor.

### Enter sales order header details

1.  Go to **Sales and marketing \> Sales orders \> All sales orders**.

2.  Click **New**.

3.  In the **Customer account** field, click the drop-down button to open the
    lookup.

4.  In the list, find and select the customer **US-004**.

5.  Click **OK**.

6.  Click **Sales order line**.

7.  Click **Dimensions**.

8.  For this example, select the Color, Site and Warehouse dimensions. The
    dimensions you select here will appear in the sales order grid. If you want
    your selections to persist, set the **Save setup** option to **Yes**.

9.  Click **OK**.

10. In the **Item number** field, click the drop-down button to open the lookup.

11. For this example, select item number **T0004**.

12. In the **Color** field, click the drop-down button to open the lookup.

13. In the list, find and select **Black**

14. In the **Quantity** field, enter **1**.

### Review the order totals

1.  On the Action Pane, click **Sales order**.

2.  Click **View \> totals**.

3.  The Totals page displays details about the entire order. This includes the
    subtotal amount, which is a sum of all line net amounts adjusted for
    eventual line discounts, the total invoice amount, which is a subtotal
    amount adjusted for eventual order-level discount, charges, and sales tax,
    the customer credit limit situation, and more. The invoice amount is the
    amount that will appear on the customer's invoice document.

4.  Click **OK**.
