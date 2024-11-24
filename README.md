# PayManager

PayManager is a system designed to handled the creation, subscription and
charge of plans. Plans could be services, products or any other type of
subscription. The system is designed to allows administrators to directly
supervise and manage billing and collection processes, providing greater
control over operations, admins will also be able of creating catalogs and
adding plans and subscription to them. User will be able to subscribe to plans;
in order to be able of adding subscriptions a user should have credit card
information added to their account. Credit cards information will be stored in
a gateway specify by the admin, the admin should add the keys
(Public and Private) provided by the payment gateway in the system so the system
will be able of communicate with the gateway, currently we support the following
gateways: Stripe, Paypal, MercadoPago, ePayco, Wompy, PayU and E-collect.
Gateways will also be used to process the transaction of charges to the user
according to the plan subscribed.

## Technical Details

- [Repository](https://www.youtube.com/watch?v=Wiy54682d1w) as pattern
to access and save data.

- We will use ids to identify users, plans, subscriptions, catalogs and
charges. The system will be able to handle multiple catalogs, plans and
subscriptions. The system will also save information of the transactions.

- We will use payments gateways to store credit card information and process
the charges to the users.

Note: Since this is a academic project wi will simulate all external iterations
with the payment gateways.

- As alternative to directory and file based storage we should use SQLite
(missing validation of requirements).

### Useful Links

- [Design Patterns](https://www.youtube.com/watch?v=JI_THVXPToQ)
