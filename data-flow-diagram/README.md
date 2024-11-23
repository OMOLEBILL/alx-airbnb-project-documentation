### Diagram Overview

#### Entities
- **Guest**, **Host**, and **Admin** represent the users interacting with the system.

#### Backend Services
- **Auth Service**: Handles user authentication.
- **User Management Service**: Manages user profiles.
- **Property Management Service**: Manages property listings.
- **Booking Service**: Manages bookings.
- **Payment Service**: Manages payments through Stripe or PayPal.
- **Review Service**: Manages property reviews.
- **Notification Service**: Sends booking notifications.
- **Admin Dashboard Service**: Admin tasks to manage users, properties, and bookings.

#### Database Layer
- **Users DB**, **Properties DB**, **Bookings DB**, **Payments DB**, and **Reviews DB** store relevant data.

#### File Storage
- **AWS S3** is used to store images.

#### Third-Party Integrations
- **OAuth Providers** for login, **Stripe** and **PayPal** for payments, **SendGrid/Mailgun** for email notifications.

#### Security
- **Firewall & Rate Limiting** is used to secure all backend services.

