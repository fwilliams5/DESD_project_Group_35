# Project Overview – Use Case 1

We've been tasked to design a system that allows a producer to submit product information to create a listing, this information should be validated before being published. The system should also include inventory management to show stock levels and availability of products.

# Full scope

| Sectors | What we should include |
|---|---|
| Purpose | Create a digital marketplace that will connect local producers to customers in the Bristol Regional Food Network. |
| Management (products) | Inventory updates / Prices / Listing notifications / Availability or 'in stock'. Can create listings with image uploads. Search box for specific foods. |
| Functions ( Orders) | Collection and delivery arrangements, searching and ordering, ability to search categories, can order from different producers. (Multi producer order) |
| Functions ( transactions) | Implementing sandbox payments, (Paypal or stripe for sandbox). Records of payments created for manager and 5% commission implemented. |
| Community and multi orders | Food information and traceability for big orders. Discounts on larger orders to keep communities engaged. Should be relevant educational information included. |
| Out of scope, but could include | For communities, bigger orders could be exempt from a 48 hour prep time on cancelling orders or refunds. |
| Out of scope, won't include | Delivery responsibilities. Real financial data stored and real payment system included. Call option for deliveries. |

# Major business process analysis

| Major Business process | Actors | Action / Purpose | Input | Expected output |
|---|---|---|---|---|
| Customer ordering | Customers | Combine purchases from different producers. One or multiple. | Basket page, customer details and fulfilment. | Validate order. Allocate producers to products bought. |
| Payment process | Payment sandbox , marketplace (commission calculator) | Calculate 5% commission on network and simulate payment process. | Total cost of order and payment details | Payment outcome. Transaction record to database |
| Product management | Local producers | Maintain accuracy with seasonal availibility, listings and stock available. | Product info, price, stock quantity available. | Catalogue updated |
| Producer settlements | Network operator, local producers | Maintain financial records | Records of commission and transactions | Simulate settlements |
| Community and sustainability | Local communities, local producers | Update info on food mile calculation, surplus discounts and educational content posted on foods | Postcode calculation, surplus stock, separate channel, recipes, allergen info, educational info. | Reports, food mile calculation, published discounts for surplus stock. |
| Food quality | Local producers, network operator | Traceability for affected products if food quality is safety concern | Traceability, purchase records | Customer unique code link to products and local producers on order. Nofication issue. |
| Order fulfilment | Local producers | 48 hr lead time | Confirm items that are ordered, payment fulfilled | Fulfilment confirmed and order created |

# Identification and scope of major functionalities - USE CASE 1

## Candidate 1 – Product listing.

**Purpose** – To allow producers to publish valid product listings that customers can view and search for easily.

**Origin of process** – Producer attempts to submit a listing to marketplace

**What do we need to include?** - Product details confirmed and validated. Publish valid listing to marketplace.

**Logic** – Details accurate and valid for system upload? Producer organic certification claimed?

**Ending of process** – Listing validated and published.

**Potential logic break** – External certification verification invalid, incorrect details (resubmit)

**Actors involved** – Local producer, marketplace and verification service ( could be external).

**Requirements that link** – FR-1, FR-5, FR-18.

**Backlog** – PB-1 and PB-4

## Candidate 2 – Inventory management, seasonal availability and stock change.

**Purpose** – Maintain marketplace stock accuracy and local producer's product quantities available for in time seasonal purchases. Helps to aid customers and local producers simultaneously with correct product quantities.

**Origin of process** – Local producer updates their stock or seasonal availability changes on their stock from records.

**What do we need to include?** - Quantity updates and periods of availibility for seasonal stock which can be uploaded to the marketplace. Use logic to validate whether products are actually valid to pruchase and keep a status of availability on products across the marketplace uploaded by producers. Keep warnings of best before and regulate these products.

**Logic** – Is product within the window of availibility of the season? Is the product within best before? Is the stock level above zero?

**Ending of process** – Any local producer change is validated against tests in the code and the status is updated to the marketplace ready to be bought.

**Potential logic break** – Invalid quantities of stock, incorrect dates uploaded or wrong info uploaded for seasonal information.

**Actors** – Local producers and marketplace

**Linked requirements** – FR-3, FR-4

**Backlog link** – PB-3