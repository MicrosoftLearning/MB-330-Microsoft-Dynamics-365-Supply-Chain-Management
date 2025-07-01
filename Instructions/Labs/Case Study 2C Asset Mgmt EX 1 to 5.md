---
lab:
    title: 'Case study 2C Asset management'
    module: 'Module 2: Implement inventory and asset management'
---
Case study 2C Asset management
=================================

In this case study, you will work with the Asset Management module to set up assets, functional locations, and maintenance requests for Munson's Pickles and Preserves Farm. You will create asset types, condition assessment templates, service levels, workers, and functional location lifecycle states and models.

Objectives
----------

- Create an asset type.

- Create a condition assessment template.

- Set up asset service levels.

- Create workers.

Exercise \#1 Set up assets
----------------------------

### Scenario
---------
You’ll set up new assets for Munson’s Pickles and Preserves Farm in Asset Management. In this task, you’ll configure "Forklift" as an asset within the system.

### Create an asset type

1. Go to **Asset management** \> **Setup** \> **Asset types** \> **Asset types**.

2. Select **New** to create a new asset type.

3. In the **Asset type** field, enter **Forklift1**.

4. In the **Name** field, enter **Forklift1**.

5. In the **Lifecycle state** section, select **Standard**.

6. In the **KPIS** section, set **Total** to **Yes**.

7. Select **Save**.

8. On the **Maintenance job types** FastTab, select **Calibration**, **Inspection**, **Lubrication**, **Preventive**, and **Repair** and then to the **Maintenance job types selected** section.

    > **Note** To select job types in the **Maintenance job types** FastTab, you must have created the **Maintenance job types**. In **Asset Management**, select **Setup** \> **Jobs** \> **Maintenance job types**.

9. Assign a **Counter for Production Hours**

10. Select and move **Counter for Production Hours** to the **Asset counters selected** section. You won’t be adding an Attribute type at this time.

11. Leave the **Condition assessments** FastTab blank for now.

12. Select **Save**.

### Create a condition assessment template

### Scenario
---------
You’re tasked with establishing a condition assessment template for Munson’s Pickles and Preserves Farm to monitor the noise levels of blender blades for any changes in volume. Follow these steps to add a condition assessment template.

1. Go to Asset anagement, select Setup, select Asset types, then select Condition assessment templates.
2. Select + New to create a new template.
3. In the Template field, enter Noise.
4. In the Name field, enter Noise.
5. On the Condition assessment lines FastTab, select the + Add .
6. In the Name field, enter No greater than 100 db.
7. In the Description field, enter No greater than 100 db.
8. In the Data type dropdown menu, select String.
9. On the Asset types FastTab, add the asset types that should be included on the condition assessment template. Select + Add and then select Air compressor.
10. Select Save.

### Set up asset service levels

### Scenario
---------
Asset service levels are used on maintenance requests and work orders to determine the priority of work orders during work order scheduling. In this task, you'll assign an asset service level to your air compressor.

To set up asset service levels, follow these steps:

1. Go to **Asset management**, select Setup, then select Asset service levels.

2. Select + New.

3. In the Functional location field, select PP-01.

4. In the Asset type field, select Air Compressor.

5. In the Work order type field, select Preventive.

6. In the Service Level field, select 3.

7. Save the new Asset service level.

### Create workers

### Scenario
---------
You must assign established workers to maintenance worker groups in the Human resources and Organization administration modules. You'll add a worker to the Electricians maintenance worker group so they can be assigned when their skills are needed.

1. Go to Asset Management, select Setup, select Workers, then select Workers.

2. Select + New.

3. In the Worker field, select Sara Thomas from the dropdown menu.

4. Set Active to Yes to schedule this worker on work orders.

5. On the Groups FastTab, select + Add.

6. In the Maintenance worker group field, select Electricians.

7. On the Functional locations FastTab, select + Add line.

8. In the Functional location field, select PP-01. Select this as the worker's Primary location.

9. Save the new worker.

### Set up product-model relations

1. Go to Asset management, select Setup, select Assets, then select Manufacturer and model.

2. Select + New to create a new product.

3. In the Manufacturer field, enter Sony.

4. In the Description field, enter Sony Pvt Lts.

5. On the Models FastTab, select + Add to create an asset model that’s related to the asset manufacturer.

6. In the Model field, enter XAV-AX0001.

7. In the Description field, enter Car play Android auto car.

8. In the Asset type field, select vehicle.

9. On the top menu bar, select Save.

Exercise #2 – Create a functional location lifecycle state and functional location lifecycle model
----------------------------

Objective
- Create a functional location lifecycle state and functional location lifecycle model.
The IT manager in USMF wants to know how to define the states that a functional location can go through, for example, created, active, and end of the lifecycle state.

The IT manager wants to view all functional locations, regardless of their lifecycle state, in the All functional locations list page. He also wants to change the state of a functional location by selecting it in the All functional locations list. You were called to help the IT manager perform these tasks.

You’ll assist the IT manager in doing the following:

- Create a functional location lifecycle state.

- Create a functional location lifecycle model.

### Create a functional location lifecycle state

1. Add a new functional lifecycle state for closed functional locations:

2. Go to Asset management, select Setup, select Functional locations, then select Lifecycle states.

3. On the Action pane, select + New  to create a new functional location lifecycle state.

4. In the Lifecycle state , enter Closed.

5. In the Name field, enter Closed – Not in use. 

    > [!**Note**]  
    > When you’re creating a new lifecycle state, the Lifecycle model field will not be populated. When this lifecycle state is added to a lifecycle model, this field automatically populates to show the number of lifecycle models that this state is included in.

6. Select the General FastTab, then set Active to Yes.

7. Set the Create asset toggle to No.

8. Set New sub locations to No.

9. Set Install assets at locations to No.

    > **Note** When initially building your lifecycle states, you won’t have any information yet to select from the Asset state > Lifecycle state dropdown menu until you've completed the full configuration for your assets, including the asset lifecycle states. Leave this field blank for now.

10. Select Save. Your new functional location lifecycle state has been created and activated.

11. Repeat steps 1-10 above to create an On Hold lifecycle state.

### Create a functional location lifecycle model

### Scenario
---------
When all the functional location lifecycle states have been created, you can then place these into groupings named functional location lifecycle models. As a reminder,  functional location lifecycle models establish the workflow for the various types of functional locations and their states.
Munson's Pickles and Preserves Farm need to create a new Quality location for a new lifecycle model.

1. Go to Asset management, select Setup, select Functional locations, then select Lifecycle models.

2. Select + New.

3. Enter the name of your Lifecycle model as Quality.

4. In the Name field, enter Quality review.

5. Select Save.

6. On the Lifecycle states FastTab, the active lifecycle states appear in the Lifecycle states remaining section at the left. Select the Active, On Hold, and Ended lifecycle states.

7. Select the right arrow button to move the selected lifecycle states to the Lifecycle states selected section.

8. Select Save.

9. Exit the Functional location lifecycle models page and then come back into it again. The Lifecycle states field on the Details FastTab will automatically be populated.

10. Lifecycle state updates tab on the Action pane.

11. Next to Active, select the Ended and On Hold states. These are the functional location lifecycle states that the Active lifecycle state can be changed to.

12. Next to Ended, select the Active checkbox. The Ended state can be changed to Active.

13. Next to On Hold, select the Active checkbox. The On Hold state can be changed to Active.

14. Select OK to save the changes.

Exercise #3 – Create functional location types
-----------------------------------------------

# Exercise #3 – Create Functional Location Types

Now you can set up a default functional location type and then set up a regular functional location type.

You need to establish a new functional location type for **Munson's Pickles and Preserves Farm** to manage the quality control of salsa. Your task is to add a new functional location.

---

## Create a Default Functional Location Type

A default functional location type must be established for use when new assets are created.

1. Go to **Asset management** > **Setup** > **Functional locations** > **Functional location types**.
2. Select **+ New** to create a new functional location type.
3. In the **Functional location type** field, enter `Default`.
4. In the **Name** field, enter `Default location`.
5. In the **LIFECYCLE STATE** section of the **General FastTab**, in the **Functional location lifecycle model** field, select `Standard`.
6. Set **Multiple assets** to `Yes`. This selection creates a default functional location.
7. On the top menu bar, select **Save**.

---

## Create a Functional Location Type

**Munson's Pickles and Preserves Farm** is taking the quality of its products seriously. The company has established a new location for its quality department.

Your next task is to create a new functional location type for the farm’s new **Quality** location.

1. Go to **Asset management** > **Setup** > **Functional locations** > **Functional location types**.
2. Select **+ New** to create a functional location type.
3. In the **Functional location type** field, enter `Office Building`.
4. In the **Name** field, enter `Quality office`.
5. In the **Functional location lifecycle model** dropdown menu, select `Quality`.
6. Set **Multiple assets** to `Yes`.
7. Set **Update asset dimension** to `Yes`.
8. Leave the **Asset type** field blank.
9. Select **Save**.


Exercise #4 – Set up work orders
----------------------------------



Exercise #2 – Set up maintenance request lifecycle states, models, and types
-----------------------------------------------------------------------