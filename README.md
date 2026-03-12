
# NestNavigate Home Buying Challenge

![React](https://img.shields.io/badge/React-18-blue)
![Vite](https://img.shields.io/badge/Vite-fast-green)
![TypeScript](https://img.shields.io/badge/TypeScript-strongly--typed-blue)
![Status](https://img.shields.io/badge/status-prototype-orange)

An interactive gamified learning experience designed to help first‑time home buyers recognize hidden property risks through quick decision‑based challenges.

Users review property listings, interpret subtle clues, and decide whether they should **Pick (Buy)** or **Pass (Skip)** the house. After each decision, the system reveals the hidden issue and explains the real‑world lesson.

The goal is to transform home‑buying education from passive reading into an **engaging, decision‑based learning experience**.

# Prototype Demo

The prototype demonstrates a gamified learning activity where users evaluate homes and decide whether they should purchase or skip the property.

Demo Flow:

1. Open the challenge page  
2. Review the property card  
3. Swipe or click **Pick / Pass**  
4. View the hidden issue reveal  
5. Learn the home buying lesson  
6. Continue to the next property

Run locally:

npm install  
npm run dev  

Then open:

http://localhost:5173

# Platform Areas Explored

During exploration of the NestNavigate platform, several areas were reviewed:

• Home buying educational modules  
• Learning progression features  
• Risk awareness lessons for first‑time buyers  
• Educational guides related to property evaluation  

Most learning content is delivered through **reading‑based lessons**.  
This revealed an opportunity to introduce a more **interactive learning activity** that allows users to practice decision‑making.

# Observations Leading to the Concept

Several insights influenced the concept:

Passive learning dominates many educational flows.

First‑time buyers often struggle to recognize warning signs in property listings.

Practical examples improve learning retention more than theory alone.

Gamification encourages repeat engagement and daily interaction.

These insights led to the creation of **Pick or Pass**, a gamified property evaluation challenge.

# Feature Concept

Pick or Pass introduces a short decision‑based challenge where users practice identifying risky properties.

Players review property cards containing key information:

• property price  
• number of rooms  
• house age  
• neighborhood rating  
• listing duration  
• seller notes  
• agent hints  

After reviewing the clues, the player decides whether to:

PICK (buy the house)  
PASS (skip the house)

The decision can be made using:

• button interactions  
• swipe gestures

After the decision is made, the platform reveals hidden issues and explains the lesson.

# Game Flow

1. User opens the NestNavigate challenge page  
2. User clicks **Start Challenge**  
3. A property scenario appears  
4. The user reviews the house details and hints  
5. The user chooses **Pick** or **Pass**  
6. The system reveals:
• whether the decision was correct  
• the hidden property issue  
• the learning point
7. Points are awarded or deducted  
8. The user proceeds to the next scenario

# Educational Learning Loop

The feature follows a clear educational feedback loop.

Step 1 — Decision  
The user evaluates property details and chooses Pick or Pass.
Step 2 — Outcome  
The system indicates whether the decision was correct.
Step 3 — Hidden Risk Reveal  
The property issue is revealed.
Example:
Hidden Risk: Sewer pipe leak causing sewage backup risk
Step 4 — Learning Reinforcement  
The system explains the lesson.
Example:
Learning Point: Always inspect plumbing systems and request a sewer inspection before purchasing.
This loop ensures that each interaction becomes a **learning moment** rather than just gameplay.

# Technical Architecture

The prototype is implemented using **React and TypeScript**.

Technology Stack:

Frontend: React  
Language: TypeScript  
Build Tool: Vite  
Animation: Framer Motion  
Data Source: JSON Mock Data

React was chosen because the feature is **UI‑heavy rather than physics‑based gameplay**.

A game engine like Phaser was not required because the concept does not involve:

• physics simulations  
• collision detection  
• sprite rendering

# Technical Implementation

Key components include:

GameCard.tsx  
RevealScreen.tsx  
NavBar.tsx

State management tracks:

• current property scenario  
• player decisions  
• score updates  
• level progression

Swipe gestures allow:

Swipe Right → Pick  
Swipe Left → Pass

Buttons are also provided for accessibility.

# Code Quality Considerations

TypeScript is used throughout the project to ensure:

• predictable data structures  
• safe component props  
• maintainable code

Timers used during animations are properly cleaned up using React hooks to prevent memory leaks.

Game scenarios are stored locally:

src/mock/houses.json

This keeps the prototype independent from external APIs.

# Responsive Design

The interface is designed to work across multiple screen sizes:

• desktop  
• tablet  
• mobile

Responsive techniques include:

• flexible card widths  
• adaptive layouts  
• responsive button placement

Swipe gestures also work on touch devices.

# Project Structure

src/

components/  
GameCard.tsx  
RevealScreen.tsx  
NavBar.tsx  

pages/  
LandingPage.tsx  
GamePage.tsx  

mock/  
houses.json  

App.tsx  
main.tsx


# Setup Instructions

1. Clone repository

git clone <repository-url>  
cd nestnavigate-game

2. Install dependencies

npm install

3. Start development server

npm run dev

4. Open application

http://localhost:5173

# Integration Guide

The challenge can be integrated into NestNavigate in several ways.

Option 1 — Dedicated Page

/challenges/home-buying-game

Advantages:

• simple integration  
• independent deployment  
• scalable feature module

Option 2 — Embedded Module

<iframe src="/challenges/home-buying-game"></iframe>

Option 3 — React Component Integration

<HomeBuyingChallenge />

This enables integration with:

• user accounts  
• progress tracking  
• learning modules

# Mock Data Example

Example property scenario stored in:

src/mock/houses.json

Example structure:

{
"title": "Mystery Basement House",
"price": "$320,000",
"rooms": 3,
"ageOfHouse": 42,
"listingPeriod": "67 days",
"neighborhoodRating": 7,
"sellerNote": "Charming older home with a basement.",
"agentHint": "Basement has a lot of character.",
"issue": "Sewer pipe leak",
"lesson": "Always inspect plumbing systems before purchase.",
"correctAction": "SKIP"
}

# Scoring System

Correct decision → +50 points  
Incorrect decision → −20 points

# Player Levels

0 — Getting Started  
500 — Rookie Buyer  
1000 — House Hunter  
1500 — Inspection Detective  
2000 — Smart Homeowner

# Key Design Decisions

React was chosen instead of a traditional game engine because the interaction is primarily UI‑driven.

Mock data is used instead of external APIs to keep the prototype predictable and self‑contained.

Card‑based interaction mirrors how buyers evaluate listings on real estate platforms.

Immediate feedback ensures every decision reinforces a learning lesson.

# Prototype Limitations

This prototype is intentionally simplified for demonstration purposes.

Current limitations:

• static mock property data  
• no user authentication  
• score resets on reload  
• limited property scenarios

These choices keep the project lightweight and easy to evaluate.

#  Future Enhancements

Potential improvements include:

• daily learning challenges  
• leaderboards  
• adaptive difficulty levels  
• AI‑generated property scenarios  
• integration with real estate datasets  
• user progress tracking

# Product Impact

This feature transforms static home‑buying education into **interactive decision‑based learning**.

Benefits include:

• higher engagement  
• stronger learning retention  
• improved decision‑making skills for first‑time buyers

# Contributions

This project is a prototype demonstrating how NestNavigate could deliver **gamified home‑buying education**.
