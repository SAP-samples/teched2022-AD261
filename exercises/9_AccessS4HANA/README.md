## Access S/4HANA Cloud System to View Sales Order

## Table of Contents
- [Overview](#overview)
- [Get Sales Order Number](#getsalesorder)
- [Open S/4HANA system](#opensystem)
- [Check Sales Order Created](#checksalesorder)
- [Summary](#summary)

## Overview <a name="overview"></a>

Once you have successfully run the business process, a sales order will be created in the backend S/4HANA cloud system. Now let us check if the sales order was created in the system with the given purchase order number and other details (as filled in the approval form).

## Get Sales Order Number <a name="getsalesorder"></a>

1. Once the Action is completed successfully, copy the sales order from **Process and Workflow Instances**
    - Goto **Monitor** section and click **Process and Workflow Instances**

      ![](images/AccessSystem_02c.png)

    - Click to filter **COMPLETED** instances

      ![](images/AccessSystem_02a.png)

    - Search for your Order Processing Instance
    - Click **EXECUTION LOG** tab
    - Check if the **Action** is completed
    - Open **CONTEXT** tab
    - Copy the sales order number
    > this is the sales order that is newly created in the backend S/4HANA system

    ![](images/AccessSystem_02b.png)

## Open S/4HANA system <a name="opensystem"></a>

2. Click to open [S/4HANA Cloud System](https://my401669.s4hana.cloud.sap/ui#Shell-home)

    - Username : AD261_XXX where XXX is the user number like AD261_000, AD261_001 etc.
    - Password: Acce$$teched22

      ![](images/AccessSystem_01a.png)

3. Select **Sales Orders** tab, and then click to open **Manage Sales Order** tile

    ![](images/AccessSystem_01.png)

## Check Sales Order Created <a name="checksalesorder"></a>

4. Enter the sales order number in **Sales Order**, click **Go**
    - once you find the sales order, click **>** to navigate to the sales order.  

    ![](images/AccessSystem_03a.png)

5. You can now explore the sales order to check Ship to Party, Expected Delivery Date etc.

    ![](images/AccessSystem_03.png)

## Summary
