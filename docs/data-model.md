# Data Model

## Overview

A star schema data model was implemented to ensure optimal performance and scalability.

## Fact Table: FactPedidos

This table contains transactional data at the order level.

### Columns:

* Order ID: Unique identifier of each order
* Order Date: Date when the order was placed
* Ship Date: Date when the order was shipped
* Sales: Revenue generated
* Profit: Net profit
* Discount: Applied discount
* Quantity: Units sold
* Shipping Cost: Cost of shipping

## Dimension Tables

### DimCliente

* Customer ID
* Customer Name
* Segment
* Region

### DimProducto

* Product ID
* Category
* Sub-Category

### DimFecha

* Date
* Year
* Month
* Month Name
* Quarter

### DimEnvio

* Ship Mode

## Relationships

* FactPedidos[Customer ID] → DimCliente[Customer ID]
* FactPedidos[Product ID] → DimProducto[Product ID]
* FactPedidos[Order Date] → DimFecha[Date]
* FactPedidos[Shipping Key] → DimEnvio[Shipping Key]

## Design Decisions

* Star schema chosen for performance optimization
* Separate date table to enable time intelligence
* Dimensions normalized for reusability

