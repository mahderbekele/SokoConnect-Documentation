__Technical Overview__

**1. Architecture Flow Description**


Registration & Login


Both customers and Mama Mboga vendors access the platform via web/mobile.
Registration/Login requests are sent to the API, which interacts with the database to authenticate or register users.
Upon successful login, users are directed to their respective dashboards.


Order


Customers browse available products and place orders.
Order details are sent to the API, which writes order data to the database.
Mama Mboga vendors receive order notifications via their dashboard.
Order status updates (e.g., confirmed, ready for pickup) are handled via the API and reflected in the database.


Stock


Mama Mboga vendors update stock information through their interface.
Stock updates are sent to the API, which modifies the product inventory in the database.
Customers see real-time stock availability when browsing.


Payment


Customers initiate payment during checkout.
Payment details are processed via the API, which updates payment status in the database.
Both customers and vendors can view payment confirmation and history.


**2. Integrations / APIs**


 M-Pesa API: Handles all customer-to-vendor payments and confirms payment status.

 Core API: Manages data flow between modules and external APIs.

 Geolocation API: Determines proximity for order broadcasting, ensuring orders go only to vendors within 500 meters.

   Out-of-Scope Features

 No real-time communication (chat/messaging) between customers and vendors

 No delivery service (pickup only)

There is no support for payment methods other than M-Pesa

No vendor-to-vendor trading or marketplace features

No multi-language support at launch

**3. Security and Data Handling**

 In building SokoConnect, a platform connecting informal vendors with young consumers, processing personal data, handling M-Pesa mobile payments, and leveraging AI for guiding daily business decisions, compliance with regulatory and legal requirements is not just a formality; it’s a basis of product development. Getting compliance right protects users, ensures ethical operations, mitigates legal risks, and secures market access, fostering trust and enabling sustainable growth.
  Here is our [regulatory and compliance data attached] (https://docs.google.com/document/d/16JZ6EFk8k9zWEoiPtGb1qfq9QtfRm0kFLaf7Z58OZNE/edit?usp=sharing)


