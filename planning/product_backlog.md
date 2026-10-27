# Product backlog – Rank smaller, more powerful -> vaguer and larger requirements to be produced first

| PB ID | Backlog item | Criteria | Requirement link |
|---|---|---|---|
| PB-1 | Create and edit product listings. | Producers can edit and list products with correct details, if incorrect – reject. Cannot change another producers listings. | FR-1 , NFR-1 |
| PB-2 | Browse products by category and search for products. | Category list with ticked box to search for specific category. Searchbox comes up with clear message if none available. | FR-2 |
| PB-3 | Stock management and seasonal availability. | Producers can update and manage there inventory availiability. Out of stock products willbe marked as unavailiable. | FR-3, FR-4 |
| PB-4 | Product origin and food info displayed on products. | Details to be shown on food products. Farm origin, harvest dates and availibility with seasons, allergens and best before date. | FR-5,FR-18 |
| PB-5 | Multi producer basket. | Customers will be able to add, remove and update the quantities of products they desire from different producers. | FR-6, FR-7 |
| PB-6 | Sandbox payments. | Successful test payments. Failed or cancelled payments will mark order as not paid. | FR-11, NFR-6 |
| PB-7 | Validate stock when checking out. | Cannot sell more stock than there is currently available and rejected with reason notification. | FR-4, NFR-5 |
| PB-8 | Display arrangements and validate prep time. | 48 hr prep time for orders and customers can see arrangements for different producer items ordered. | FR-8,FR-10 |
| PB-9 | Prevent duplicate checkouts within the same checkout request. | Cannot order simultaneously twice and second order will be rendered not available. | NFR-8 |
| PB-10 | Create customer order uniqueness. | Checkouts that are successful will be given a unique order reference code. The code links the customer to the producer. Records can be found easily by the network operator. | FR-6,FR-7,FR-17,NFR-1,NFR-4 |
| PB-11 | Calculate the network commission. | 5% commission on all orders placed. | FR-12 |
| PB-12 | Record weekly settlements and provide financial records. | Network operators can review payments, commision and settlements in a portfolio style board. Records shall be kept and settlements recorded weekly. | FR-13, FR-14, NFR-4 |
| PB-13 | Give notice for surplus offers and discounts available. | Producers can publish surplus quantities if desired with discounts shown available. Separate channel for discounts and surplus. | FR-15 |
| PB-14 | Display food miles and publish educational info alongside. | Postcode to postcode calculation for food miles info. Producers can be able to publish their own educational info too. | FR-16 |

# Refinement (INVEST)

| Letter | Applied to our project | Explanation |
|---|---|---|
| I | Independent – Product listing can be developed separately from checkout and payment processes. However, products cannot be ordered until listing exists. | Allows group members to work on different features at the same time, reducing waiting delays for other tasks to finish. |
| N | Negotiable – Requirements establish what each stakeholder must be able to do. The team can decide how it will be displayed. | Gives the team flexibility to make design choices without changing the functionality required for stakeholders. |
| V | Valuable – Accurate inventory management will benefit producers with up to date listings and benefit customers by reducing the risk of ordering unavailable products. | Helps us prioritise features that wil be useful, especially during a sprint. |
| E | Estimable – Product listing and stock management tasks have defined requirements, inputs and expected outcomes. | Allows the team to estimate the time and effort required for each task and allocate work accordingly. |
| S | Small – Product listing can be broken down and split up into smaller tasks such as entering product details, validating information and publishing the product to the marketplace. | Smaller sized tasks will be much easier to manage and assign to team members and complete within the relveant sprint |
| T | Testable – Product listings can be tested by submitting valid and invalid details and using test cases automated or manual. | Gives us clear acceptance criteria so we can verify functionality is working as should be|