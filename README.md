# FoodSave

## SE3090 - Software Engineering Frameworks

### Assignment 2 - Mini Hackathon

FoodSave is a web-based surplus food redistribution platform developed
to help reduce food waste in Sri Lanka by connecting food businesses
with people and organizations that can make use of surplus food.

**Group Number:** 2026-AI-41\
**Institution:** Sri Lanka Institute of Information Technology (SLIIT)\
**Specialization:** Artificial Intelligence\
**Batch:** Y3.S1.WE.AI.01.02\
**Campus:** Malabe

------------------------------------------------------------------------

## 1. Selected Problem

Food waste is a growing environmental and social problem in Sri Lanka.

Restaurants, bakeries, supermarkets, food businesses, and households
often have surplus food that is still safe for consumption but may be
discarded because it is close to its expiry time or cannot be sold. At
the same time, individuals and community organizations may need
affordable or available food but have limited ways to discover nearby
surplus food.

The lack of a simple platform connecting food providers with potential
recipients can therefore result in unnecessary food waste and missed
opportunities to redistribute usable food.

------------------------------------------------------------------------

## 2. Proposed Solution

FoodSave is a web-based digital solution developed using the MERN stack
to help reduce food waste by making surplus food easier to discover and
redistribute.

Businesses can list available surplus food by providing information such
as food name, category, description, quantity, location, business name,
and expiry date. Recipients can browse available food, search and filter
listings, view food details, and submit requests for suitable food
items.

The system also supports a request management process. Businesses can
review incoming food requests and accept or reject them, while
recipients can track the status of their requests. Food listings can
become unavailable when their available quantity is exhausted or when
their expiry time has passed.

Through these features, FoodSave aims to make surplus food
redistribution easier, reduce unnecessary food waste, and create a
practical digital connection between food businesses and people who can
make use of surplus food.

------------------------------------------------------------------------

## 3. Main Features

### 3.1 User Login

Users can log in to the FoodSave system and access the functions
available to their role.

### 3.2 Food Listing

Business users can add surplus food to the platform.

A food listing includes:

-   Business name
-   Food name
-   Category
-   Description
-   Quantity
-   Unit
-   Location
-   Expiry date

### 3.3 Browse Food

Recipients can browse available surplus food listings and view important
information about each food item.

### 3.4 Search and Filter

Recipients can search and filter food listings to find suitable surplus
food based on available listing information such as food name, category,
and location.

### 3.5 Food Request

Recipients can submit a request for an available food listing by
providing their name and requested quantity.

The system checks that the selected food exists, is available, and has
sufficient quantity.

### 3.6 Business Request Management

Business users can view incoming food requests and manage them by:

-   Accepting requests
-   Rejecting requests
-   Reviewing request details
-   Checking requested quantities
-   Tracking request status

### 3.7 Request Status Tracking

Food requests are managed using the following statuses:

-   Pending
-   Accepted
-   Rejected
-   Collected

Recipients can view their requests and track their current status.

### 3.8 Food Quantity and Availability Management

When a request is accepted, the available quantity of the food listing
is reduced.

When the available quantity reaches zero, the food listing becomes
unavailable.

Food listings can also become unavailable after their expiry time.

### 3.9 Input Validation

The application validates user input and displays meaningful error
messages when information is missing or invalid.

Examples include:

-   Required fields cannot be empty.
-   Food quantity must be valid.
-   Requested quantity cannot exceed available quantity.
-   Expired or unavailable food cannot be requested.
-   Invalid request statuses are rejected.

### 3.10 Responsive User Interface

The FoodSave interface is designed to work on both desktop and mobile
screen sizes.

------------------------------------------------------------------------

## 4. Target Users

### Food Businesses

Restaurants, bakeries, supermarkets, and other food businesses can use
FoodSave to list surplus food and manage requests from recipients.

### Recipients

People and community organizations can use FoodSave to discover
available surplus food, submit requests, and track their requests.

### Community Organizations

Community organizations can use the platform to discover surplus food
that can be redistributed to people who can make use of it.

------------------------------------------------------------------------

## 5. System Workflow

The main FoodSave workflow is:

``` text
Business
   |
   v
Add Surplus Food
   |
   v
Food Listing Available
   |
   v
Recipient Browses / Searches / Filters
   |
   v
Recipient Requests Food
   |
   v
Business Reviews Request
   |
   +------------------+
   |                  |
   v                  v
 Accept             Reject
   |                  |
   v                  v
Accepted            Rejected
   |
   v
Recipient Collects Food
   |
   v
Collected
```

------------------------------------------------------------------------

## 6. Technologies Used

  Technology     Purpose
  -------------- -------------------------------------------------
  React.js       Frontend user interface
  Vite           Frontend development and build tool
  Node.js        Backend runtime
  Express.js     REST API development
  MongoDB        Database for users, food listings and requests
  Mongoose       MongoDB data modelling and database interaction
  Axios          Communication between frontend and backend APIs
  React Router   Client-side navigation
  CSS            Responsive interface styling
  Git            Version control
  GitHub         Source-code management

------------------------------------------------------------------------

## 7. Repository Structure

``` text
FoodSave/
│
├── backend/
│   ├── config/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   └── server.js
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   │   ├── common/
│   │   │   ├── food/
│   │   │   └── dashboard/
│   │   ├── pages/
│   │   │   ├── Home/
│   │   │   ├── Food/
│   │   │   ├── Business/
│   │   │   ├── Recipient/
│   │   │   └── Admin/
│   │   ├── services/
│   │   │   └── api.js
│   │   ├── routes/
│   │   │   └── AppRoutes.jsx
│   │   ├── styles/
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── package.json
│   └── vite.config.js
│
└── README.md
```

------------------------------------------------------------------------

## 8. AI Tools Used

### ChatGPT

ChatGPT was used as an AI-assisted development tool during the
development of FoodSave.

It was used for:

-   Problem ideation
-   Defining the project features
-   Backend structure planning
-   Frontend setup
-   UI component development
-   Backend and frontend code assistance
-   Debugging
-   Sample data generation
-   Food listing implementation
-   Food request management
-   Login UI development
-   Documentation support

All AI-generated outputs were reviewed, modified, integrated, and tested
by the team.

------------------------------------------------------------------------

## 9. AI Usage Declaration

ChatGPT was used during the development of FoodSave for problem
ideation, UI component generation, backend and frontend code assistance,
debugging, sample data generation, and documentation support.

The generated outputs were reviewed, modified, integrated, and tested by
the team. The team understands the submitted implementation and takes
responsibility for the final software solution.

------------------------------------------------------------------------

## 10. Team Members and Contributions

  -----------------------------------------------------------------------
  Student ID              Team Member             Contribution
  ----------------------- ----------------------- -----------------------
  IT24103346              Gunawardhana M.P.D.H    UI improvements,
                                                  testing functions to
                                                  ensure they work
                                                  properly, GitHub
                                                  management and
                                                  documentation

  IT24102768              Senadeera H.P.R.L.C     User login, frontend
                                                  development, navigation
                                                  and deployment

  IT24102743              Mihigurathna M.D.S.M    Backend development and
                                                  database integration

  IT24101938              Janith W.A.L            Admin login, frontend
                                                  development, navigation
                                                  and responsive UI
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## 11. Installation and Execution

### Prerequisites

Install the following before running FoodSave:

-   Node.js
-   npm
-   MongoDB / MongoDB Atlas
-   Git

------------------------------------------------------------------------

## 12. Clone the Repository

### Main Repository

``` bash
git clone https://github.com/sumudumudunayana/Food-Save.git
cd Food-Save
```

### Deployment Repositories

The project also contains separate repositories used for deployment:

**Frontend Repository**

https://github.com/sumudumudunayana/Food-Save-Frontend.git

**Backend Repository**

https://github.com/sumudumudunayana/Food-Save-Backend.git

------------------------------------------------------------------------

## 13. Backend Setup

Open a terminal and navigate to the backend folder:

``` bash
cd backend
```

Install dependencies:

``` bash
npm install
```

Create a `.env` file inside the backend folder.

Example:

``` env
PORT=5300
MONGODB_URI=YOUR_MONGODB_CONNECTION_STRING
```

Replace `YOUR_MONGODB_CONNECTION_STRING` with the MongoDB connection
string used by the project.

Start the backend:

``` bash
npm start
```

If the project uses a development script:

``` bash
npm run dev
```

The backend runs locally on:

``` text
http://localhost:5300
```

------------------------------------------------------------------------

## 14. Frontend Setup

Open another terminal and navigate to the frontend folder:

``` bash
cd frontend
```

Install dependencies:

``` bash
npm install
```

Start the Vite development server:

``` bash
npm run dev
```

The frontend will normally be available at:

``` text
http://localhost:5173
```

Open the displayed URL in a web browser.

------------------------------------------------------------------------

## 15. Environment Variables

Sensitive configuration values such as database connection strings
should be stored in environment variables.

Do not commit passwords, database credentials, API keys, or other
sensitive information to GitHub.

Example:

``` env
MONGODB_URI=YOUR_MONGODB_CONNECTION_STRING
PORT=5300
```

The actual `.env` file should not be uploaded to the repository.

------------------------------------------------------------------------

## 16. API Overview

### Food Listing APIs

``` text
GET    /api/foods
GET    /api/foods/:id
POST   /api/foods
PUT    /api/foods/:id
DELETE /api/foods/:id
```

### Food Request APIs

``` text
GET    /api/requests
POST   /api/requests
PUT    /api/requests/:id/status
GET    /api/requests/business/:businessName
GET    /api/requests/recipient/:recipientName
```

These APIs allow the frontend to communicate with the Express.js backend
and MongoDB database.

------------------------------------------------------------------------

## 17. Deployed Application

### Frontend

https://food-save-frontend.vercel.app/

### Backend

https://food-save-backend.onrender.com

The frontend is deployed using Vercel and the backend is deployed using
Render.

------------------------------------------------------------------------

## 18. Demonstration Video

**Two-Minute Demonstration Video:**

> **TODO: Add the final demonstration video link here.**

The demonstration video should cover:

1.  The team and project
2.  The selected Sri Lankan problem
3.  The FoodSave solution
4.  The main working features
5.  The deployed application
6.  The expected impact

------------------------------------------------------------------------

## 19. Sample Data

FoodSave uses sample data relevant to the Sri Lankan food waste problem.

Example:

``` json
{
  "businessName": "Colombo Bakery",
  "foodName": "Vegetable Buns",
  "category": "Bakery",
  "description": "Fresh vegetable buns available at the end of the day.",
  "quantity": 20,
  "unit": "items",
  "location": "Colombo",
  "expiryDate": "2026-12-31T18:00:00.000Z"
}
```

Sample data is used to demonstrate food listing, browsing, searching,
filtering, and request functionality.

------------------------------------------------------------------------

## 20. Validation and Error Handling

FoodSave includes validation to handle incorrect or incomplete user
input.

Examples include:

-   Required fields are checked before submission.
-   Food quantity must be at least 1.
-   Requested quantity must not exceed available quantity.
-   Requests cannot be created for unavailable food.
-   Invalid request statuses are rejected.
-   Collected requests cannot be changed.
-   Food listings can become unavailable after expiry.

The application provides meaningful error messages to help users correct
their input.

------------------------------------------------------------------------

## 21. Expected Impact

FoodSave aims to provide a practical digital solution to surplus food
waste in Sri Lanka.

The platform can help:

-   Reduce unnecessary food waste.
-   Make surplus food easier to discover.
-   Connect food businesses with potential recipients.
-   Improve redistribution of usable surplus food.
-   Help recipients find available food.
-   Provide businesses with a simple way to manage surplus food
    requests.

The main value of FoodSave is creating a simple digital connection
between food providers and people or organizations that can make use of
surplus food.

------------------------------------------------------------------------

## 22. Minimum Software Requirements

FoodSave addresses the minimum requirements of the SE3090 Mini
Hackathon:

  --------------------------------------------------------------------------
  Requirement                            FoodSave Implementation
  -------------------------------------- -----------------------------------
  Clear landing/main UI                  FoodSave user interface and login
                                         page

  Sri Lankan problem explanation         Food waste problem and FoodSave
                                         solution

  At least two functional features       Food listing, browsing,
                                         search/filtering and requests

  User-input form                        Food listing and food request forms

  Input validation                       Form validation and request
                                         quantity validation

  Display/search/filter/update/process   Food search/filtering and request
  information                            status processing

  Responsive interface                   Responsive CSS-based interface

  Basic navigation                       React Router navigation

  Relevant sample data                   Surplus food sample listings

  Demonstration of value to Sri Lankan   Surplus food redistribution
  users                                  workflow
  --------------------------------------------------------------------------

------------------------------------------------------------------------

## 23. GitHub Repository

### Main Repository

https://github.com/sumudumudunayana/Food-Save.git

### Frontend Repository

https://github.com/sumudumudunayana/Food-Save-Frontend.git

### Backend Repository

https://github.com/sumudumudunayana/Food-Save-Backend.git

The repositories contain the FoodSave source code and deployment-related
code.

The project uses Git and GitHub for source-code management and
collaborative development.

------------------------------------------------------------------------

## 24. Conclusion

FoodSave demonstrates how a practical web-based software solution can
address the problem of surplus food waste in Sri Lanka.

By allowing food businesses to list surplus food and recipients to
discover and request it, FoodSave creates a simple digital workflow for
surplus food redistribution.

The project uses the MERN stack to provide a working prototype with food
listing, browsing, searching, filtering, food requests, request
management, validation, and status tracking.

------------------------------------------------------------------------

## Project Information

**Project:** FoodSave\
**Group Number:** 2026-AI-41\
**Module:** SE3090 - Software Engineering Frameworks\
**Assignment:** Assignment 2 - Mini Hackathon\
**Institution:** Sri Lanka Institute of Information Technology (SLIIT)\
**Year:** 3\
**Semester:** 1 - 2026\
**Specialization:** Artificial Intelligence\
**Campus:** Malabe
