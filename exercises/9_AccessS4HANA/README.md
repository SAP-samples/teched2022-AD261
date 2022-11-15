## Access S/4HANA Cloud System to View Sales Order

## Table of Contents
- [Overview](#overview)
- [Get Sales Order Number](#getsalesorder)
- [Open S/4HANA system](#opensystem)
- [Check Sales Order Created](#checksalesorder)
- [Summary](#summary)

## Overview <a name="overview"></a>

Once you have successfully run the business process, a sales order will be created in the backend S/4HANA cloud system. Now let us check if the sales order was actually created in the system with the given purchase order number and other details (as filled in the approval form).

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

    | Username    | Password     |
    | :------------- | :------------- |
    | AD261_XXX <br> where XXX is the user number <br>like AD261_000, AD261_001 etc.      | Acce$$teched22     |

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

Action is a feature in **SAP Process Automation** to connect processes with external systems, be it SAP or non-SAP systems. This is an important piece of the puzzle especially if you want to automate or extend your business processes for any available LoB processes like S/4HANA, Ariba, SuccessFactors etc. These extensions can be easily build using SAP Process Automation, and using Actions you can connect to your given S/4HANA, Ariba or other SAP LoB systems for any kind of GET, POST, PATCH and other calls.

In this workshop, you learnt how to:
- [x] Create, configure and test Action Project
- [x] Publish various actions from action project in Action Library
- [x] Add action published in Action Library in business process
- [x] Configure action inputs with the business process outputs.
- [x] Release, Deploy and Run business process with connectivity to the backend system.
- [x] Check backend system for newly created  business object.

The same scenario can be used for posting an invoice to the S/4HANA system after approval from business process or getting the employee details from SuccessFactors system for off-boarding process or updating purchase requisition details for the changes in the order in Ariba system or getting asset details from Asset Management system before sending it for approval for asset depreciation. There are many such real-world examples where you can use Action concept to create, fetch or update the data in the backend system based on the process outcomes (approval, validation etc.)
