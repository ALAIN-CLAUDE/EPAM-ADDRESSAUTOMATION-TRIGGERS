# EPAM-ADDRESSAUTOMATION-TRIGGERS


Addresses

As part of our system we want to support multiple addresses for customer as separate object. In the same
time, we want to keep the standard SF address fields on the Account page layout
1. Create custom object to store addresses as separate entity for account. Address can be or Billing, or
Shipping. Address can be marked as main.
2. Create Apex logic to support following behavior:
a. If user creates a new account and at least one field for Billing address isn’t empty system
must automatically create a new Main Billing Address. The same logic should be applied for
Shipping Address
b. One account can have only one main billing address and only one main shipping address
c. If user updates Account Billing Address field changes should be automatically applied to
Main Billing Address. Same logic for Shipping Address
d. If user updates Main Billing Address changes should be automatically applied to Account
Billing Address. The same logic should be applied for Main Shipping Address
e. User should be able to create new address billing/shipping address and mark it as main.
3. Create set of LWC components to display list of account addresses on the Account Lightning Page.
a. Component should show following fields: address name, main flag, address type
b. Component should provide an ability to open specific address for view(standard SF page)
c. Component should provide an ability to create a new address
d. Component should provide an ability to delete existing address
e. Component should provide an ability to modify existing address
f. Component should provide an ability to filter addresses by type and by flag ‘main’
