# Information Architecture Lead — Role 3

## 1. Task Flow

The task flow describes the steps a user follows to complete the main task in the system: selecting an item and completing an order.

```text
START
  |
  v
Home / Menu
  |
  v
Browse Categories or Search
  |
  v
View Product List
  |
  v
Select Item
  |
  v
View Item Details
  |
  v
Select Quantity / Options
  |
  v
Add to Cart
  |
  v
View Cart
  |
  +----------------------+
  |                      |
  v                      v
Edit Cart           Continue Shopping
  |                      |
  |                      v
  |                Product List
  |                      |
  +----------<-----------+
  |
  v
Checkout
  |
  v
Enter / Confirm Delivery Details
  |
  v
Select Payment Method
  |
  v
Review Order
  |
  v
Confirm Order
  |
  v
Order Confirmation
  |
  v
END
```

### Task Steps

1. User opens the application.
2. User views the Home/Menu screen.
3. User browses categories or searches for an item.
4. User views the available products.
5. User selects an item.
6. User views the item details.
7. User selects the required quantity/options.
8. User adds the item to the cart.
9. User reviews the cart.
10. User edits the cart or continues shopping if necessary.
11. User proceeds to checkout.
12. User enters or confirms delivery details.
13. User selects a payment method.
14. User reviews the order.
15. User confirms the order.
16. System displays the order confirmation.

---

## 2. User Journey

The user journey shows what the user does, what they need, and how the system responds at each stage.

| Stage | User Action | User Need | System Response |
|---|---|---|---|
| 1. Discover | Opens the application | Know what is available | Displays Home/Menu |
| 2. Browse | Selects a category or searches | Find the required item | Displays relevant products |
| 3. Evaluate | Selects a product | Understand the product | Displays item details, price and options |
| 4. Select | Chooses quantity/options | Prepare the purchase | Updates item selection |
| 5. Add | Clicks Add to Cart | Save the selected item | Adds item to cart and updates cart |
| 6. Review | Opens the cart | Check selected items and total | Displays cart contents and total |
| 7. Checkout | Selects Checkout | Complete the purchase | Opens checkout |
| 8. Delivery | Enters/confirms details | Provide delivery information | Validates and saves details |
| 9. Payment | Selects payment method | Pay for the order | Displays payment options |
| 10. Confirm | Reviews and confirms order | Ensure information is correct | Processes order |
| 11. Complete | Views confirmation | Know the order was successful | Displays confirmation and order details |

---

## 3. Interaction Flow

The interaction flow shows how the user moves between screens and how the system responds to user actions.

```text
                 +----------------+
                 |  Home / Menu   |
                 +--------+-------+
                          |
             +------------+------------+
             |                         |
             v                         v
     +---------------+         +---------------+
     |   Categories  |         |    Search     |
     +-------+-------+         +-------+-------+
             |                         |
             +------------+------------+
                          |
                          v
                 +----------------+
                 | Product List   |
                 +--------+-------+
                          |
                     Select Item
                          |
                          v
                 +----------------+
                 |  Item Detail   |
                 +--------+-------+
                          |
                     Add to Cart
                          |
                          v
                 +----------------+
                 |      Cart      |
                 +--------+-------+
                          |
              +-----------+-----------+
              |                       |
              v                       v
        Continue Shopping          Checkout
              |                       |
              |                       v
              |               +---------------+
              |               |   Delivery    |
              |               |    Details    |
              |               +-------+-------+
              |                       |
              |                       v
              |               +---------------+
              |               |    Payment    |
              |               +-------+-------+
              |                       |
              |                       v
              |               +---------------+
              |               | Order Review  |
              |               +-------+-------+
              |                       |
              |                 Confirm Order
              |                       |
              |                       v
              |               +---------------+
              +-------------->| Confirmation  |
                              +---------------+
```

### Main Interactions

- **Home → Categories/Search:** User chooses how to find an item.
- **Product List → Item Detail:** User selects a product.
- **Item Detail → Cart:** User adds the selected item.
- **Cart → Product List:** User can continue shopping.
- **Cart → Checkout:** User starts the purchasing process.
- **Checkout → Delivery:** User provides or confirms delivery information.
- **Delivery → Payment:** User selects a payment method.
- **Payment → Order Review:** User checks the complete order.
- **Order Review → Confirmation:** User confirms the order.
- **Confirmation → Home:** User can return to the main application.

---

## 4. Screen Map

The screen map defines the screens required for the system and how they are connected.

```text
                          +----------------+
                          |  01 Home/Menu  |
                          +-------+--------+
                                  |
                 +----------------+----------------+
                 |                                 |
                 v                                 v
        +------------------+              +------------------+
        | 02 Categories /  |              | 03 Search        |
        |   Product List   |              |     Results      |
        +--------+---------+              +--------+---------+
                 |                                 |
                 +----------------+----------------+
                                  |
                                  v
                         +----------------+
                         | 04 Item Detail|
                         +-------+--------+
                                 |
                                 v
                         +----------------+
                         |    05 Cart     |
                         +-------+--------+
                                 |
                                 v
                         +----------------+
                         |  06 Checkout   |
                         +-------+--------+
                                 |
                                 v
                     +------------------------+
                     | 07 Delivery / Contact  |
                     |        Details         |
                     +-----------+------------+
                                 |
                                 v
                         +----------------+
                         | 08 Payment     |
                         |    Method      |
                         +-------+--------+
                                 |
                                 v
                         +----------------+
                         | 09 Order       |
                         |    Review      |
                         +-------+--------+
                                 |
                                 v
                         +----------------+
                         | 10 Order       |
                         |   Confirmation |
                         +----------------+
```

### Screen Relationships

```text
Home/Menu
   ├── Categories → Product List → Item Detail
   ├── Search → Search Results → Item Detail
   └── Cart

Item Detail → Cart

Cart → Product List (Continue Shopping)
Cart → Checkout

Checkout → Delivery Details
Delivery Details → Payment
Payment → Order Review
Order Review → Order Confirmation
Order Confirmation → Home/Menu
```
