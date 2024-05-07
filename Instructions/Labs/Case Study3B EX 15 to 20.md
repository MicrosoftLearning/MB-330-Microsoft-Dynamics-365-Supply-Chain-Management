---
lab:
    title: 'Case study 3B Transportation management'
    module: 'Module 4: Implement warehouse management and transportation management '
---
Case study 3B Transportation management
===============================================================

Objectives
----------

- Implement transportation management


Exercise \#1 Configure carriers
--------------------------------

*Objective: Set up a new carrier and add a carrier service.*

**USMF** in the United States has a new customer located in Europe.

The Transportation coordinator at Contoso Entertainment, has determined that a
new company will be used for transporting the products to this customer.

You will need to do the following:

- Set up a new ocean carrier.

- Add a carrier service to the carrier.

### Set up a new carrier

1. In USMF, Open **Transportation management** \> **Setup** \> **Carriers** \> **Shipping
carriers**.  

2. In the action pane, select **New** to create a new shipping carrier.  

3. In the **Shipping carrier** field, enter **Ocean Carrier 2**.

4. In the **Name** field, enter **Secondary ocean carrier**.

5. In the **Mode** field, select **Ocean**.  

6. Expand the **Overview** FastTab.

7. Set the **Activate shipping carrier** slider to **Yes**.

8. Select vendor account **1002** from the **Vendor** drop-down menu.  

9. In the **SCAC** field, enter **2005.**

10. Set the **Activate carrier rating** slider to **Yes.**

11. On the **Addresses** FastTab, select **New**.

12. In the **New address** form, enter **Ocean carrier location** in the **Name**
    field.

13. Select **Business** from the **Purpose** drop-down list.

14. Select USA in the Country/region drop-down list.

15. In the **ZIP/postal code** field, enter **11251**.

16. In the **Street** field, enter **1577 Madison Blvd**.

17. Set the **Primary** slider to **Yes**.

18. Select **OK.**

19. Close the **Shipping carriers** form.

### Add a carrier service to the carrier

1. Open **Transportation management \> Setup \> Carriers \> Shipping
    carriers.**

2. Select **Ocean Carrier 2** in the left-hand pane.

3. Expand the **Services** FastTab.

4. Select **New.**

5. In the **Carrier service** field, enter **Ocean**.  

6. In the **Name** field, enter **Ocean**.

7. In the **Transportation method** field, select **Ocean**.

8. Select **Freight** from the **Billing group ID** drop-down menu.

9. Close the form.

Exercise \#2 Configure rate masters
------------------------------------

*Objective: Configure a rate master and base.*

To support the logistics & transportation manager for **USMF**, you were asked
to record the rates for an air carrier.

This is done by setting up the rate masters according to the contracts signed
with the carriers

You will need to do the following:

- Setup the rate master.

- Set up the rate base.

- Assign the rate base.

### Set up rate master

1. Go to **Transportation management \> Setup \> Rating \> Rate master.**

2. Select **New**.

3. In the Rate master field, enter **AtlantaMaster**.

4. In the Name field, enter **Atlanta rate master**.

5. In the Rating metadata ID field, select the drop-down button to open the
    lookup.

    - The rating metadata ID will determine the data needed for the rate
        master, as it defines the metadata expected by the TMS engine using this
        rate master.

6. For this example, select the **P2P** option.

7. Select Save.

### Set up rate base

1. Select **Rate base**.

    - The rate base determines the rate of the carrier and can be used to set
        up a tariff structure as it structures the rates in the breakpoints
        defined in the break master.

2. Select **New**.

3. In the **Rate base** field, enter **AtlantaBase**.

4. In the **Name field**, enter **Atlanta rate base**.

5. In the **Break master** field, select the drop-down button to open the
    lookup.

    - Break masters are used to define the pricing structure and its
        breakpoints. The pricing structure uses tiered pricing that is based on
        physical dimensions.

For this example, use **weight.**

1. Toggle the expansion of the **Details** section.

2. Select **New**.

3. In the **Drop-off Postal Code From** field, enter **30301**.

4. In the **Drop-off Postal Code To** field, enter **30318**.

5. In the **Drop-off Country Region** field, enter **USA**.

6. In the **\<1.00 Lbs** field, enter **100**.

    - Insert the rate per lbs if the total weight of the load is less than 1
        pound.

7. In the **\<5.00 Lbs** field, enter **300**.

    - Insert the rate per lbs if the total weight of the load is less than 5
        pounds.

8. In the **\<20.00 Lbs** field, enter **500**.

    - Insert the rate per lbs if the total weight of the load is less than 20
        pounds.

9. In the **\<100.00** Lbs field, enter **1000**.

    - Insert the rate per lbs if the total weight of the load is less than 100
        pounds.

10. In the **\<1,000.00** Lbs field, enter **3000**.

    - Insert the rate per lbs if the total weight of the load is less than
        1000 pounds.

11. Select **Save**.

12. Close the page.

### Assign rate base

1. Toggle the expansion of the **Rate base assignments** section.

2. Select **New**.

    - You can have several rate base assignments for each rate master. This
        makes it possible to create several different price points for each
        carrier depending on destinations, services, or different rate bases. In
        this procedure you will only create one rate base assignment.

3. In the Name field, enter **AtlantaRateAssignment**.

4. In the Rate base field, select the drop-down button to open the lookup.

5. In the list, select **AtlantaBase**.

6. In the Service field, select the drop-down button to open the lookup.

7. In the list, find and select **Truck**.

8. In the Pick-up Postal Code field, enter **98052**.

    - Specify which postal code this rate base assignment should be valid
        from.

9. In the **Pick-up Country Region** field, enter **USA**.

10. Select **Save**.

Exercise \#3 Setup route plans and route guides (Bonus)
--------------------------------------------------------

*Objective: Configure a route pan, hub, and route guide.*

You were asked to help the logistics manager at **USMF** to setup route plans
and route guides.

You will need to do the following:

- Configure a new route plan for Georgia to Los Angeles.

- Create a new hub for the warehouses at Georgia and Los Angeles.

- Add details to the route plan.

- Create a route guide for Georgia to Los Angeles.

### Create a new route plan named “GA to LA”

1. Open **USMF \> Transportation management \> Setup \> Routing \> Route
    plans.**  

2. Select **New**.

3. In the **Route plan** field, enter **GA to LA**.

4. In the **Name** field, enter **Georgia to Los Angeles**.

5. Close the form.

### Create a new hub for Georgia and one for Los Angeles

1. Open **Transportation management \> Setup \> Routing \> Hub masters**.  

2. Select **New**.  

3. In the **Hub** field, enter **Georgia 3**.

4. In the **Name** field, enter **Savannah GA**.

5. Expand the **Codes** FastTab.

6. In the **Hub type** field, select Hub.

7. In the **Rate master** field, select **TruckRateMaster**.  

8. Expand the **Effective dates** FastTab.

9. In the **Effective start date and time** field, select **Today**.

10. In the **Effective end date and time** field, select **12/31/2025**.

11. Expand the **Address** FastTab.

12. Select **Add**.

13. In the **Name or description** field, enter **Georgia 3**.

14. In the **Zip/postal code** field, enter **31302**.

15. In the **Street** field, enter **123 ABC Street**.

16. Select **OK**.

17. Select **New**.  

18. In the **Hub** field, enter **Los Angeles 2**.

19. In the **Name** field, enter **Los Angeles CA 2**.

20. Expand the **Codes** FastTab.

21. In the **Hub type** field, select Hub.

22. In the **Rate master** field, select **TruckRateMaster**.  

23. Expand the **Effective dates** FastTab.

24. In the **Effective start date and time** field, select **Today**.

25. In the **Effective end date and time** field, select **12/31/2025**.

26. Expand the **Address** FastTab.

27. Select **Add**.

28. In the **Name or description** field, enter **Los Angeles 2**.

29. In the **Zip/postal code** field, enter **90001**.

30. In the **Street** field, enter **987 XYZ Avenue**.

31. Select **OK**.

32. Close the form.

### Add details to the route plan

1. Open **Transportation management \> Setup \> Routing \> Route plans.**  

2. Select the **GA to LA** route plan.

3. On the **Details** FastTab, select **New**.  

4. In the **Origin hub** field, select **Georgia 3**.

5. In the **Destination hub** field, select **Los Angeles 2**.

6. In the **Shipping carrier** field, select **TruckCarrier**.

7. In the **Carrier service** field, select **Truck**.

8. Close the form.

### Create a route guide

You must configure a new routing guide for Georgia to Los Angeles. The routing
guide should use a particular shipping carrier, TruckCarrier, with the carrier
service Truck.  

### Create a new routing guide named “GA to LA”

1. In **USMF**, go to **Transportation management** \> **Setup** \> **Routing** \> **Route guides.**  

2. Select **New**.

3. In the **Routing guide** field, enter **GA to LA**.

4. In the **Name** field, enter **Georgia to Los Angeles**.  

### Add Information, Origin, Destination, and Result entities to the routing guide

1. Expand the **Information** FastTab.

2. In the **Direction** field, select **Outbound**.  

3. Set the **Active** slider to the **Yes** position.

4. In the **Effective start date and time** field, select **Today**.

5. In the **Effect end date and time** field, enter **12/31/2025**.

6. Expand the **Origin** FastTab.

7. In the **Zip/postal code** field, enter **31302**.

8. In the **Hub** field, select **Los Angeles 2**.

9. In the **Country/region** field, enter **USA**.

10. Expand the **Destination** FastTab.

11. In the **Zip/postal code from** field, enter **31302**.

12. In the **Zip/postal code to** field, enter **90001**.

13. In the **Hub** field, select **Georgia 3**.

14. In the **Country/region** field, enter **USA**.

15. Expand the **Result** FastTab.

16. In the **Shipping carrier** field, select **TruckCarrier**.

17. In the **Carrier service** field, select **Truck**.

18. Select **Save**.

Exercise \#4 Process inbound shipments (Bonus)
-----------------------------------------------

*Objective: Configure a route and manage inbound shipments.*

You were asked to help the logistics manager at USMF, to manage the inbound
shipments from Ade Supply Company.

You will need to do the following:

- Complete the prerequisite steps.

- Create a hub, route plan, and route guide.

- Initiate an inbound shipment.

- Process an inbound shipment.

- Confirm an inbound shipment.

### Add a vendor address for the Ade Supply Company

1. Open **Accounts payable \> Vendors \> All vendors**.

2. Select vendor **1003** from the list of vendors.

3. In the action pane, select **Edit**.

4. In the **Addresses** FastTab, select **Add**.

5. In the **Name or description** field, enter **Ade Supply Main Location**.

6. In the **Zip/postal code** field, enter **00210**.

7. In the **Street** field, enter **123 Main Street**.

8. Set the **Primary** slider to **Yes**.

9. Select **OK**.

10. In the **Invoice and delivery** FastTab, in the **Mode of delivery** field,
    select **Parce-STD**.

11. Close the forms.

### Modify the CFR terms of delivery

1. Open **Accounts payable \> Setup \> Terms of delivery**.

2. Select **CFR** from the left-hand panel.

3. Select **Edit** in the action pane.

4. In the **Transportation** FastTab, set the **Add transportation charges to
    retail sales orders** slider to **Yes**.

5. Close the form.

### Create a Hub, Route Plan, and Route Guide

You have been asked to set up a hub for the Ade Supply Company and create a
route plan and guide between the Ade Supply Company and USMF’s Warehouse 61.

### Create a hub for the Ade Supply Company

1. Open **Transportation management \> Setup \> Routing \> Hub masters**.

2. Select **New** in the action pane.

3. In the **Hub** field, enter **Ade Supply.**

4. In the **Name** field, enter **Ade Supply NH**.

5. In the **Codes** FastTab, in the **Hub type** field, select **Hub**.

6. In the **Rate master** field, select **ParcelRateMaster**.

7. In the **Address** FastTab, select **Add**.

8. In the **New address** form, in the **Name or description** field, enter
    **Ade Supply NH**.

9. In the **ZIP/postal code** field, enter **00210**.

10. In the **Street** field, enter **123 Main Street**.

11. Select **OK**.

12. Close the form.

### Create a route plan from New Hampshire to Washington

1. Open **Transportation management \> Setup \> routing \> Route plans**.

2. Select **New** in the action pane.

3. In the **Route plan** field, enter **NH to WA**.

4. In the **Name** field, enter **New Hampshire to Washington**.

5. In the **Details** FastTab, select **New**.

6. In the **Origin hub** field, select **Ade Supply**.

7. In the **Destination hub** field, select **Own WHS**.

8. In the **Shipping carrier** field, select **ParcelCarrier**.

9. In the **Carrier service** field, select **STD**.

10. In the **Vendor** field, select **1003**.

11. Close the form.

### Create a route guide from New Hampshire to Washington

1. Open **Transportation management \> Setup \> Routing \> Route guides**.

2. Select **New** in the action pane.

3. In the **Routing guide** field, enter **NH to WA**.

4. In the **Name** field, enter **New Hampshire to Washington**.

5. In the **Origin** FastTab, in the **ZIP/postal code** field, enter
    **00210**.

6. In the **Destination** FastTab, in the **ZIP/postal code** field, enter
    **98052**.

7. In the **Result** FastTab, in the **Route plan** field, select **NH to
    WA**.

8. Close the form.

### Initiate an Inbound Shipment

You have been asked to create a new purchase order for 10 mini-speakers from the
Ade Supply Company. After creating the purchase order, you will need to create
an inbound shipment and then rate shop for the inbound load to find the cheapest
transportation rate.

### Create a new purchase order

1. Open **Accounts payable \> Purchase orders \> All purchase orders**.

2. Select **New** in the action pane.

3. On the **Create purchase order** form, in the **Vendor account** field,
    select **1003**.

4. In the **General** FastTab, in the **Site** field, select **6**.

5. In the **Warehouse** field, select **61**.

6. Select **OK**.

7. In the **Purchase order lines** FastTab, in the **Item number** field, enter
    **L0101**.

8. In the **Quantity** field, enter **10**.

9. In the **Unit price** field, enter **50**.

10. In the **Purchase** tab on the action pane, select **Confirm**.

### Create an inbound shipment

1. In the **Warehouse** tab on the action pane, select **Load planning
    workbench**.

2. Select the check mark column for the purchase order line.

3. In the **Supply and demand** tab on the action pane, select **To new load**.

4. In the **Load template assignment** form, in the **Load template ID** field,
    select **Stnd Load template**.

5. Select **OK**.

### Rate shop for the inbound load

1. In the **Loads** tab of the Load planning workbench, select **Rate route
    workbench** from the **Rating and routing** drop-down menu.

2. In the action pane of the Rate route workbench, select **Rate shop**.

3. In the Route results FastTab, clear the **Hide exceptions** check box.

4. Select the **Route result** line for the route guide.

5. Select **Assign**.

### Process an Inbound Shipment

Now that the inbound shipment has been created and rated, you need to schedule
an appointment for the mini-speaker shipment. You’ve also been asked to schedule
driver Tim Smith in and out of the appointment.

### Schedule an appointment

1. Open **Transportation management \> Planning \> Load planning workbench**.

2. In the **Loads** tab, select the load ID for the purchase order created in
    the earlier practice.

3. Select **Appointment scheduling** from the **Transportation** drop-down
    menu.

4. In the **Appointment scheduling** form, select **New** in the action pane.

5. In the **Appointment details** FastTab, in the **Appointment rule** field,
    select **Inbound docks 61**.

6. Select **Save**.

7. In the action pane, select the **Update status** drop-down arrow and select
    **Firm**.

### Check the driver in

1. In the action pane, select the **Update status** drop-down arrow and select
    **Driver check-in**.

2. In the **Driver check-in details** form, in the **Driver name** field, enter
    **Tim Smith**.

3. In the **Driver license** field, enter **123**.

4. Select **OK**.

5. Close the **Appointment scheduling** form.

### Check the driver out

1. Select **Appointment scheduling** in the **Transportation** drop-down menu.

2. In the **Appointment scheduling** form, in the action pane, select the
    **Update status** drop-down arrow and select **Driver check-out**.

3. In the **The driver’s information** form, select **OK** to accept the default
    information.

4. Close the form.

### Confirm an Inbound Shipment

You now need to confirm the inbound load.

### Confirm the inbound load

1. Open **Transportation management \> Planning \> Load planning workbench**.

2. In the **Loads** tab, clear the **Hide shipped and received** check box.

3. Select the load ID.

4. In the **Load details** form, select the **Ship and receive** tab in the
    action pane, and then select **Inbound shipment** in the **Confirm** area.

5. Close the form.

Exercise \#5 Process outbound shipments
----------------------------------------

*Objective: Manage an outbound shipment and a consolidated shipment*

The logistics manager at USMF, would like to process an outbound shipment for
Desert Wholesales.

This involves receiving and confirming the sales order, reserving stock for the
order, and creating an outbound transportation load.

In addition, Desert Wholesales wants to add another line to their sales order.

They requested that both sales order lines arrive in one consolidated load.

You have been asked to help creating the consolidated load and confirming it.

You need do the following:

- Initiate an outbound shipment.

- Create a consolidated shipment.
    > **NOTE** There's an exclusion on sales orders lesser than $10,000 for all customers. The sales order may provide an informational message that the order amount may be less than or equal to the sales order exclusion amount in the sales order rule and will not be sent to credit management. Before the execution of this task, view blocking rules and exclusion rules on the **Credit and collections** > **Setup** > **Credit management setup** > **Blocking rules page**.

### Initiating an Outbound Shipment

You have been asked to confirm a sales order for Desert Wholesales, reserve
stock for the order, and create an outbound transportation load.

### Receive and confirm the sales order

1. Open **Sales and marketing \> Customers \> All customers**.  

2. In the list of customers, select the line for account **US-007**.

3. In the action pane, select the **Sell** tab.

4. In the **New** group, select **Sales order**.

5. In the **Sales order** form, expand the **Sales order lines** FastTab, if
    not expanded already.

6. In the existing sales order line, in the **Item number** field, enter
    **A0001**.

7. In the **Quantity** field, enter **5**.

8. In the **Site** field, enter **6**.

9. In the **Warehouse** field, enter **62**.

10. In the **Unit price** field, enter **15**.  

11. In the action pane, select **Save**.

12. In the action pane, select the **Sell** tab.

13. In the **Generate** area, select **Confirm sales order**.

14. Confirm the information on the **Confirm sales order** form and select
    **OK**.

15. Select **OK** to post without printing.

### Reserve stock for the order

1. In the **Sales order details** form, select the order line in the **Sales
    order lines** FastTab.

2. Select the **Inventory** drop-down arrow and select **Reservation**.

3. In the **Reservation** form, in the **Reservation** field, enter **5**.

4. In the action pane, select **Reserve lot**.

5. Close the form.

### Create an outbound transportation load

1. In the **Sales order details** form, select the **Warehouse** tab in the
    action pane.

2. In the **Loads** area, select **Load planning workbench**.

3. In the **Sales lines** tab, select the line for your current sales order.

4. In the action pane, select **Supply and demand**.

5. In the **Add** area, select **To new load**.

6. In the **Load template assignment** form, select **Stnd Load Template** from
    the **Load template ID** drop-down menu.

7. Select **OK**.

8. Select **OK** to confirm exceeding capacity.

### Creating a Consolidated Shipment

Desert Wholesales wants to add another line to their sales order. They request
that both sales order lines arrive in one consolidated load. You have been
tasked with creating the consolidated load and confirming it.

### Set up parameters for consolidated shipments

1. Open **Transportation management \> Setup \> Transportation management
    parameters**.

2. Select the **General** tab.

3. In the **In transit planning** FastTab, set the **In transit planning**
    slider to **Yes**.

4. Close the form.

### Add a new line to a sales order

1. Open **Accounts receivable \> Orders \> All sales orders**.

2. Select the current sales order for Desert Wholesales.

3. In the **Sales order details** form, in the **Sales order lines** FastTab,
    select **Add line**.

4. In the **Item number** field, enter **A0002**.

5. In the **Quantity** field, enter **5**.

6. For **Site**, select **5**.

7. In the action pane, select the **Sell** tab.

8. In the **Generate** area, select **Confirm sales order**.

9. Confirm the information on the Confirm sales order form and select **OK**.

10. Select **OK** to post without printing.

### Reserve stock for the order

1. In the **Sales order details** form, select one of the order lines in the
    **Sales order lines** FastTab.

2. Select the **Inventory** drop-down arrow and select **Reservation**.

3. In the **Reservation** form, in the **Reservation** field, enter **5**.

4. In the action pane, select **Reserve lot**.

5. Close the form.

### Create and confirm a new outbound load

1. In the **Sales order details** form, select the **Warehouse** tab in the
    action pane.

2. In the **Loads** area, select **Load planning workbench**.

3. In the **Sales lines** tab, select a line for your current sales order.

4. In the action pane, select **Supply and demand**.

5. In the **Add** area, select **To new load**.

6. In the **Load template assignment** form, select **Stnd Load Template** from
    the **Load template ID** drop-down menu.

7. Select **OK**.

8. Select **OK** to confirm exceeding capacity.

### Add hub consolidation and rate both loads

1. In the **Load planning workbench**, select the first load you created in the
    **Loads** tab.

2. Select **Hub consolidation** in the **Transportation** drop-down menu.

3. In the **Override location** form, select the **Hub** drop-down arrow and
    select **Los Angeles**.

4. Select **OK**.

5. Select the load line in the **Loads** tab.

6. Select **Rate route workbench** from the **Rating and routing** drop-down
    menu.

7. In the **Rate route workbench**, select **Route with rate** in the action
    pane.

8. In the **Route Results** FastTab, select route guide **Wh 61 to Cust 003 004
    019**.

9. Select **Assign**.

10. Close the **Routes** form and the **Rate route workbench**.

11. Repeat steps **1–10** for the second load.

### Create the consolidated load

1. In the **Transportation request lines** tab, select both lines.

2. In the action pane, select the **Supply and demand** tab.

3. In the **Add** area, select **To new load**.

4. In the **Load template assignment** form, select **Stnd Load Template** from
    the **Load template ID** drop-down menu.

5. Select **OK**.

6. Select **OK** to confirm exceeding capacity.

*Note:* The consolidated load may take several minutes to appear in the Loads
tab.

### Rate the consolidated load

1. In the **Loads** tab, select the consolidated load line.

2. Select **Rate route workbench** from the **Rating and routing** drop-down
    menu.

3. In the **Rate route workbench**, select **Route with rate** in the action
    pane.

4. In the **Route Results** FastTab, select route guide **Wh 61 to Cust 003 004
    019**.

5. Select **Assign**.

6. Close the **Routes** form and the **Rate route workbench**.

### Confirm the consolidated load shipment

1. On the **Load planning workbench**, in the **Loads** tab, select the
    consolidated load line.

2. Select **Outbound load** in the **Ship and receive** drop-down menu.

Exercise \#6 Configure freight reconciliation (Bonus)
------------------------------------------------------

*Objective: Configure and manage freight reconciliation.*

You were asked to help the logistics manager at **USMF**, to setup the system
for Desert Wholesales for freight reconciliation.

You will need to do the following:

- Create the freight reconciliation reason code for overtime.

- Verify that the fright bill type is configured.

- Create a freight bill type assignment for the truck carrier service.

- Create a billing group named Duties.

- Create an audit master for overtime.

### Create a freight reconciliation reason code for Overtime

1. Open **Transportation management \> Setup \> Freight reconciliation \>
    Reconciliation reasons**.

2. Select **New**.

3. Type **OT** in the **Reconciliation reason code** field.

4. Type **Overtime** in the **Description** field.

5. Type **211650** in the **Debit account** field.

6. Select the **Pay the freight vendor** check box.

7. Close the form.

### Verify the Freight bill type is configured

1. Open **Transportation management \> Setup \> Freight reconciliation \>
    Freight bill type**.

2. Select the TL **Freight bill type**.

3. Verify the **Engine assembly** field is populated.

4. Verify that two records exist, one for Billing group ID and one for External
    code.

5. Close the form.

### Create a freight bill type assignment for the Truck Carrier service

1. Open **Transportation management \> Setup \> Freight reconciliation \>
    Freight bill type assignments**.

2. Select **New**.

3. Select **None** in the **Direction** field.

4. Select **Ground** in the **Mode** field.

5. Select **TruckCarrier** in the **Shipping carrier** field.

6. Select **TL** in the **Freight bill type** field.

7. Close the form.

### Create a billing group named Duties

1. Open **Transportation management \> Setup \> Freight reconciliation \>
    Billing Group**.

2. Select **New**.

3. Type **Duties** in the **Billing group** field.

4. Type **Duties** in the **Name** field.

5. Close the form.

### Create an audit master for overtime

1. Open **Transportation management \> Setup \> Freight reconciliation \> Audit
    master**.

2. Select **New**.

3. Enter **Overtime** in the **Audit master ID** field.

4. Select **TruckCarrier** in the **Shipping carrier** field.

5. Select **TL** in the **Freight bill type** field.

6. In the **Result** FastTab, select **OT** in the **Overpayment reason code**
    field.

7. Select **Damage claim** in the **Underpayment reason code** field.

8. Close the form.
