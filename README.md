
# Project Setup & API Guide
#credentials 
email: kiral2084@gmail.com
password:Vishaaal@11
## Prerequisites

- Node.js (LTS version recommended)
- npm (comes with Node.js)
- MongoDB (local or cloud, e.g., MongoDB Atlas)
- Postman (for API testing)

---

## Installation

### Frontend

```bash
cd frontend
npm install
npm run dev

### Backend

cd backend
npm install
npm run dev

All APIs require Authorization via JWT token.
In Postman, go to Headers and set:

Authorization: Bearer {token}

1. Top Product API

POST https://mernback-2-x047.onrender.com/api/v1/all/top

Request Body:

{
  "name": "RedBull",
  "rating": 5
}

2. Invoice API

POST https://mernback-2-x047.onrender.com/api/v1/invoice

Request Body:

{
  "invoiceId": "1002",
  "refernce_number": "02",
  "amount": 6000,
  "status": "Paid",
  "due_date": "23-oct-2025"
}

3. Sales API

POST https://mernback-2-x047.onrender.com/api/v1/sale

Request Body:

{
  "totalSales": 150,
  "totalRevenue": 4000,
  "totalCost": 3600
}

4. Chart API

POST https://mernback-2-x047.onrender.com/api/v1/all/chart

Request Body:

{
  "name": "sun",
  "sales": 20000,
  "purchase": 14000
}
```
