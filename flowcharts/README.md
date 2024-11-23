### Flowchart: Property Booking Process

#### Key Steps and Data Flow

1. **Guest Login/Registration**
   - The **Guest** logs in using **Auth Service**. If not registered, they complete the **registration** process.
   - **Auth Service** verifies credentials and generates a session token.

2. **Search Properties**
   - The **Guest** uses **Property Management Service** to search and filter available properties.
   - **Properties DB** is queried for availability and relevant filters (e.g., location, price, amenities).

3. **Select Property**
   - The **Guest** selects a property for booking.
   - Property details, including **availability**, are fetched from **Properties DB**.

4. **Booking Request**
   - The **Guest** initiates a booking request through the **Booking Service**.
   - **Booking Service** checks the **availability** in **Properties DB** and **Booking DB** to prevent double booking.

5. **Make Payment**
   - Once the booking is confirmed, the **Guest** makes a payment using the **Payment Service**.
   - **Payment Service** interacts with **Stripe** or **PayPal** for secure payment processing.
   - Upon successful payment, booking details are saved in **Booking DB** and **Payments DB**.

6. **Booking Confirmation**
   - **Notification Service** sends a confirmation email to the **Guest** and **Host** using **SendGrid/Mailgun**.
   - Booking status is updated to **confirmed** in **Booking DB**.

#### Summary of Services and Data Flow
- **Auth Service**: Handles guest authentication.
- **Property Management Service**: Facilitates searching for available properties.
- **Booking Service**: Handles booking requests and availability checks.
- **Payment Service**: Processes payments securely.
- **Notification Service**: Sends booking confirmations to guests and hosts.

#### Data Storage
- **Users DB**: Stores guest and host information.
- **Properties DB**: Stores property details and availability.
- **Booking DB**: Records all booking details, including status.
- **Payments DB**: Logs payment transactions.

