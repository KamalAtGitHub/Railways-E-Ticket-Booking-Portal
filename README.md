### **Railway E-Ticket Booking Portal**

This is a **Railway E-Ticket Booking Portal** that allows users to create accounts, log in, book train tickets, check ticket status, cancel tickets, and manage their accounts. It uses **MySQL** as the database for storing user accounts and ticket details.

---

## **Key Features**

## **User Authentication & Account Management**
### **Login Menu (`login_menu`)**
- Displays three options:
  1. Create a new account
  2. Log in
  3. Exit the portal

### **Account Creation (`create_acc`)**
- Generates a random **user ID**.
- Takes user input for **password, name, gender, age, DOB, and phone number**.
- Inserts the new account details into the **`accounts`** table.

### **Login (`login`)**
- Asks for **User ID** and **password**.
- Checks if credentials exist in the **`accounts`** table.
- If found, welcomes the user and redirects to the **main menu**.
- If not found, allows the user to retry or create a new account.

---

## **Main Functionalities**
### **Main Menu (`main_menu`)**
- Once logged in, users can:
  1. Purchase a Ticket
  2. Check Ticket Status
  3. Cancel Ticket
  4. Manage Account
  5. Logout
  6. Exit

### **Booking a Ticket (`buy_ticket`)**
- Asks the user for **train name, date of journey, departing station, and destination**.
- Generates a random **PNR number**.
- Stores ticket details in the **`tickets`** table.

### **Checking Ticket Status (`show_ticket`)**
- Takes **PNR number** as input.
- Fetches ticket details from the **`tickets`** table.
- Checks if the ticket belongs to the logged-in user.

### **Cancel Ticket (`cancel_ticket`)**
- Asks for **PNR number**.
- Validates if the ticket belongs to the logged-in user.
- Deletes the ticket from the **`tickets`** table upon confirmation.

---

## **5. Additional Features**
### **Account Management (`account`)**
- Users can **view their account details**.
- Users can **delete their account**, with an option to **refund any booked tickets**.

### **Exit Handling (`exit_prompt`)**
- Asks the user for confirmation before exiting.
- Redirects back to the main menu if the user chooses **not to exit**.

