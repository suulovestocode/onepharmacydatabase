# 💊 OnePharmacy
## Government-Oriented Pharmacy Transparency & Drug Authentication Platform
## Overview

OnePharmacy is a full-stack MERN application designed to improve transparency and accountability in the pharmaceutical supply chain. The system focuses on two critical public health challenges:

•Circulation of counterfeit medicines

•Unregulated pricing markups across pharmacies

The platform provides a centralised government-managed database where pharmacies register their information, maintain drug inventories, and submit pricing data. The system automatically detects suspicious price markups and allows consumers to verify the authenticity of medicines through serialized tracking.

The project aims to create a transparent pharmaceutical ecosystem where regulators, pharmacies, and consumers can interact through a unified digital platform. 

# 🚀 Key Features
## Pharmacy Registration & Data Aggregation

•Enables pharmacies to register with the system

•Stores critical details such as:

  •Pharmacy name

  •Location

  •Contact information

  •License history

•Creates a centralized government database of authorized pharmacies.

## Drug Serialization & Authenticity Verification

•Each drug unit is assigned a unique identifier

•Tracks medicines using:

  •Batch number

  •Expiry date

  •Manufacturer information

•Creates a traceable chain of custody for pharmaceutical products.

Consumers can verify drug authenticity through a mobile interface by scanning the serialized identifier.

## Dynamic Inventory Management

•Pharmacies maintain real-time drug inventory

•Tracks available stock across pharmacies

•Supports updates through integrated APIs.

## Pricing Transparency & Markup Detection

•Pharmacies submit both:

  •Buying price

  •Selling price

The system calculates markup automatically and triggers alerts if pricing exceeds a configurable threshold, helping detect unethical or exploitative pricing.

## Consumer Transparency

Consumers can:

•Compare prices across pharmacies

•Detect abnormal markups

•Verify medicine authenticity

•Ensure they are purchasing legitimate drugs.

This promotes public trust and healthcare transparency.

# 🧠 System Architecture

The system follows a MERN full-stack architecture:

React (Frontend UI)
        │
        ▼
Axios API Calls
        │
        ▼
Node.js + Express Backend
        │
        ▼
MongoDB Database

The architecture allows:

•Real-time updates

•Fast API communication

•Scalable backend storage

•Efficient data management.

🛠 Tech Stack
Frontend

•React.js

•Bootstrap

•Vite

•Axios for API communication

Backend

•Node.js

•Express.js

Database

•MongoDB

•MongoDB Compass for schema validation and inspection

Key Packages

•Mongoose

•MongoShell

•Express

•Axios

The platform enables seamless frontend-backend integration and real-time updates through REST APIs. 

# 🗄 Database Design

The system includes several structured collections designed to manage pharmaceutical data.

## Pharmacy Collection

Stores pharmacy details.

Fields include:

•pharmacy_id

•name

•location

•phone_number

•permit_number

## Drug Collection

Stores information about medicines.

Fields include:

•drug_id

•drug_name

•description

## Stock Collection

Tracks inventory of medicines across pharmacies.

Fields include:

•pharmacy_id

•drug_id

•quantity

## Price Collection

Handles pricing transparency.

Fields include:

•pharmacy_id

•drug_id

•buying_price

•selling_price

•markup

## Transaction Collection

Records medicine purchases.

Fields include:

•transaction_id

•pharmacy_id

•drug_id

•quantity

•customer_name

•date

The schema normalisation and structure are shown in the database diagrams included in the project report. 

# 🔄 Real-Time System Workflow

1️⃣ Pharmacy registers in the system

2️⃣ Drug inventory is uploaded into the database

3️⃣ Price information is submitted

4️⃣ System calculates markup automatically

5️⃣ Alerts are triggered if markup exceeds threshold

6️⃣ Consumers verify drugs through serialized tracking

This ensures full traceability across the pharmaceutical supply chain.

# 🖥 User Interface

The platform provides a simple administrative interface that allows:

•Adding new pharmacies

•Managing drug inventory

•Updating pricing information

•Monitoring database records

The UI is built using React with Bootstrap styling, allowing a responsive and efficient interface for managing pharmacy data.

Real-time updates are reflected in the MongoDB database through API calls. 

# 📂 Project Structure
OnePharmacy
│

├── client

│   ├── src

│   │   ├── AddDrug.jsx

│   │   ├── AddPharmacy.jsx

│   │   ├── AddPrice.jsx

│   │   ├── AddStock.jsx

│   │   ├── AddTransaction.jsx

│   │   ├── Pharmacies.jsx

│   │   ├── Drugs.jsx

│   │   ├── Prices.jsx

│   │   └── Stock.jsx

│

├── server

│   ├── models

│   └── index.js

This modular structure allows scalable expansion of the platform.

# 🌍 Real-World Impact

The system is designed to support government initiatives for:

•Combating counterfeit medicines

•Ensuring ethical drug pricing

•Increasing transparency in the pharmaceutical industry

•Improving consumer trust in healthcare systems

By introducing drug traceability and markup monitoring, the project provides a technological solution to major challenges in pharmaceutical regulation.

# 📈 Future Enhancements

Potential extensions include:

•QR code scanning for drug verification

•Mobile application for consumers

•AI-based anomaly detection for pricing patterns

•Blockchain-based drug supply chain tracking

•Integration with government health databases

# 👩‍💻 Authors

Suhani Srivastava

B.Tech Computer Science

VIT Chennai
