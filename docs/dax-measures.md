# DAX Measures

## Sales Metrics

### Total Sales

SUM(FactPedidos[Sales])

### Total Profit

SUM(FactPedidos[Profit])

### Profit Margin %

DIVIDE([Total Profit], [Total Sales])

---

## Customer Metrics

### Total Customers

DISTINCTCOUNT(FactPedidos[Customer ID])

---

## Logistics Metrics

### Avg Ship Days

AVERAGE(FactPedidos[Ship Days])

### On-Time %

DIVIDE(
CALCULATE(COUNTROWS(FactPedidos), FactPedidos[Ship Days] <= 4),
COUNTROWS(FactPedidos)
)

### Shipping Cost per Order

DIVIDE(
SUM(FactPedidos[Shipping Cost]),
COUNT(FactPedidos[Order ID])
)

