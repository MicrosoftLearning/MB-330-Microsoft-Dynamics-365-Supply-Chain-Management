Exercise 1: Set up a Shipping Carrier and Carrier Service 
==========================================================

**USMF** in the United States has a new customer that is located in Europe. Ted,
the Transportation Coordinator, at Contoso Entertainment has determined that a
new company will be used for transporting the products to this customer. Ted
needs to set up a new ocean carrier and carrier service. 

Set up a new carrier. 
----------------------

1.  Open **Transportation management** \> **Setup** \> **Carriers** \>
    **Shipping carriers**.  

2.  In the action pane, click **New** to create a new shipping carrier.  

3.  In the **Shipping carrier** field, type **Ocean Carrier 2**. 

4.  In the **Name** field, type **Secondary ocean carrier**. 

5.  In the **Mode** field, select **Ocean**.  

6.  Expand the **Overview** FastTab.   

7.  Set the **Activate shipping carrier** slider to **Yes**. 

8.  Select vendor account **1002** from the **Vendor** drop-down menu.  

9.  In the **SCAC** field, type **2005.** 

10. Set the **Activate carrier rating** slider to **Yes.** 

11. On the **Addresses** FastTab, click **New**. 

12. In the **New address** form, type **Ocean carrier location** in the **Name**
    field. 

13. Select **Business** from the **Purpose** drop-down list. 

14. Select USA in the Country/region drop-down list. 

15. In the **ZIP/postal code** field, type **11251**. 

16. In the **Street** field, type **1577 Madison Blvd**. 

17. Set the **Primary** slider to **Yes**. 

18. Click **OK.** 

19. Close the **Shipping carriers** form. 

Add a carrier service to the carrier. 
--------------------------------------

1.  Open **Transportation management \> Setup \> Carriers \> Shipping
    carriers.** 

2.  Select **Ocean Carrier 2** in the left-hand pane. 

3.  Expand the **Services** FastTab. 

4.  Click **New.** 

5.  In the **Carrier service** field, type **Ocean**.  

6.  In the **Name** field, type **Ocean**. 

7.  In the **Transportation method** field, select **Ocean**. 

8.  Select **Freight** from the **Billing group ID** drop-down menu. 

9.  Close the form. 

 

Exercise 2: Set up rate masters
===============================

This procedure shows you how to set up a rate master. The logistics manager
usually sets up rate masters, depending on the contracts signed with the
carriers. In this scenario you will set up a rate master for an air carrier. The
demo data company used to create this procedure is USMF.

Set up rate master
------------------

1.  Go to **Transportation management \> Setup \> Rating \> Rate master.**

2.  Click New.

3.  In the Rate master field, type **AtlantaMaster**.

4.  In the Name field, type **Atlanta rate master**.

5.  In the Rating metadata ID field, click the drop-down button to open the
    lookup.

    -   The rating metadata ID will determine the data needed for the rate
        master, as it defines the metadata expected by the TMS engine using this
        rate master.

6.  For this example, select the **P2P** option.

7.  Click Save.

Set up rate base
----------------

1.  Click Rate base.

    -   The rate base determines the rate of the carrier, and can be used to set
        up a tariff structure as it structures the rates in the breakpoints
        defined in the break master.

2.  Click New.

3.  In the Rate base field, type **AtlantaBase**.

4.  In the Name field, type **Atlanta rate base**.

5.  In the Break master field, click the drop-down button to open the lookup.

    -   Break masters are used to define the pricing structure and its
        breakpoints. The pricing structure uses tiered pricing that is based on
        physical dimensions.

>   For this example, use **weight.**

1.  Toggle the expansion of the Details section.

2.  Click New.

3.  In the Drop-off Postal Code From field, type '30301'.

4.  In the Drop-off Postal Code To field, type '30318'.

5.  In the Drop-off Country Region field, type 'USA'.

6.  In the \<1.00 Lbs field, type '100'.

    -   Insert the rate per lbs if the total weight of the load is less than 1
        pound.

7.  In the \<5.00 Lbs field, type '300'.

    -   Insert the rate per lbs if the total weight of the load is less than 5
        pounds.

8.  In the \<20.00 Lbs field, type '500'.

    -   Insert the rate per lbs if the total weight of the load is less than 20
        pounds.

9.  In the \<100.00 Lbs field, type '1000'.

    -   Insert the rate per lbs if the total weight of the load is less than 100
        pounds.

10. In the \<1,000.00 Lbs field, type '3000'.

    -   Insert the rate per lbs if the total weight of the load is less than
        1000 pounds.

11. Click Save.

12. Close the page.

Assign rate base
----------------

1.  Toggle the expansion of the Rate base assignments section.

2.  Click New.

    -   You can have several rate base assignments for each rate master. This
        makes it possible to create several different price points for each
        carrier depending on destinations, services, or different rate bases. In
        this procedure you will only create one rate base assignment.

3.  In the Name field, type **AtlantaRateAssignment**.

4.  In the Rate base field, click the drop-down button to open the lookup.

5.  In the list, select **AtlantaBase**.

6.  In the Service field, click the drop-down button to open the lookup.

7.  In the list, find and select **Truck**.

8.  In the Pick-up Postal Code field, type '98052'.

    -   Specify which postal code this rate base assignment should be valid
        from.

9.  In the Pick-up Country Region field, type 'USA'.

10. Click Save.

 

Exercise 3: Create route plan and route guide 
==============================================

Create a Route Plan 
--------------------

As a member of the Dynamics 365 for Operations project team for Adventure Works
Cycles, you have to configure a new route plan for Georgia to Los Angeles. You
will need to create a new hub for the warehouses at Georgia and Los Angeles. 

### Create a new route plan named “WA to IL”. 

1.  Open **USMF \> Transportation management \> Setup \> Routing \> Route
    plans.**  

2.  Click **New**. 

3.  In the **Route plan** field, enter GA to LA. 

4.  In the **Name** field, enter Georgia to Los Angeles. 

5.  Close the form. 

### Create a new hub for Georgia and one for Los Angeles. 

1.  Open **Transportation management \> Setup \> Routing \> Hub masters**.  

2.  Click **New**.  

3.  In the **Hub** field, enter Georgia 3. 

4.  In the **Name** field, enter Savannah GA. 

5.  Expand the **Codes** FastTab. 

6.  In the **Hub type** field, select Hub. 

7.  In the **Rate master** field, select TruckRateMaster.  

8.  Expand the **Effective dates** FastTab. 

9.  In the **Effective start date and time** field, select Today. 

10. In the **Effective end date and time** field, select 12/31/2025. 

11. Expand the **Address** FastTab. 

12. Click **Add**. 

13. In the **Name or description** field, enter Georgia 3. 

14. In the **Zip/postal code** field, enter 31302. 

15. In the **Street** field, enter 123 ABC Street. 

16. Click **OK**. 

17. Click **New**.  

18. In the **Hub** field, enter Los Angeles 2. 

19. In the **Name** field, enter Los Angeles CA 2. 

20. Expand the **Codes** FastTab. 

21. In the **Hub type** field, select Hub. 

22. In the **Rate master** field, select TruckRateMaster.  

23. Expand the **Effective dates** FastTab. 

24. In the **Effective start date and time** field, select Today. 

25. In the **Effective end date and time** field, select 12/31/2025. 

26. Expand the **Address** FastTab. 

27. Click **Add**. 

28. In the **Name or description** field, enter Los Angeles 2. 

29. In the **Zip/postal code** field, enter 90001. 

30. In the **Street** field, enter 987 XYZ Avenue. 

31. Click **OK**. 

32. Close the form. 

### Add details to the route plan. 

1.  Open **Transportation management \> Setup \> Routing \> Route plans.**  

2.  Select the **GA to LA** route plan. 

3.  On the **Details** FastTab, click **New**.  

4.  In the **Origin hub** field, select Georgia 3. 

5.  In the **Destination hub** field, select Los Angeles 2. 

6.  In the **Shipping carrier** field, select TruckCarrier. 

7.  In the **Carrier service** field, select Truck. 

8.  Close the form. 

 

Create a Route Guide 
---------------------

As a member of the Dynamics 365 for Operations project team for Adventure Works
cycles, you have to configure a new routing guide for Georgia to Los Angeles.
The routing guide should ultimately lead to the result being a particular
shipping carrier, TruckCarrier, with the carrier service, Truck. 

### Create a new routing guide named “GA to LA”. 

1.  Open **USMF \> Transportation management \> Setup \> Routing \> Route
    guides.**  

2.  Click **New**. 

3.  In the **Routing guide** field, enter GA to LA. 

4.  In the **Name** field, enter Georgia to Los Angeles.  

### Add Information, Origin, Destination, and Result entities to the routing guide. 

1.  Expand the **Information** FastTab. 

2.  In the **Direction** field, select Outbound.  

3.  Set the **Active** slider to the **Yes** position. 

4.  In the **Effective start date and time** field, select Today. 

5.  In the **Effect end date and time** field, enter 12/31/2025. 

6.  Expand the **Origin** FastTab. 

7.  In the **Zip/postal code** field, enter 31302. 

8.  In the **Hub** field, select Los Angeles 2. 

9.  In the **Country/region** field, enter USA. 

10. Expand the **Destination** FastTab. 

11. In the **Zip/postal code from** field, enter 31302. 

12. In the **Zip/postal code to** field, enter 90001. 

13. In the **Hub** field, select Georgia 3. 

14. In the **Country/region** field, enter USA. 

15. Expand the **Result** FastTab. 

>   In the **Shipping carrier** field, select TruckCarrier. 

>   In the **Carrier service** field, select Truck. 

1.  Click **Save**.

 

 

Exercise 4: Process inbound shipment 
=====================================

Prerequisite Steps 
-------------------

### Add a vendor address for the Ade Supply Company. 

1.  Open **Accounts payable \> Vendors \> All vendors**. 

2.  Select vendor **1003** from the list of vendors. 

3.  In the action pane, click **Edit**. 

4.  In the **Addresses** FastTab, click **Add**. 

5.  In the **Name or description** field, type **Ade Supply Main Location**. 

6.  In the **Zip/postal code** field, enter **00210**. 

7.  In the **Street** field, enter **123 Main Street**. 

8.  Set the **Primary** slider to **Yes**. 

9.  Click **OK**. 

10. In the **Invoice and delivery** FastTab, in the **Mode of delivery** field,
    select **Parce-STD**. 

11. Close the forms. 

### Modify the CFR terms of delivery. 

1.  Open **Accounts payable \> Setup \> Terms of delivery**. 

2.  Select **CFR** from the left-hand panel. 

3.  Click **Edit** in the action pane. 

4.  In the **Transportation** FastTab, set the **Add transportation charges to
    retail sales orders** slider to **Yes**. 

5.  Close the form. 

 

Create a Hub, Route Plan, and Route Guide 
------------------------------------------

You have been asked to set up a hub for the Ade Supply Company and create a
route plan and guide between the Ade Supply Company and USMF’s Warehouse 61. 

### Create a hub for the Ade Supply Company. 

1.  Open **Transportation management \> Setup \> Routing \> Hub masters**. 

2.  Click **New** in the action pane. 

3.  In the **Hub** field, enter **Ade Supply.** 

4.  In the **Name** field, enter **Ade Supply NH**. 

5.  In the **Codes** FastTab, in the **Hub type** field, select **Hub**. 

6.  In the **Rate master** field, select **ParcelRateMaster**. 

7.  In the **Address** FastTab, click **Add**. 

8.  In the **New address** form, in the **Name or description** field, enter
    **Ade Supply NH**. 

9.  In the **ZIP/postal code** field, enter **00210**. 

10. In the **Street** field, enter **123 Main Street**. 

11. Click **OK**. 

12. Close the form. 

### Create a route plan from New Hampshire to Washington. 

1.  Open **Transportation management \> Setup \> routing \> Route plans**. 

2.  Click **New** in the action pane. 

3.  In the **Route plan** field, enter **NH to WA**. 

4.  In the **Name** field, enter **New Hampshire to Washington**. 

5.  In the **Details** FastTab, click **New**. 

6.  In the **Origin hub** field, select **Ade Supply**. 

7.  In the **Destination hub** field, select **Own WHS**. 

8.  In the **Shipping carrier** field, select **ParcelCarrier**. 

9.  In the **Carrier service** field, select **STD**. 

10. In the **Vendor** field, select **1003**. 

11. Close the form. 

### Create a route guide from New Hampshire to Washington. 

1.  Open **Transportation management \> Setup \> Routing \> Route guides**. 

2.  Click **New** in the action pane. 

3.  In the **Routing guide** field, enter **NH to WA**. 

4.  In the **Name** field, enter **New Hampshire to Washington**. 

5.  In the **Origin** FastTab, in the **ZIP/postal code** field, enter
    **00210**. 

6.  In the **Destination** FastTab, in the **ZIP/postal code** field, enter
    **98052**. 

7.  In the **Result** FastTab, in the **Route plan** field, select **NH to
    WA**. 

8.  Close the form. 

### Initiate an Inbound Shipment 

You have been asked to create a new purchase order for 10 mini-speakers from the
Ade Supply Company. After creating the purchase order, you will need to create
an inbound shipment and then rate shop for the inbound load to find the cheapest
transportation rate. 

### Create a new purchase order. 

1.  Open **Accounts payable \> Purchase orders \> All purchase orders**. 

2.  Click **New** in the action pane. 

3.  On the **Create purchase order** form, in the **Vendor account** field,
    select **1003**. 

4.  In the **General** FastTab, in the **Site** field, select **6**. 

5.  In the **Warehouse** field, select **61**. 

6.  Click **OK**. 

7.  In the **Purchase order lines** FastTab, in the **Item number** field, enter
    **L0101**. 

8.  In the **Quantity** field, enter **10**. 

9.  In the **Unit price** field, enter **50**. 

10. In the **Purchase** tab on the action pane, click **Confirm**. 

### Create an inbound shipment. 

1.  In the **Warehouse** tab on the action pane, click **Load planning
    workbench**. 

2.  Select the check mark column for the purchase order line. 

3.  In the **Supply and demand** tab on the action pane, click **To new load**. 

4.  In the **Load template assignment** form, in the **Load template ID** field,
    select **Stnd Load template**. 

5.  Click **OK**. 

### Rate shop for the inbound load. 

1.  In the **Loads** tab of the Load planning workbench, select **Rate route
    workbench** from the **Rating and routing** drop-down menu. 

2.  In the action pane of the Rate route workbench, click **Rate shop**. 

3.  In the Route results FastTab, clear the **Hide exceptions** check box. 

4.  Select the **Route result** line for the route guide. 

5.  Click **Assign**. 

Process an Inbound Shipment 
----------------------------

Now that the inbound shipment has been created and rated, you need to schedule
an appointment for the mini-speaker shipment. You’ve also been asked to driver
Tim Smith in and out of the appointment. 

### Schedule an appointment. 

1.  Open **Transportation management \> Planning \> Load planning workbench**. 

2.  In the **Loads** tab, select the load ID for the purchase order created in
    the earlier practice. 

3.  Select **Appointment scheduling** from the **Transportation** drop-down
    menu. 

4.  In the **Appointment scheduling** form, click **New** in the action pane. 

5.  In the **Appointment details** FastTab, in the **Appointment rule** field,
    select **Inbound docks 61**. 

6.  Click **Save**.

7.  In the action pane, click the **Update status** drop-down arrow and select
    **Firm**. 

### Check the driver in. 

1.  In the action pane, click the **Update status** drop-down arrow and select
    **Driver check-in**. 

2.  In the **Driver check-in details** form, in the **Driver name** field, enter
    **Tim Smith**. 

3.  In the **Driver license** field, enter **123**. 

4.  Click **OK**. 

5.  Close the **Appointment scheduling** form. 

### Check the driver out. 

1.  Select **Appointment scheduling** in the **Transportation** drop-down menu. 

2.  In the **Appointment scheduling** form, in the action pane, click the
    **Update status** drop-down arrow and select **Driver check-out**. 

3.  In the **The driver’s information** form, click **OK** to accept the default
    information. 

4.  Close the form. 

Confirm an Inbound Shipment 
----------------------------

You now need to confirm the inbound load. 

### Confirm the inbound load. 

1.  Open **Transportation management \> Planning \> Load planning workbench**. 

2.  In the **Loads** tab, clear the **Hide shipped and received** check box. 

3.  Click the load ID. 

4.  In the **Load details** form, click the **Ship and receive** tab in the
    action pane, and then select **Inbound shipment** in the **Confirm** area. 

5.  Close the form. 

 

Exercise 5: Process outbound shipment 
======================================

Initiating an Outbound Shipment 
--------------------------------

You have been asked to confirm a sales order for Desert Wholesales, reserve
stock for the order, and create an outbound transportation load. 

### Receive and confirm the sales order. 

1.  Open **Sales and marketing \> Customers \> All customers**.  

2.  In the list of customers, select the line for account **US-007**. 

3.  In the action pane, click the **Sell** tab. 

4.  In the **New** area, click **Sales order**. 

5.  In the **Sales order** form, expand the **Sales order lines** FastTab, if
    not expanded already. 

6.  In the existing sales order line, in the **Item number** field, enter
    **A0001**. 

7.  In the **Quantity** field, enter **5**. 

8.  In the **Site** field, enter **6**. 

9.  In the **Warehouse** field, enter **62**. 

10. In the **Unit price** field, enter **15**.  

11. In the action pane, click **Save**. 

12. In the action pane, click the **Sell** tab. 

13. In the **Generate** area, click **Confirm sales order**. 

14. Confirm the information on the Confirm sales order form and click **OK**. 

15. Click **OK** to post without printing. 

###  Reserve stock for the order. 

1.  In the **Sales order details** form, select the order line in the **Sales
    order lines** FastTab. 

2.  Click the **Inventory** drop-down arrow and select **Reservation**. 

3.  In the **Reservation** form, in the **Reservation** field, enter **5**. 

4.  In the action pane, click **Reserve lot**. 

5.  Close the form. 

### Create an outbound transportation load. 

1.  In the **Sales order details** form, click the **Warehouse** tab in the
    action pane. 

2.  In the **Loads** area, click **Load planning workbench**. 

3.  In the **Sales lines** tab, select the line for your current sales order. 

4.  In the action pane, click **Supply and demand**. 

5.  In the **Add** area, click **To new load**. 

6.  In the **Load template assignment** form, select **Stnd Load Template** from
    the **Load template ID** drop-down menu. 

7.  Click **OK**. 

8.  Click **OK** to confirm exceeding capacity. 

Creating a Consolidated Shipment 
---------------------------------

Desert Wholesales wants to add another line to their sales order. They request
that both sales order lines arrive in one consolidated load. You have been
tasked with creating the consolidated load and confirming it. 

### Set up parameters for consolidated shipments. 

1.  Open **Transportation management \> Setup \> Transportation management
    parameters**. 

2.  Click the **General** tab. 

3.  In the **In transit planning** FastTab, set the **In transit planning**
    slider to **Yes**. 

4.  Close the form. 

### Add a new line to a sales order. 

1.  Open **Accounts receivable \> Orders \> All sales orders**. 

2.  Select the current sales order for Desert Wholesales. 

3.  In the **Sales order details** form, in the **Sales order lines** FastTab,
    click **Add line**. 

4.  In the **Item number** field, enter **A0002**. 

5.  In the **Quantity** field, enter **5**. 

6.  For **Site**, select **5**.

7.  In the action pane, click the **Sell** tab. 

8.  In the **Generate** area, click **Confirm sales order**. 

9.  Confirm the information on the Confirm sales order form and click **OK**. 

10. Click **OK** to post without printing. 

### Reserve stock for the order. 

1.  In the **Sales order details** form, select one of the order lines in the
    **Sales order lines** FastTab. 

2.  Click the **Inventory** drop-down arrow and select **Reservation**. 

3.  In the **Reservation** form, in the **Reservation** field, enter **5**. 

4.  In the action pane, click **Reserve lot**. 

5.  Close the form. 

### Create and confirm a new outbound load. 

1.  In the **Sales order details** form, click the **Warehouse** tab in the
    action pane. 

2.  In the **Loads** area, click **Load planning workbench**. 

3.  In the **Sales lines** tab, select a line for your current sales order. 

4.  In the action pane, click **Supply and demand**. 

5.  In the **Add** area, click **To new load**. 

6.  In the **Load template assignment** form, select **Stnd Load Template** from
    the **Load template ID** drop-down menu. 

7.  Click **OK**. 

8.  Click **OK** to confirm exceeding capacity. 

### Add hub consolidation and rate both loads. 

1.  In the **Load planning workbench**, select the first load you created in the
    **Loads** tab. 

2.  Select **Hub consolidation** in the **Transportation** drop-down menu. 

3.  In the **Override location** form, click the **Hub** drop-down arrow and
    select **Los Angeles**. 

4.  Click **OK**. 

5.  Select the load line in the **Loads** tab. 

6.  Select **Rate route workbench** from the **Rating and routing** drop-down
    menu. 

7.  In the **Rate route workbench**, click **Route with rate** in the action
    pane. 

8.  In the **Route Results** FastTab, select route guide **Wh 61 to Cust 003 004
    019**. 

9.  Click **Assign**. 

10. Close the **Routes** form and the **Rate route workbench**. 

11. Repeat steps **1–10** for the second load. 

### Create the consolidated load. 

1.  In the **Transportation request lines** tab, select both lines. 

2.  In the action pane, click the **Supply and demand** tab. 

3.  In the **Add** area, click **To new load**. 

4.  In the **Load template assignment** form, select **Stnd Load Template** from
    the **Load template ID** drop-down menu. 

5.  Click **OK**. 

6.  Click **OK** to confirm exceeding capacity. 

*Note:* The consolidated load may take several minutes to appear in the Loads
tab. 

### Rate the consolidated load. 

1.  In the **Loads** tab, select the consolidated load line. 

2.  Select **Rate route workbench** from the **Rating and routing** drop-down
    menu. 

3.  In the **Rate route workbench**, click **Route with rate** in the action
    pane. 

4.  In the **Route Results** FastTab, select route guide **Wh 61 to Cust 003 004
    019**. 

5.  Click **Assign**. 

6.  Close the **Routes** form and the **Rate route workbench**. 

### Confirm the consolidated load shipment. 

1.  On the **Loan planning workbench**, in the **Loads** tab, select the
    consolidated load line. 

2.  Select **Outbound load** in the **Ship and receive** drop-down menu. 

 

 

Exercise 6: Set up automatic freight reconciliation 
====================================================

Freight Reconciliation 
-----------------------

You have been tasked with setting up the system for Desert Wholesales for
freight reconciliation. 

### Create a freight reconciliation reason code for Overtime. 

1.  Open **Transportation management \> Setup \> Freight reconciliation \>
    Reconciliation reasons**. 

2.  Click **New**. 

3.  Type **OT** in the **Reconciliation reason code** field. 

4.  Type **Overtime** in the **Description** field. 

5.  Type **211650** in the **Debit account** field. 

6.  Select the **Pay the freight vendor** check box. 

7.  Close the form. 

### Verify the Freight bill type is configured. 

1.  Open **Transportation management \> Setup \> Freight reconciliation \>
    Freight bill type**. 

2.  Select the TL **Freight bill type**. 

3.  Verify the **Engine assembly** field is populated. 

4.  Verify that two records exist; one for Billing group ID and one for External
    code. 

5.  Close the form. 

### Create a freight bill type assignment for the Truck Carrier service. 

1.  Open **Transportation management \> Setup \> Freight reconciliation \>
    Freight bill type assignments**. 

2.  Click **New**. 

3.  Select **None** in the **Direction** field. 

4.  Select **Ground** in the **Mode** field. 

5.  Select **TruckCarrier** in the **Shipping carrier** field. 

6.  Select **TL** in the **Freight bill type** field. 

7.  Close the form. 

### Create a billing group named Duties. 

1.  Open **Transportation management \> Setup \> Freight reconciliation \>
    Billing Group**. 

2.  Click **New**. 

3.  Type **Duties** in the **Billing group** field. 

4.  Type **Duties** in the **Name** field. 

5.  Close the form. 

### Create an audit master for overtime. 

1.  Open **Transportation management \> Setup \> Freight reconciliation \> Audit
    master**. 

2.  Click **New**. 

3.  Enter **Overtime** in the **Audit master ID** field. 

4.  Select **TruckCarrier** in the **Shipping carrier** field. 

5.  Select **TL** in the **Freight bill type** field. 

6.  In the **Result** FastTab, select **OT** in the **Overpayment reason code**
    field. 

7.  Select **Damage claim** in the **Underpayment reason code** field. 

8.  Close the form. 

 

 

 

 

 

 

 

 

Exercise 7: Working with appointment scheduling 
================================================

Create a new appointment rule. 
-------------------------------

1.  Open **Transportation management \> Setup \> Appointment scheduling \>
    Appointment rules**. 

2.  Click **New**. 

3.  In the **Appointment rule** field, enter **Warehouse 24**. 

4.  In the **Site** field, select **2**. 

5.  In the **Warehouse** field, select **24**. 

6.  In the **Duration** field, enter **30**. 

7.  In the **Max. number of appointments** field, enter **5**. 

8.  In the **Item movement direction** field, select **Both**. 

9.  Close the form. 

Create and pick a new sales order. 
-----------------------------------

1.  Open **Accounts receivable \> Orders \> All sales orders**. 

2.  Click **New**. 

3.  In the **Customer account** field, select **US-003**. 

4.  Click **OK**. 

5.  Select Sales order in the action pane. 

6.  In the **Copy** area, click **From all**. 

7.  In the **Copy from all** form, select **00783**. 

8.  Click **OK**. 

9.  Close the form. 

10. In the Load planning workbench (Transportation management \> Planning \>
    Load planning workbench), in the Loads section, select the Load ID. 

11. Select **Release to warehouse** from the **Release** drop-down menu. You may
    need to scroll up in the Loads section. 

*Note: Use the Load ID generated by the above steps as the load to select for
the rest of the exercise.* 

Working with Appointment Scheduling 
------------------------------------

You have been instructed to create a new load assignment for an existing sales
order for Warehouse 24. 

### Create a new load assignment. 

1.  Open **Transportation management \> Planning \> Load planning workbench**. 

2.  In the **Loads** section, select Load ID \<\<prerequisite\>\>. 

3.  Select **Appointment scheduling** from the **Transportation** menu. 

4.  In the **Appointment scheduling** form, click **New** in the action pane. 

5.  In the **Appointment details** FastTab, in the **Appointment rule** field,
    select **Warehouse 24**. 

6.  Click Save.

7.  In the action pane, select **Firm** from the **Update status** drop-down
    menu. 

Check a Driver In 
------------------

You have been asked to create an instant appointment for driver Tom Anderson,
and then check him in for the appointment. 

### Create an instant appointment. 

1.  Open **Transportation management \> Planning \> Dock appointment scheduling
    \> Driver check-in and check-out**. 

2.  In the action pane, click the **Schedule an instant appointment** drop-down
    arrow. 

3.  In the **Appointment rule** field, select **Warehouse 24**. 

4.  Click **OK**. 

### Check in a driver for the instant appointment. 

1.  In the **Driver check-in and check-out** list page, select the appointment
    ID that has just been created. 

2.  In the action pane, click **Driver check-in**. 

3.  In the **Driver check-in details** form, in the **Shipping carrier** field,
    select **TruckCarrier**. 

4.  In the **Driver name** field, enter **Tom Anderson**. 

5.  In the **Driver license** field, enter **123**. 

6.  Click **OK**. 
