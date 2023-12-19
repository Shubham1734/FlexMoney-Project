# Yoga Classes Admission Form
## Overview
This project is a web application for managing admission to Yoga Classes on a monthly basis. Users can enroll in classes and make monthly payments.

## Technologies Used
- React for the frontend
- Node.JS for the backend
- MongoDB for the database

## Setup Instructions
1. Clone the repository: `git clone <repository-url>`
2. Set up Frontend and Backend
3. Install dependencies
4. Set up the MongoDB database and configure the connection in `.env`.
5. Run the application: `npm start`


# Frontend
- User form
    - name
    - age
    - selectBatch

- Generate Receipt
    - Date
    - invoice number
    - Customer Name
    - Age
    - Batch 
    - Amount Paid
    - Total Paid

# Backend
## schema
```typescript
type User = {
    name : string,
    age : number
    selectBatch:string
}
```

# ER Diagram
![image (4)](https://github.com/Shubham1734/project3/assets/93915712/d7c48b11-efe5-4ecb-a85e-dfd92ac917c9)\
We assume additional entities, such as payment and batch, as per the question. However, we don't need to implement payment, so we will ignore it.

# Demo
https://front-lr57.onrender.com
## Screenshots
![Screenshot (1066)](https://github.com/Shubham1734/project3/assets/93915712/bef30415-fcfa-46f8-af2d-fa26d5014949)
![Screenshot (1067)](https://github.com/Shubham1734/project3/assets/93915712/7a046ccb-099c-4720-8af8-911ac7f03bb0)


# Approach 
1. Design a user-friendly form to gather information such as name, age, and preferred batch.
2. After filling out the form, users click the submit button.
3. Upon submission, the entered data is securely stored in the MongoDB Atlas database.
4. The database schema is set up to match the structure of the form, ensuring seamless data storage.
5. The project is deployed on a free cloud service, making use of MongoDB Atlas as the cloud database.
6. This choice ensures scalability, reliability, and accessibility of the application.
7. The form includes a payment link, enabling users to make payments for the Yoga Classes.
8. Clicking on the payment link initiates the payment process.
9. After successful payment, users are redirected to a dedicated page where they can view their payment receipt.

# Assumptions
- A fixed monthly fee of 500 Rs INR for Yoga Classes.

# Future improvements
- Explore additional payment gateways for user convenience.
- Enhance form validation and error handling.
- Implement user authentication for a more personalized user experience.
- Introduce a notification system to send confirmation emails or SMS to users upon successful enrollment and payment.
- Create an admin dashboard to manage user enrollments, view payment statuses, and generate reports. 
