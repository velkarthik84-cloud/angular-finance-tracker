# Angular Finance Tracker

A personal finance tracking web application built using Angular.
Assignment 4C — Deckzi Software Developer Pre-Recruitment Program — Section 4.

---

## Features

* Dashboard with total income, expenses, and balance
* Visual summary of expenses by category
* Add, edit, and delete transactions
* Categorize transactions (Food, Housing, etc.)
* Reactive Forms with validation
* Centralized error handling using HTTP interceptor
* Local data persistence using localStorage
* Responsive UI with modern design

---

## Tech Stack

| Technology     | Purpose                    |
| -------------- | -------------------------- |
| Angular        | Frontend framework         |
| TypeScript     | Strongly typed language    |
| RxJS           | Reactive programming       |
| Angular Router | Page navigation            |
| Reactive Forms | Form handling & validation |
| localStorage   | Data persistence           |

---

## Project Structure

angular-finance-tracker/
├── src/
│   ├── app/
│   │   ├── pages/
│   │   │   ├── dashboard/
│   │   │   ├── transactions/
│   │   │   └── categories/
│   │   ├── services/
│   │   │   ├── transaction.ts
│   │   │   ├── category.ts
│   │   │   └── notification.ts
│   │   ├── interceptors/
│   │   │   └── error-interceptor.ts
│   │   ├── app.routes.ts
│   │   ├── app.config.ts
│   │   └── app.ts
│   ├── environments/
│   ├── index.html
│   └── main.ts
├── dist/                     ← Production build output
├── angular.json
├── package.json
├── tsconfig.json
├── vercel.json               ← Deployment config
└── README.md

---

## Requirements

* Node.js installed
* Angular CLI installed

Check versions:
node --version
npm --version
ng version

---

## Setup Instructions

### 1. Clone the repository

git clone https://github.com/velkarthik84-cloud/angular-finance-tracker.git
cd angular-finance-tracker

### 2. Install dependencies

npm install

### 3. Run development server

ng serve

Open in browser:
http://localhost:4200

---

## Build for Production

ng build --configuration production

Output folder:
dist/angular-finance-tracker

---


## How to Use

### Dashboard

* View total income, expenses, and balance
* See expense distribution by category

### Transactions

* Add new transaction
* Edit existing transaction
* Delete transaction
* Form validation ensures correct input

### Categories

* View and manage categories
* Used for organizing expenses

---

## Validation Rules

* Title: Required, minimum 2 characters
* Amount: Required, must be greater than 0
* Category: Required
* Date: Required

---

## Error Handling

* Centralized using HTTP interceptor
* Displays user-friendly messages for:

  * Network errors
  * Server errors
  * Invalid requests

---


## Scripts

| Command       | Description            |
| ------------- | ---------------------- |
| npm start     | Run development server |
| npm run build | Build for production   |
| ng serve      | Start local server     |
| ng build      | Production build       |

---

## Common Issues

### Build fails

Fix TypeScript errors before deploying

### Page not loading after refresh

Ensure vercel.json is present

### Data disappears

Check localStorage implementation


