Database
The USSD gateway relies on a MySQL database named register containing three tables: admin, creatte, and pay.

Table Structure
1. admin
This table stores information about registered users who have paid their school fees.

Columns:
id: Unique identifier for each user.
Names: Name of the user.
Regnumber: Registration number of the user.
Department: Department of the user.
Campus: Campus where the user is registered.
amount_in_franc: Amount paid by the user (in francs).
Phonenumber: Phone number of the user.
2. creatte
This table stores information about registered users who have not paid their school fees yet.

Columns:
email: Email address of the user (if available).
phonenumber: Phone number of the user.
password: Password set by the user during registration.
cpassword: Confirmation of the password.
pay_status: Payment status of the user (not_pay or payed).
3. pay
This table records the payment transactions made by users.

Columns:
pay: Amount paid by the user.
number: Phone number of the user making the payment.
Sample Data
The tables contain sample data to demonstrate the functionality of the USSD gateway:

admin: Contains information about registered users who have paid fees.
creatte: Contains information about registered users who have not paid fees yet.
pay: Records payment transactions made by users.
