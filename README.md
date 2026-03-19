# SmartShift: AI-Powered Income Protection for Gig Workers

## Introduction

SmartShift is a parametric insurance platform built to support delivery partners who depend on daily earnings. In real-world conditions, workers often face situations like heavy rain, pollution, or extreme heat that prevent them from working. When this happens, their income drops immediately, and there is no system in place to compensate for that short-term loss.

This project focuses on solving that problem by creating an automated system that detects such disruptions and provides instant financial support without requiring users to manually file claims.

---

## Problem Understanding

Delivery partners working with platforms like Swiggy and Zomato rely on consistent outdoor activity. However, external factors such as:

- Sudden rainfall
- High air pollution
- Extreme temperatures
- Restricted working zones

can significantly reduce their ability to complete orders. Even a few hours of disruption can impact their weekly earnings.

Traditional insurance products are not designed for these short, frequent disruptions. They are either too complex, too slow, or not relevant to the gig economy.

---

## What SmartShift Does

SmartShift introduces a simple idea: instead of waiting for users to report a problem, the system detects it automatically.

Once a disruption is identified, the system evaluates how much the worker’s activity has been affected and calculates the loss using a structured approach. If the impact crosses a certain threshold, the system triggers a payout instantly.

This removes the need for manual claims and reduces delays.

---

## How the System Works

1. A delivery partner registers on the platform and activates a weekly plan.
2. The system calculates a premium based on location, income level, and risk factors.
3. Once the policy is active, the system continuously monitors environmental conditions.
4. When a disruption occurs, the system evaluates its impact using a scoring model.
5. The system verifies whether the worker was genuinely affected.
6. If the conditions are met, the claim is automatically approved.
7. The payout is processed and reflected on the dashboard.

---

## Core Idea: Loss Score

Instead of making decisions based on a single condition, SmartShift uses a scoring system to determine whether a payout should be made.

The Loss Score represents how severely a worker’s income is affected.

Loss Score is calculated using:

Loss Score = (0.4 × Environmental Severity)  
           + (0.3 × Activity Drop)  
           + (0.3 × Order Drop)

- Environmental Severity reflects how strong the disruption is.
- Activity Drop measures the reduction in working hours.
- Order Drop measures the reduction in completed deliveries.

This approach ensures that payouts are based on real impact rather than just the presence of an event.

---

## Decision Logic

Based on the Loss Score:

- If the score is below 40, no payout is triggered.
- If the score is between 40 and 60, a partial payout is provided.
- If the score is above 60, a full payout is triggered.

This makes the system fair and predictable.

---

## Weekly Pricing Model

SmartShift uses a weekly subscription model that aligns with how gig workers earn.

The premium is calculated using:

Premium = Base × Zone Risk × Income Factor × Behavior Factor

This allows the system to adjust pricing based on real conditions instead of using a fixed value for everyone.

---

## Preventing False Claims

One of the challenges in such systems is ensuring that payouts are not misused.

To handle this, SmartShift does not rely on a single data point. Instead, it validates claims using multiple signals such as:

- Consistency of user activity
- Location patterns
- Matching environmental conditions

This helps in filtering out suspicious or invalid cases without adding complexity for genuine users.

---

## Technology Stack

The system is designed using a MERN-based architecture:

- Frontend: React.js for user interface
- Backend: Node.js with Express for APIs
- Database: MongoDB for storing user and policy data
- External Data: Weather APIs and simulated platform data

The focus is on keeping the system modular and easy to extend.

---

## Key Features

- Fully automated claim processing
- Real-time monitoring of external conditions
- Dynamic weekly premium calculation
- Transparent decision-making using a scoring model
- Simple and intuitive user interface

---

## Deployment Approach

The frontend can be deployed using static hosting platforms such as Vercel or Netlify. The backend can run on cloud services like Render or AWS, and MongoDB Atlas can be used for database hosting.

---

## Future Improvements

Some potential improvements include:

- Integration with real delivery platform APIs
- More advanced prediction models for risk estimation
- Mobile application for better accessibility
- Detailed analytics dashboard for both users and administrators

---

## Conclusion

SmartShift is designed to bring a practical solution to a real problem faced by gig workers. By combining automated detection, structured evaluation, and instant payouts, it creates a system that is both simple and effective.

The goal is to ensure that workers are not left without support when external conditions prevent them from earning.
