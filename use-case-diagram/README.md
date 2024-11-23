### **Use Case Diagram: Airbnb Clone Backend**

#### **Actors:**

1.  **Guest (User)**
    *   A user who wants to book a property.
2.  **Host (User)**
    *   A user who wants to list and manage their properties.
3.  **Admin**
    *   A user who monitors and manages users, properties, and bookings.
4.  **Payment Gateway**
    *   Handles secure transactions for property bookings.

#### **Key Use Cases:**

1.  **User Registration & Authentication**
    
    *   **Register Account**: Guests and hosts can register for an account.
    *   **Login**: Authenticate users using email/password or OAuth (Google, Facebook).
    *   **Update Profile**: Guests and hosts can update their personal information.
2.  **Property Management (Host)**
    
    *   **Add Property**: Hosts can list their properties by providing property details.
    *   **Update Property**: Hosts can update property details.
    *   **Delete Property**: Hosts can remove a property listing.
3.  **Search Properties (Guest)**
    
    *   **Search & Filter Properties**: Guests can search for available properties based on location, price, number of guests, and amenities.
4.  **Booking Management (Guest & Host)**
    
    *   **Book Property**: Guests can book available properties for specified dates.
    *   **Cancel Booking**: Guests can cancel their bookings.
    *   **Manage Bookings**: Hosts can manage bookings, confirming or canceling reservations.
5.  **Payments (Guest, Host, Payment Gateway)**
    
    *   **Make Payment**: Guests can pay for booked properties via Stripe or PayPal.
    *   **Host Payout**: Hosts receive payouts after bookings are completed.
6.  **Reviews & Ratings (Guest, Host)**
    
    *   **Leave Review**: Guests can leave reviews for properties after their stay.
    *   **Respond to Review**: Hosts can respond to guest reviews.
7.  **Notifications System (Guest, Host, Admin)**
    
    *   **Send Notification**: Booking confirmations, cancellations, and payment updates are notified to guests and hosts via email and in-app notifications.
8.  **Admin Management**
    
    *   **Manage Users**: Admin can view and manage guest and host accounts.
    *   **Monitor Properties**: Admin can manage property listings.
    *   **Oversee Bookings & Payments**: Admin can view and manage booking details and payment transactions.

