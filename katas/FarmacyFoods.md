# Farmacy Food
### Inputs
Founder: Kwaku Osei
Farmacy Food is a tech-enabled healthy food startup that takes the “Let food be thy medicine” quote literally and creates tasty mund peoples’ dietary needs and active lifestyles to support their overall well-being. Our mission is to meals that are radically affordable and accessible.
Farmacy Food mission: https://www.youtube.com/watch?v=9aSLSVAIkoM
Farmacy Food website: https://www.farmacyfood.com/d: Food as Medicine Actualized - Kwaku Osei - Farms, Food & Health Conference 2019


A “ghost kitchen” needs a system to allow users to have visibility of what items are available, purchase, and pick up items at any one of their points of sale.

Users: dozens of automated fridges and representative run kiosks, thousands of customers.
Requirements:
Must integrate with 3rd party smart fridges to obtain inventory and purchase activity
Smart Fridges accessible through the POS systems API’s.Produce item inventory levels and purchases. The smart fridges have a cloud based management system that handles communication with the Smart Fridge so obtaining this data would be through an API.
Must integrate with point of sale system at kiosks
The Kiosk is a sublet space inside another business where we will sell our product but have an employee to handle the transactions through a point of sale. The same data should be 
Mobile  Web accessible
Support providing feedback on items of verified purchases and in app surveys
Accept coupons and promotional pricing
Send inventory updates to central kitchen


Long term Goals
Long term would like to allow multiple vendors to offer items through points of sale
Wants to harvest data to provide personalized recommendations based on users health goals, purchase history, and item ratings

### Farmacy Food Ghost Kitchen System

**Title**: Efficient Nutrition: Streamlined Food Tech for Healthier Lifestyles

**Introduction**:
Farmacy Food, a health-focused food tech startup, is enhancing their ghost kitchen system to offer users real-time inventory visibility and convenient purchasing options at multiple point-of-sale locations.

**Problem Statement**:
To accommodate increasing demand and improve operational efficiency, Farmacy Food requires a robust system that seamlessly integrates with smart fridges and kiosk POS systems, ensuring accurate inventory tracking and easy customer transactions.

**Users**:
- Automated Fridges and Kiosks: Dozens across various locations
- Customers: Thousands, interfacing primarily through mobile and web applications

**Requirements**:
- **Third-Party Integration**: Must interface with smart fridge APIs for real-time inventory and transaction data.
- **Kiosk Integration**: Ensure synchronization of sales data between kiosks and central systems.
- **User Accessibility**: Mobile and web platforms for user interactions, including purchases and feedback.
- **Feedback System**: Ability to provide feedback and participate in surveys post-purchase.
- **Promotions**: Support for coupon redemption and promotional pricing.
- **Inventory Management**: Real-time inventory updates to the central kitchen and possibly, in future, to multiple vendors.

**Additional Context**:
In the long term, Farmacy Food aims to support multiple vendors through their system and utilize user data to deliver personalized dietary recommendations. The startup environment is fast-paced, with a focus on innovation and user satisfaction, influencing rapid deployment and continuous system updates.

**Budget**:
Approximately $500,000 initially, considering technology integration, development, and scaling needs based on similar startup models.

### Team Name: NutriNet Architects

**A. Logical Component Design**

### Initial Workflow Components

To establish the foundation for our architecture, we begin by mapping out major system workflows. Here's a breakdown of the targeted, workflow-based components:

- **Inventory Tracker**
- **Transaction Handler**
- **Feedback Processor**
- **Promotion Engine**
- **Data Aggregator**

### Refine the component design by analyzing actor actions

**Identify Actors:**
- Customers
- Kiosk Operators
- Central Kitchen Staff

**Map Actions:**
- Customers: Browse products, Make purchases, Provide feedback
- Kiosk Operators: Process transactions, Update inventory
- Central Kitchen Staff: Monitor inventory levels, Update product listings

**Assign Actions:**
- Inventory Tracker: Central Kitchen Staff actions, Kiosk Operator updates
- Transaction Handler: Customer purchases, Kiosk Operator transactions
- Feedback Processor: Customer feedback entries
- Promotion Engine: Apply discounts, Process coupons
- Data Aggregator: Collect data for analytics and reporting

**Align Requirements:**
- Each component aligns with the high-level requirements, ensuring functionalities such as third-party API integrations, user accessibility, and feedback mechanisms are embedded within the system.

**Refine Components:**
- Ensure components are well-defined and specific to their functions without overlapping responsibilities.

### Output Table 1 - Roles, Actions

| **Actor**             | **Role**              | **Actions**                             |
|-----------------------|-----------------------|-----------------------------------------|
| Customers             | End Users             | Browse products, Make purchases, Provide feedback |
| Kiosk Operators       | POS Interface         | Process transactions, Update inventory  |
| Central Kitchen Staff | Inventory Management  | Monitor inventory levels, Update product listings |

### Output Table 2 - Components, Behaviors/actions (responsibilities), and aligned requirements

| **Component**         | **Responsibilities**                          | **Aligned Requirements**                             |
|-----------------------|-----------------------------------------------|------------------------------------------------------|
| Inventory Tracker     | Track and update inventory in real-time       | Integration with smart fridge APIs, Real-time updates |
| Transaction Handler   | Handle purchasing transactions                | Seamless POS integration, Mobile/Web accessibility   |
| Feedback Processor    | Process user feedback and survey responses    | User feedback system, Enhance user satisfaction      |
| Promotion Engine      | Manage and apply promotions and coupons       | Support promotional pricing, Coupon redemption       |
| Data Aggregator       | Aggregate data for analytics and reporting    | Long-term user data utilization, Vendor support      |

### Requirements Not Satisfied:
- All listed requirements are currently aligned with the proposed components.



