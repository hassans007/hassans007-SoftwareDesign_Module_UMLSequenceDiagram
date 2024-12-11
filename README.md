![Logbook 3 (UML Sequence Diagram)-images-0](https://github.com/user-attachments/assets/398fac4d-2ea2-44e5-8a62-51a467a129d0)

# Hotel Management System (HMS) UML Sequence Diagram

This document provides an overview of the UML Sequence Diagram representing the functionality of a **Hotel Management System (HMS)**. The sequence diagram captures the interaction flow for tasks such as user login, making reservations, processing payments, updating reservation statuses, and user logout.

## Functionalities Represented in the Sequence Diagram

### 1. **User Login**
   - **Description**: The user initiates the login process by providing their credentials.
   - **Process**:
     - The HMS verifies the user's credentials by checking them against the Server.
     - The login functionality is separated into a distinct step to ensure proper authentication before granting access to system features.
   - **Security**: The login process enhances security by confirming user identity before allowing access to the system.

### 2. **Making a Reservation**
   - **Description**: After logging in successfully, the user proceeds to make a reservation.
   - **Process**:
     - The HMS requests reservation details from the user and checks room availability in the Server.
     - If a room is available, the HMS displays room options to the user, allowing them to choose a specific room.
     - The HMS reserves the selected room by updating the Server accordingly.
   - **User Experience**: Real-time room availability checks ensure accurate booking information, allowing for a smooth reservation process.

### 3. **Processing Payments**
   - **Description**: Once the reservation is confirmed, the user proceeds to select a payment method.
   - **Process**:
     - The HMS requests payment details and communicates with the **Payment Gateway (PG)** to process the payment.
     - Before processing the payment, the HMS checks the user's account balance to ensure sufficient funds.
   - **Security**: The additional step of checking the user's balance helps avoid payment failures, ensuring a seamless transaction experience.

### 4. **Updating Reservation Status and Confirmation**
   - **Description**: After a successful payment, the HMS updates the reservation status in the Server to reflect the payment completion.
   - **Process**:
     - The system then provides the user with a reservation confirmation displaying relevant details.
   - **User and Staff Coordination**: This functionality ensures that both users and hotel staff have up-to-date information on reservations, helping maintain accurate reservation tracking.

### 5. **User Logout**
   - **Description**: When the user decides to logout, the HMS invalidates the user's session by communicating with the Server.
   - **Process**:
     - The system ensures proper session termination to maintain security and prevent unauthorized access.
   - **Security**: Logging out prevents any unauthorized access to the system after the user has finished their session.

## Conclusion
The design of the **Hotel Management System (HMS)** UML Sequence Diagram focuses on key functionalities necessary for the hotel management process. These include secure login, efficient reservation management, seamless payment processing, and secure session handling. The system is designed to provide a user-friendly experience, accurate reservation tracking, and data integrity, ensuring both users and hotel staff can effectively manage hotel operations.
