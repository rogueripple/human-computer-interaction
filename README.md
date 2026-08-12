# Smart Cafeteria Ordering Mobile App

## Project Description
The **Smart Cafeteria Ordering Mobile App** is a Human-Computer Interaction (HCI) project developed as part of the coursework at Dedan Kimathi University of Technology. The application aims to streamline the meal ordering process for students and staff during busy peak hours. By providing an intuitive mobile interface, users can browse menus, customize meals, place orders, and track preparation status in real time, reducing physical queues and improving the overall dining experience.

---

## University & Course Information
- **University:** Dedan Kimathi University of Technology  
- **School:** School of Computer Science and Information Technology  
- **Department:** Information Technology  
- **Course:** Human-Computer Interaction (HCI)  

---

## Team Members
| **Name**               | **Registration Number**   |
|------------------------|---------------------------|
| Kelvin Makumi          | C025-01-0659/2023         |
| Samuel Wanjau          | C025-01-0606/2023         |
| Preston Njihia         | C025-01-0615/2023         |
| Edwin Weru             | C025-01-2089/2023         |
| Edward Mwangi          | C025-01-0608/2023         |
| Keter Njeri            | C025-01-0622/2023         |

---

## Problem Statement
During lunch and dinner rushes, the campus cafeteria faces significant bottlenecks:
- Long queues lead to wasted time and frustration.
- Students and staff often miss out on popular meals due to lack of real-time availability.
- Order errors are common due to miscommunication at the counter.
- There is no visibility into waiting times or meal preparation status.

These issues lower user satisfaction and reduce the efficiency of cafeteria operations.

---

## Target Users
The mobile app is designed for two main user groups:
1. **Students:** Need a fast and reliable way to order meals between classes.
2. **Staff/Faculty:** Require a convenient option to order meals without long waits during limited break times.

---

## Key Features
| **Feature** | **Description** |
|-------------|-----------------|
| **Browse Menu** | View a categorized list of available meals (e.g., breakfast, mains, snacks, beverages). |
| **View Meal Details & Prices** | Tap on any meal to see a description, ingredients, calorie count, and price. |
| **Select / Customize Order** | Choose meal options, portion sizes, and add special instructions (e.g., extra sauce, dietary preferences). |
| **Confirm Order** | Review the order summary, total cost, and confirm payment (mock checkout). |
| **Track Preparation & Collection** | Receive real-time status updates: *Order Received → Preparing → Ready for Collection*. |

---

## HCI Focus Areas
This project applies core HCI principles to ensure a seamless mobile experience:
- **Mobile Task Flow:** Optimized, step-by-step user journey from browsing to collection.
- **Visual Hierarchy:** Clear, scannable layouts with prominent call-to-action buttons.
- **Feedback:** Instant visual and haptic feedback for every user action (e.g., button taps, order confirmations).
- **Error Prevention:** Input validation, confirmation dialogs, and undo options to prevent mistakes.
- **Touch Interaction:** Designed for natural finger gestures (swipe, tap, pinch) with appropriately sized touch targets.

---

## Prototype
The high-fidelity interactive prototype was built using **Figma**, focusing on a clean, intuitive mobile interface.

### Prototype Links
- **Figma Prototype:** [Insert Figma Link]
- **Video Walkthrough:** [Insert YouTube/Loom Link]

### Key Screens
| Screen | Description |
|--------|-------------|
| **Onboarding / Login** | Simple login with optional guest browsing. |
| **Home / Menu** | Categorized meal cards with images and prices. |
| **Meal Detail** | Full description, customization options, and "Add to Cart" button. |
| **Cart / Order Summary** | List of selected items, modifications, total cost, and "Confirm Order" button. |
| **Order Tracking** | Progress bar showing preparation and collection status with estimated time. |
| **Order History** | Past orders for quick reordering. |

*(Insert screenshots here)*

---

## Testing

### Usability Testing Approach
- **Participants:** 12 volunteers (8 students, 4 staff members).
- **Tasks:** Users completed the following core actions:
  1. Log in to the app.
  2. Browse the menu and find a specific meal.
  3. Customize a meal (e.g., change portion size, add note).
  4. Add items to the cart and confirm the order.
  5. Track the order status until "Ready for Collection."
- **Metrics:** Task success rate, time on task, error count, and post-task satisfaction (System Usability Scale – SUS).
- **Environment:** In-person moderated sessions with a mobile prototype (Figma mirror on Android/iOS devices).

### Testing Results
| **Task** | **Success Rate** | **Avg. Time (sec)** | **Avg. SUS Score** |
|----------|------------------|----------------------|---------------------|
| Login    | 100%             | 8                    | 88                  |
| Browse Menu | 92%           | 12                   | 82                  |
| Customize Meal | 83%       | 25                   | 78                  |
| Confirm Order | 91%       | 18                   | 85                  |
| Track Order | 100%         | 10                   | 90                  |
| **Overall** | **93.2%**  | **14.6** (avg)       | **84.6**            |

---

## Findings

### Key Usability Issues Identified
1. **Customization Clarity:** Some users were confused about how to apply multiple customizations (e.g., selecting both portion size *and* special instructions).
2. **Cart Visibility:** Users occasionally forgot they had items in the cart because the cart icon was not prominent.
3. **Order Confirmation Feedback:** After tapping "Confirm Order," there was a slight delay in visual feedback, causing some users to tap multiple times.
4. **Tracking Status Wording:** The phrase "Preparing" was perceived as vague; users wanted a clearer indication of progress (e.g., "Cooking" vs. "Packing").

### Recommendations
- Redesign customization options using expandable sections with clear labels.
- Add a persistent cart badge (with item count) on the top navigation bar.
- Implement an immediate loading spinner or success animation upon order confirmation, followed by a clear "Order Placed!" screen.
- Replace generic statuses with more descriptive steps: *Order Received → Cooking in Progress → Plating → Ready for Pickup*.

---

## Design Iterations

This folder records how usability findings are converted into prototype improvements.

### Recommended Structure
```text
iterations/
├── README.md
├── iteration-1/
│   └── notes.md
└── iteration-2/
    └── notes.md
