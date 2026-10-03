# Week 1 — Topic 1: What is SAP?

## 1. SAP Meaning

SAP stands for:

**Systems, Applications, and Products in Data Processing**

SAP is an enterprise software system used by companies to manage and integrate their business operations.

---

## 2. What is ERP?

ERP stands for:

**Enterprise Resource Planning**

An ERP system connects different departments of a company using one integrated system.

Examples of departments:

- Sales
- Finance
- Purchasing
- Inventory
- Manufacturing
- Human Resources
- Supply Chain

### Main Goal of ERP

The main goal is to allow different departments to work using connected business data.

Example:

Customer places an order.

Flow:

Customer Order  
→ Inventory Check  
→ Warehouse Processing  
→ Delivery  
→ Billing  
→ Finance

---

## 3. Why Companies Use SAP

Companies use SAP because it provides:

- Centralized business data
- Integrated business processes
- Real-time information
- Better reporting
- Better control over business operations
- Reduced duplicate data
- Standardized business processes

---

## 4. SAP Full Stack Architecture

Basic SAP Full Stack flow:

User  
↓  
SAP Fiori / SAPUI5  
↓  
Service / API  
↓  
ABAP Business Logic  
↓  
CDS Data Model  
↓  
SAP HANA Database

### Layers

**Frontend**

SAPUI5 and Fiori are mainly used for user interfaces.

**Backend**

ABAP is mainly used for business logic.

**Data Modeling**

CDS is used to model and expose business data.

**Database**

SAP HANA stores and processes the data.

---

## 5. Important SAP Terms

| Term | Meaning |
|---|---|
| SAP | Enterprise business software ecosystem |
| ERP | Enterprise Resource Planning |
| S/4HANA | SAP's modern ERP system |
| SAP HANA | In-memory database platform |
| ABAP | SAP backend programming language |
| SAPUI5 | JavaScript framework for SAP applications |
| Fiori | SAP user experience and design system |
| BTP | SAP Business Technology Platform |
| CDS | Core Data Services |
| OData | Protocol used to expose business services and data |

---

## 6. Important SAP Modules

### FI — Financial Accounting

Used for:

- Accounting
- Financial transactions
- Customer payments
- Vendor payments
- Financial reports

### CO — Controlling

Used for:

- Cost control
- Cost centers
- Profitability analysis
- Internal accounting

### SD — Sales and Distribution

Used for:

- Customers
- Sales orders
- Deliveries
- Billing

### MM — Materials Management

Used for:

- Purchasing
- Suppliers
- Purchase orders
- Materials
- Inventory

### PP — Production Planning

Used for:

- Manufacturing
- Production planning
- Material requirements

### HCM — Human Capital Management

Used for:

- Employees
- Payroll
- HR processes

---

## 7. SAP Business Process Example

### Procurement Process

Requirement  
↓  
Purchase Requisition  
↓  
Purchase Order  
↓  
Goods Receipt  
↓  
Supplier Invoice  
↓  
Payment

### Sales Process

Customer Requirement  
↓  
Sales Order  
↓  
Delivery  
↓  
Goods Issue  
↓  
Billing  
↓  
Customer Payment

---

## 8. Business Object Concept

A business object represents a real business entity.

Examples:

- Customer
- Supplier
- Material
- Sales Order
- Purchase Order
- Invoice

Example:

Purchase Order

Header:
- Supplier
- Company Code
- Purchasing Organization
- Currency

Items:
- Material
- Quantity
- Price
- Plant

---

## 9. Important SAP Concept — Document Flow

SAP business transactions are connected through documents.

Example:

Sales Order  
→ Delivery  
→ Goods Issue  
→ Billing Document  
→ Accounting Document

This relationship between documents is called:

**Document Flow**

---

## 10. SAP Developer Mindset

A normal developer may think:

Database  
→ Backend  
→ API  
→ Frontend

An SAP developer should think:

Business Process  
→ Business Object  
→ Business Rules  
→ Authorization  
→ Data Model  
→ Backend Logic  
→ API  
→ Fiori UI

---

## 11. Key Point

SAP is not only about programming.

SAP development is mainly about:

**Understanding business processes and implementing or extending them using SAP technologies.**

Technologies include:

- ABAP
- CDS
- RAP
- OData
- SAPUI5
- Fiori
- SAP HANA
- SAP BTP

---

## Interview Question

**Q: What is SAP?**

SAP is an enterprise software platform used to integrate and manage business processes such as finance, sales, purchasing, inventory, manufacturing, and human resources in a centralized system.

**Q: What is ERP?**

ERP stands for Enterprise Resource Planning. It is a software system that integrates different departments and business processes of an organization.

**Q: Why is SAP called an integrated system?**

Because transactions in one business area can automatically affect other related areas such as inventory, finance, sales, and reporting.

---

## One-Line Revision

**SAP connects business processes, people, data, and technology inside one integrated enterprise system.**

# Week 1 — Topic 2: ERP and SAP S/4HANA

## ECC vs S/4HANA

### ECC
- Older SAP ERP
- Supports different databases
- More traditional data model
- SAP GUI centric
- Classical ABAP common

### S/4HANA
- Modern SAP ERP
- Designed for HANA
- Simplified data model
- Fiori-centric UX
- CDS, RAP, APIs and modern ABAP
- Stronger cloud and clean-core approach

### Why SAP moved to the HANA database
SAP moved to HANA to make enterprise processing faster, simplify the data model, and support real-time analytics and transactions on the same platform.

#### Traditional databases had limitations
Older ERP systems often depended on:
- disk-based storage
- many indexes
- aggregate tables
- precomputed totals
- separate reporting systems

#### HANA Capabilities
- In-memory means much of the active data can be processed directly from RAM instead of constantly reading from slower disk storage.
That allows very fast calculations and queries.
- HANA heavily uses column-oriented storage
- Columnar storage also makes compression very effective
- HANA allows SAP to perform much more operational analytics directly on the transactional data

#### HANA is powerful, but bad application design can still be slow.
For example:
- inefficient joins
- poor CDS design
- excessive data retrieval
- badly written ABAP
- missing filters
So developers still need to understand performance.


Basic S/4HANA architecture
On-premise vs cloud deployment
Where ABAP fits inside S/4HANA


