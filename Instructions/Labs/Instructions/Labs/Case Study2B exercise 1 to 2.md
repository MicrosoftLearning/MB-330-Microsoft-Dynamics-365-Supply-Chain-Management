---
lab:
    title: 'Case study 2B Sales and marketing'
    module: 'Module 3: Implement and manage supply chain processes '
---
Case study 2B Sales and marketing
=================================

Objectives
----------

- *Enter a sales order, review the order totals, and confirm the sale*

- *Create a sales order with commission, and then check the registered sales
    commission on the sales order.*

- *Create a customer trade agreement for specific customers, a specific item
    and for a certain date range.*

- *Generate rebates and process rebate claims for payment.*

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

    > **Note** The Totals page displays details about the entire order. This includes the
    subtotal amount, which is a sum of all line net amounts adjusted for
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
- Invoice a sales order that qualifies a salesperson for a commission.
- Assign a commission group to a customer and a product
- Review the registered sales commission.

###

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

13. The value in the **Sales group** field represents a group with one or more
    sales representatives assigned to it. The people in the group are the ones
    who will receive commissions when the order is invoiced, as per predefined
    rates and distribution. The value is copied from the Customer card, but you
    can change it if you wish. The Sales group is also copied to the sales order
    line. You can change it so that it can differ from the one in the header
    and/or between lines.

14. The value in the **Commission group** field represents a group that you have
    created for one or more customers with the purpose of tracking commissions.
    The value is copied from the Customer card, but you can change it if you
    wish.

15. Select **Lines** tab.

16. In the **Item number** field, select the drop-down button to open the lookup.

17. In the list, select **D0001/MidRangeSpeaker**.

18. In the **Quantity** field, enter **2**.

    > **TIP**
    > Review the net amount. It represents the sales revenue, which in this example is the basis for commission.

19. Select **Save**.

20. On the Action Pane, select **Sell**.

21. Select **Generate\> Confirm Sale Order**.

22. This will prompt you with a screen where you will check the **Posting** field
    is set to **Yes** and **Print confirmation** is set to **Yes**.

23. Select **OK**.

24. Select **Yes** to post and print the Sale order confirmation on the screen.

25. On the Action Pane, select **Pick and Pack**.

26. Select **Generate\> Post packing Slip**.

27. This will prompt you with a screen where you will check that the Parameter
    **Quantity** Field is set to **ALL** and the **Posting** flag is set to
    **Yes**.

28. Select **OK** twice.

29. Select **OK**.

30. On the Action Pane, select **Invoice**.

31. Under **Generate** field group, select **Invoice**.

32. Expand the **Parameters** section.

33. In the **Quantity** field, select **All**.

34. Select **Yes** in the **Posting** field.

35. Select **OK**.

36. Select **OK**.

    > **Note** It may take a minute or so to post the transaction. Allow the
    processing to complete.

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
