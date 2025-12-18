This is a full-stack e-commerce web application developed using Spring Boot and thymeleaf. The project demonstrates real-world features such as authentication, role-based access, online payments, order management, and admin controls.

Tech Stack -
Backend: Spring Boot, Spring MVC, Spring Security, Dependency Injection
Frontend: Thymeleaf, HTML, CSS, JavaScript
Authentication: JWT (JSON Web Token)
Database: MySQL
Payment Gateway: Razorpay
Mail Service: JavaMailSender

Key Features

User Features
User registration and login with JWT-based authentication
Browse products by categories
Add products to cart

Place orders using:
Cash on Delivery (COD)
Online Payment (Razorpay Integration)

For COD orders, an order confirmation email is sent
For online payments, users are redirected to the Razorpay checkout page and order is confirmed only after successful payment

View order history
Cancel orders if not required

Admin Features -
Admin authentication and role-based access
Add, update, and delete products
Manage categories
View and control all user orders
Update order status (placed, shipped, delivered, canceled)

Razorpay Payment Flow

User selects Pay Online during checkout
Razorpay order is created from the backend
User is redirected to the Razorpay payment page
On successful payment:
Payment is verified
Order is saved
User is redirected to the success page
Failed or canceled payments do not create an order

Email Notifications
Order confirmation email is sent automatically for Cash on Delivery orders
Ensures better user communication and order tracking

Security
JWT-based authentication for users and admins
Role-based authorization
Secure payment verification using Razorpay signature validation
