## Requirements register - open to changes based on initial draft

## Use case 1 

## Functional requirements 


## Functional requirements

| Req ID | Functional requirement | MoSCoW rating | Dependencies |
|---|---|---|---|
| FR-1 | The system must allow producers to create and update product listings. | Must | NFR-1 |
| FR-2 | The system must allow users to browse products by categories and search product name. | Must | FR-1 |
| FR-3 | The system must update seasonal availability for products. | Must | FR-1 |
| FR-4 | The system must maintain inventory quantities to be updated freely. | Must | FR-1 |
| FR-5 | The system must display product information including harvest dates, farm origin and seasonality. | Must | FR-1 |
| FR-6 | The system must support orders containing products from one or multiple producers. | Must | FR-1,FR-3,FR-4,FR-7 |
| FR-7 | The system must identify the producer responsible for each product. | Must | FR-1 |
| FR-8 | The system must display delivery and collection arrangements. | Must | FR-6,FR-7 |
| FR-9 | The system must allow producers to access their incoming orders. | Must | FR-6,FR-7,NFR-1 |
| FR-10 | The system must support a minimum 48-hour preparation time for producers. | Must | FR-7,FR-8 |
| FR-11 | The system must have a secure payment system that complies with current data protection and financial services regulations. | Must | FR-6, NFR-1 |
| FR-12 | The system must calculate 5% commission on orders. | Must | FR-6, FR-7, FR-11 |
| FR-13 | The system must simulate settlements that follow a weekly schedule. | Must | FR-7, FR-11, FR-12, FR-14 |
| FR-14 | The system must implement financial audit trails. | Must | FR-11, FR-12, NFR-4 |
| FR-15 | The system must notify users of surplus produce offers and allow surplus discounts to be applied. | Must | FR-1, FR-3, FR-4 |
| FR-16 | The system must publish recipes, guidance and farm stories for educational purposes. | Must | FR-7 |
| FR-17 | The system must link customers to the relevant products and producers. | Must | FR-1, FR-6 |
| FR-18 | The system must display food information, including certifications, postcode-based food miles, allergens and best-before information. | Must | FR-1 |

## Non functional requirements

| Req ID | Non functional requirement | MoSCoW rating | Dependencies |
|---|---|---|---|
| NFR-1 | The system must protect customer orders and producer listings. | Must | FR-1,FR-6 |
| NFR-2 | The system should aim for a min three response time once loaded (testable). | Should | FR-2 |
| NFR-3 | The system should be appealable, with a min three second response time. | Should | FR-1,FR-2 |
| NFR-4 | The system must retain records (financial) | Must | FR-6,FR-14 |
| NFR-5 | The system must prevent concurrent overselling and maintain accurate inventory stock. | Must | FR-4,FR-6 |
| NFR-6 | The system must handle unsuccessful payments in the payment sandbox. | Must | FR-11 |
| NFR-7 | The system could provide background information on local producers for more info. | Could | FR-16 |
| NFR-8 | The system must prevent duplicate payments and orders on same checkout. | Must | FR-6,FR-11 |
| NFR-9 | The system could allow users to browse using only a keyboard. | Could | FR-2 |
| NFR-10 | The system could allow customers to reorder products from a previous order. | Could | FR-1,FR-3,FR-6,FR-4 |
| NFR-11 | The system could offer a loyalty system that gives repeat customers discounts. | Could | FR-6,NFR-4 |
| NFR-12 | The system could allow users to schedule collection instead of delivery. | Could | FR-8 |
