# Circular88-KPI
Power Platform solution to manage, gather, report and track performance indicators (KPI). Designed for South African municipalities, based on Circular 88.

## Background
This is provided as a solution accelerator. It's a sample solution which is not supported by Microsoft or myself. Use as a starter to help you get going quickly with a solution for performance indicator management. It is based on Circular 88 requirements and Excel template. It is flexible so that it can be used for scenarios which dont align directly to Circular 88. This solution uses the Dataverse for storage, and has both a Model Driven application (for indicator defintion, settings, rules and more) and a Canvas application (for users to submit their data elements). 

## Features
Here is a list of core features of the solution

- 2
- 3
- 4

## How it works
There are 2 main applications which makeup this solution. 1 - Admin Model Driven App (Indicator Manager) 2 - User Indicator Canvas App. All data resides in the Microsoft Dataverse. There are a few Power Automate Flows which are used to notify users to submit their indicators, or to setup indicators, perform rollup calculations and more.

## Installation
There are 2 solution files which need to be imported into a Power Platform environment for the solution to work.
1 - Calculation Connector solution - this contains a custom connector only. This connector is used for C# based formula logic, and doesnt actually connect to any backend service. This must be imported first.
2 - Circular 88 solution - this contains the rest of the solution i.e. model driven app, canvas app, several flows, several tables, some web resources and a few custom roles.

Once imported, use the model driven apps setup section to add a default settings record, add Collection Business Unit records and Unit of Measure records. There are 3 custom roles which users will need to be assigend to i.e. Performance Indicator User, Performance Indicator Manager, and Performance Indicator Admin.


## Provided "As-Is"
This is a a starter / sample. It hasn't been well tested, and is missing some key features that I hope to add over time. It not officialy supported by myself or Microsoft. However, because the unmanaged and managed solution is provided, you should be able to support it yourself, either directly or through a certified Microsoft partner.
