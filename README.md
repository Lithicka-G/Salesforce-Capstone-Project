# WhatNext Vision Motors – Salesforce CRM Implementation

## 📌 Project Overview

**WhatNext Vision Motors** is a Salesforce-based CRM application developed to centralize and automate the core operations of a vehicle sales and service organization.

The application manages the complete vehicle business workflow, including **vehicle inventory, customers, dealers, vehicle orders, test drives, and service requests**. It combines Salesforce declarative tools such as **Flows, Validation Rules, Lightning App Builder, Reports, and Dashboards** with programmatic solutions using **Apex, Batch Apex, and Scheduled Apex**.

The project is designed to reduce manual processes, improve data accuracy, automate business operations, and provide better visibility into vehicle sales and service activities.

demo link : (https://drive.google.com/file/d/1KWASzmfZuBxdeIeaCt8DbMm4Q1Wspp4l/view?usp=sharing)

## 🎯 Objectives

- Centralize vehicle, customer, dealer, order, test-drive, and service information.
- Automate repetitive business processes using Salesforce Flow and Apex.
- Automatically assign suitable dealers to vehicle orders.
- Prevent vehicle orders when the selected vehicle is out of stock.
- Send automated reminders for upcoming test drives.
- Automatically process pending orders when stock becomes available.
- Provide reports and dashboards for management visibility.
- Maintain structured relationships between customers, vehicles, dealers, orders, and service requests.

## 🗂️ Core Salesforce Objects

The application consists of six main custom objects:

- **Vehicle** – Stores vehicle models, prices, stock quantities, and status.
- **Vehicle Dealer** – Maintains dealer information such as location, contact details, and email.
- **Vehicle Customer** – Stores customer information and preferred vehicle type.
- **Vehicle Order** – Represents customer orders for specific vehicles.
- **Vehicle Test Drive** – Manages test-drive bookings and schedules.
- **Vehicle Service Request** – Tracks service requests associated with vehicles and customers.

Lookup relationships connect these objects to maintain a consistent flow of information across the application.

## ⚙️ Key Automations

### 1. Automatic Dealer Assignment

A **Record-Triggered Flow** automatically identifies the appropriate dealer and assigns the dealer to a newly created Vehicle Order, reducing manual order routing.

### 2. Vehicle Stock Validation

An **Apex-based validation mechanism** prevents Vehicle Orders from being created or updated when the selected vehicle has zero available stock.

### 3. Test Drive Reminder

A **Record-Triggered Flow with a Scheduled Path** retrieves the customer's email address and sends an automated reminder before the scheduled test drive.

### 4. Pending Order Processing

**Batch Apex and Scheduled Apex** are used to periodically process pending orders and automatically confirm eligible orders once vehicle stock becomes available.

## 📊 Reports & Dashboards

The Salesforce application includes reports and dashboards to provide visibility into:

- Vehicle inventory
- Vehicle orders
- Sales activity
- Test drives
- Service requests
- Pending and completed business processes

These analytics help provide a centralized view of the organization's operations.

## 🛠️ Technologies & Salesforce Features

- Salesforce Lightning Platform
- Custom Objects & Fields
- Lookup Relationships
- Validation Rules
- Salesforce Flow Builder
- Record-Triggered Flows
- Scheduled Paths
- Apex
- Batch Apex
- Scheduled Apex
- Lightning App Builder
- Reports & Dashboards
- Salesforce Security & Permissions

## 🔄 Business Workflow

```text
Customer
   ↓
Vehicle Selection
   ↓
Test Drive / Vehicle Order
   ↓
Stock Validation
   ↓
Dealer Assignment
   ↓
Order Processing
   ↓
Vehicle Delivery
   ↓
Service Request
```
## 👩‍💻 Author

**Lithicka G**  
B.E. Computer Science and Design  
R.M.K. Engineering College
