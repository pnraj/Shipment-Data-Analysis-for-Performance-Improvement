### Data Model for Shipment Data Analysis

#### Table: `Shipments`

| Column Name       | Data Type    | Description                            |
| ----------------- | ------------ | -------------------------------------- |
| `shipment_id`     | INT          | Unique identifier for each shipment.   |
| `order_id`        | INT          | Identifier linking to the order.       |
| `shipment_date`   | DATETIME     | Date and time when the shipment occurred. |
| `delivery_time`   | INT          | Time taken for delivery in minutes.    |
| `status`          | VARCHAR(50)  | Shipment status (e.g., delivered, in transit). |
| `shipment_mode`   | VARCHAR(50)  | Mode of shipment (e.g., sea, air, road, rail). |


#### Table: `Orders`

| Column Name       | Data Type    | Description                            |
| ----------------- | ------------ | -------------------------------------- |
| `order_id`        | INT          | Unique identifier for each order.      |
| `customer_id`     | INT          | Identifier linking to the customer.    |
| `order_date`      | DATETIME     | Date and time when the order was placed. |
| `product_id`      | INT          | Identifier linking to the product.    |
| `quantity`        | INT          | Quantity of the product in the order.  |


#### Table: `Customers`

| Column Name       | Data Type    | Description                            |
| ----------------- | ------------ | -------------------------------------- |
| `customer_id`     | INT          | Unique identifier for each customer.  |
| `customer_name`   | VARCHAR(100) | Name of the customer.                  |
| `email`           | VARCHAR(255) | Email address of the customer.         |
| `Gender`          | VARCHAR(10) | Male or Female or Transgender      |
