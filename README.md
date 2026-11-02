# Advanced Data Modeling Project | Microsoft Power BI

## 1. Project Overview

An advanced Power BI data modeling project focused on designing a structured, scalable, and reliable analytical data model using multiple fact tables and shared dimensions.

The project demonstrates how different business processes can be represented within a single semantic model, allowing data from sales, inventory, marketing campaigns, order fulfillment, and sales targets to be analyzed through connected dimensions.

The main objective was to understand how business processes, data granularity, relationships, and filtering behavior influence the quality and reliability of analytical reports.

## 2. Business Problem

Organizations often manage data across multiple business processes, such as sales, inventory, marketing, and order fulfillment.

Combining these datasets without a proper data model can lead to incorrect aggregations, ambiguous relationships, and unreliable analytical results.

This project addresses the challenge of building an integrated data model that connects different business processes while preserving their individual levels of detail.

Key questions addressed:

- How can multiple business processes coexist within one data model?
- How should Fact Tables and Dimension Tables be identified and structured?
- How can shared dimensions connect multiple Fact Tables?
- How should relationships and filter directions be configured?
- How can different date roles be handled?
- How can data access be controlled for different users?

## 3. Project Objectives

- Understand the business meaning and structure of available datasets.
- Identify the grain of each Fact Table.
- Distinguish between transactional facts and descriptive dimensions.
- Design a multi-fact data model using shared dimensions.
- Establish appropriate relationships between tables.
- Apply advanced modeling concepts.
- Create a dedicated Date Table.
- Develop core analytical measures.
- Implement Row-Level Security (RLS).

## 4. Data Model Architecture

The project uses a multi-fact data model with shared dimensions, following the principles of Fact Constellation (Galaxy Schema).

### Fact Tables

The model includes multiple business processes:

| Fact Table | Business Process |
|---|---|
| Fact Sales | Sales transactions |
| Fact Inventory | Inventory movements or stock information |
| Fact Campaign | Marketing campaign performance |
| Fact Orders Process | Order fulfillment and payment processes |
| Fact Sales Targets | Sales target tracking |

### Dimension Tables

| Dimension Table | Purpose |
|---|---|
| Dim Customer | Customer-related attributes |
| Dim Product | Product information and classification |
| Dim Date | Calendar and time analysis |
| Dim Geography | Geographic information |
| Dim Orders Flags | Order channels, status, and priority |
| Dim Campaign | Campaign information and attributes |

### Additional Modeling Components

- Fact Promotion Coverage: Supports relationships between promotional campaigns and products.
- Measures Table: Organizes analytical measures.
- Security Table: Supports user-based data access through RLS.

## 5. Advanced Data Modeling Concepts Applied

### Understanding Data Grain
Identified the level of detail represented by different Fact Tables to ensure that measures and aggregations are evaluated at the correct level.

### Shared Dimensions
Applied shared dimensions to connect multiple Fact Tables and enable analysis across different business processes.

### Relationships
Worked with:
- Cardinality (One-to-Many and other relationship types where appropriate).
- Cross-filter direction.
- Active and inactive relationships.
- Relationship paths between Fact and Dimension Tables.

### Role-Playing Dimensions
Applied the concept of using one dimension for multiple business roles, particularly when working with different date fields.

### Bridge Tables
Worked with bridge-table concepts to support more complex relationships between business entities.

### Special Fact Table Types
Explored different fact table patterns and how they represent different business processes.

### Date Table
Created a dedicated Date Table to support consistent time-based analysis.

## 6. Measures & Analytical Calculations

Created a dedicated Measures Table to organize DAX measures and support analytical calculations.

The model was designed to support measures across different business processes while maintaining appropriate filter context.

## 7. Row-Level Security (RLS)

Implemented Row-Level Security to control data visibility based on user access.

The security setup uses a security table containing user email and region information to support region-based data access.

## 8. Technical Skills & Tools

- Microsoft Power BI
- Advanced Data Modeling
- Fact Constellation / Galaxy Schema
- Fact and Dimension Tables
- Data Grain Analysis
- Shared Dimensions
- Bridge Tables
- Role-Playing Dimensions
- Relationship Management
- Cardinality & Filter Direction
- Active & Inactive Relationships
- DAX Measures
- Date Table Design
- Row-Level Security (RLS)

## 9. Key Learning Outcomes

This project strengthened my understanding that effective data modeling starts with understanding business processes rather than simply connecting tables.

Key takeaways:

- Understanding the grain of each Fact Table is essential for accurate analysis.
- Shared dimensions provide a structured way to analyze multiple business processes.
- Relationship design directly affects filtering behavior and analytical results.
- Different fact table types require different modeling considerations.
- Security should be considered as part of the data model design.

## 10. Project Deliverables

- Power BI Semantic Data Model
- Multiple Fact and Dimension Tables
- Shared Dimension Architecture
- Dedicated Date Table
- Organized DAX Measures
- Row-Level Security Implementation
