# Guidewire-Hackathon

# AI Powered Parametric Insurance for Gig Workers

## Overview

Gig economy workers such as food delivery partners rely on daily earnings to sustain their livelihood. However, external disruptions such as heavy rainfall, extreme heat, air pollution, traffic restrictions, or government curfews can significantly reduce their working hours and income.

Traditional insurance systems require manual claim submissions and verification processes, making them slow and inefficient.

Our solution introduces an **AI-powered parametric insurance platform** that automatically compensates gig workers when predefined disruption triggers occur. By using real-time data and AI-based risk assessment, the system ensures quick payouts without requiring manual claim filing.

---

# Problem Statement

Gig workers face income instability due to unpredictable external factors. When these disruptions occur, workers often lose significant income but lack access to affordable and fast insurance solutions.

This project aims to build a system that:

* Protects gig workers against income loss
* Automatically detects disruption events
* Triggers instant compensation
* Uses AI to determine fair weekly premium pricing

---

# Persona Based Scenario

### Persona

Name: Rahul
Age: 26
Occupation: Food Delivery Partner (Swiggy/Zomato)
Location: Chennai

### Scenario

Rahul typically earns around **₹1200 per day** delivering food orders.

On a particular day, **heavy rainfall of 70mm** occurs in his area. Due to flooding and traffic disruptions, Rahul cannot complete many deliveries and loses potential income.

Since rainfall exceeds the predefined threshold, the system automatically detects the event and triggers a **₹300 payout** to Rahul without requiring him to submit a claim.

---

# Application Workflow

1. User registers on the platform.
2. User selects an insurance plan with a weekly premium.
3. AI calculates a risk score based on location and historical disruption data.
4. The system continuously monitors external data sources.
5. When a disruption trigger occurs:

   * The system identifies affected workers
   * Calculates compensation
   * Automatically credits payout to workers.

Workflow Summary:

User Registration
↓
AI Risk Assessment
↓
Weekly Premium Selection
↓
External Data Monitoring
↓
Trigger Detection
↓
Automatic Claim Processing
↓
Payout to Worker

---

# Weekly Premium Model

The platform uses a **risk-based pricing model** where weekly premium depends on:

* Worker location
* Historical disruption frequency
* Average weekly income
* Working hours

### Premium Formula

Weekly Premium = Base Rate × Risk Score × Average Weekly Income

### Example

| Worker  | City    | Risk Score | Weekly Premium |
| ------- | ------- | ---------- | -------------- |
| Rider A | Chennai | Medium     | ₹35            |
| Rider B | Mumbai  | High       | ₹50            |

### Insurance Plans

| Plan     | Weekly Premium | Maximum Payout |
| -------- | -------------- | -------------- |
| Basic    | ₹20            | ₹500           |
| Standard | ₹40            | ₹1000          |
| Premium  | ₹70            | ₹2000          |

---

# Parametric Triggers

The system uses external APIs to detect disruption events.

### Weather Trigger

If rainfall > 60mm → Automatic payout triggered

### Air Pollution Trigger

If AQI > 400 → Compensation activated

### Extreme Heat Trigger

If temperature > 42°C → Worker receives payout

### Curfew or Road Restriction

If delivery zone is restricted → Compensation credited

---

# AI / ML Integration

Artificial Intelligence plays a major role in three areas.

## 1. Premium Calculation

Machine learning models analyze historical disruption data to calculate fair risk-based premium pricing.

Possible models:

* Logistic Regression
* Random Forest

---

## 2. Income Prediction

AI predicts the expected income of a worker and estimates income loss.

Example:

Expected Daily Income: ₹1200
Actual Income: ₹600
Income Loss: ₹600

---

## 3. Fraud Detection

The system detects fraudulent claims using:

* GPS location verification
* Duplicate claim detection
* Worker activity validation

Example rule:

If worker location ≠ disruption location
→ Claim rejected

---

# Platform Choice

The solution uses a **mobile-first platform** because gig workers primarily operate using smartphones.

Benefits:

* Easy accessibility during delivery
* Real-time notifications
* GPS integration
* Instant payout alerts

A **web dashboard** is also provided for administrators to monitor system activity and analytics.

---

# Tech Stack

Frontend

* React.js
* Tailwind CSS

Backend

* Node.js
* Express.js

Database

* MongoDB

AI / ML

* Python
* Scikit-learn

APIs

* WeatherAPI
* OpenWeather AQI API
* OpenStreetMap + Leaflet

Payments

* Razorpay / UPI simulation

---

# Development Plan

### Phase 1 – Prototype

* User registration system
* Insurance plan selection
* External API integration

### Phase 2 – AI Integration

* Risk scoring model
* Fraud detection model

### Phase 3 – Automation

* Event trigger detection
* Automatic claim payout system

### Phase 4 – Dashboard

* Analytics dashboard
* Claim tracking and monitoring

---

# Future Enhancements

* Integration with Swiggy and Zomato partner APIs
* Real-time traffic disruption detection
* WhatsApp chatbot for worker support
* Blockchain-based claim transparency

---

# Conclusion

This platform aims to provide **fast, transparent, and automated income protection** for gig workers by combining real-time data, AI-driven risk analysis, and parametric insurance triggers.

By eliminating manual claim processes and ensuring rapid payouts, the system improves financial security for gig economy workers facing unpredictable disruptions.
