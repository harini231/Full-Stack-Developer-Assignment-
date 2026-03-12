
# Pick or Pass – Gamified Home Buying Decision Challenge

# Overview

Pick or Pass is an interactive learning challenge designed for the Nest Navigate platform. The feature presents users with realistic house listings and asks them to quickly decide whether they should buy the home or skip it. Instead of passively reading about home buying concepts, users actively evaluate properties using clues such as price, neighborhood rating, listing duration, and seller notes.

The goal of the feature is to turn learning about home buying risks into a short and engaging decision-based experience. By interacting with property cards and receiving feedback on their choices, users can practice recognizing common mistakes that first-time home buyers often make.

This concept aligns with Nest Navigate’s mission of helping users build confidence in the home buying process through interactive and educational experiences.

# Problem Observed

While exploring the Nest Navigate platform and its learning flow, it became clear that many educational experiences rely heavily on reading or passive content consumption. Although this content provides valuable information, users may lose engagement if they are only reading lessons without opportunities to apply what they have learned.

First-time home buyers often struggle with recognizing hidden risks in property listings. Without practice evaluating real scenarios, it can be difficult to translate theoretical knowledge into confident decision-making.

This observation led to the idea of creating a short, repeatable challenge where users can practice evaluating home listings in a safe environment while learning from their mistakes.

# Feature Concept

Pick or Pass introduces a gamified decision challenge where users review property cards and decide whether the home is a good investment.

Each card presents key information about a home, including:

- Property price
- Number of rooms
- Age of the house
- Neighborhood rating
- Listing duration
- Seller note
- Agent hint

After reviewing this information, the user makes a decision:

- Pick (Buy the house)
- Pass (Skip the house)

The decision can be made by either pressing the action buttons or swiping the card left or right. This interaction keeps the experience simple, fast, and engaging.

After the user makes a decision, the system immediately reveals hidden information about the property and explains whether the decision was correct. This feedback creates a learning loop that helps users understand what signals they should watch for when evaluating homes.

# Educational Learning Loop

The feature is designed around a clear learning cycle:

1. User Action 
   The user evaluates the house information and chooses Pick or Pass.

2. Outcome Feedback 
   The system reveals whether the decision was correct or risky.

3. Hidden Risk Explanation  
   The feature explains the hidden issue associated with the property.

4. Learning Reinforcement  
   A “Learning Point” message explains what the user should look for in real home-buying scenarios.

Example:

- Hidden issue: Sewer pipe leak risk
- Learning point: Always inspect plumbing systems and request a sewer inspection before purchasing a home.

This cycle ensures that each decision becomes a small educational moment rather than just a game result

# Platform Integration

Pick or Pass fits naturally into the Nest Navigate ecosystem and learning journey.

The feature can be integrated into the platform in several ways:

Daily Challenge
The game can appear as a daily challenge on the dashboard where users can earn points for completing the activity.

Learning Reinforcement
After finishing lessons related to home buying, budgeting, or property evaluation, users can play the challenge to practice applying what they learned.

Progress and Rewards
The feature integrates with the platform’s progress system by awarding points or coins based on performance.

Skill Building
By repeatedly evaluating different properties, users gradually build stronger instincts for identifying good or risky home purchases.

This integration allows the feature to feel like a natural extension of the existing Nest Navigate learning experience.

## User Experience Flow

The user experience is designed to be simple and intuitive.

1. The user logs into the Nest Navigate platform and sees the House Challenge on the dashboard.
2. The user clicks **Start Challenge** to begin the activity.
3. A property card appears showing key details about the house.
4. The user evaluates the information and chooses **Pick** or **Pass**.
5. The platform reveals hidden risks or confirms the correct decision.
6. A learning message explains what the user should look for in real home-buying situations.
7. The user receives a score update and moves on to the next property card.

Each round takes only a few seconds, allowing users to quickly practice multiple decisions in one session.

# Technical Approach

The prototype was built using **React and TypeScript**, which aligns with the UI-heavy nature of the feature.

The implementation focuses on:

- Component-based architecture
- Interactive swipe and button actions
- Responsive layout for desktop and mobile devices
- Mock data representing realistic property listings
- Clean state management for score tracking and card progression

React was chosen instead of a traditional game engine because the feature relies primarily on UI interactions rather than physics, collision detection, or sprite-based animations.

# Design Decisions

Several design decisions were made to keep the experience engaging and easy to understand.

Card-Based Interaction
Using property cards allows users to quickly scan information and make decisions without feeling overwhelmed.

Swipe Interaction
Swiping left or right provides a natural and playful interaction while still supporting button-based actions for accessibility.

Immediate Feedback
Users receive feedback immediately after making a decision, reinforcing the educational value of each interaction.

Story-Based Reveals
Messages such as “Plot twist” or “Hidden risk” make the learning experience feel more memorable and engaging.

# Visual Risk Indicators
Risk bars and score updates help users understand the severity of potential property issues.

# Why This Feature Increases Engagement

Pick or Pass increases engagement because it transforms passive learning into an active experience.

Instead of simply reading about home buying mistakes, users practice identifying them in simulated scenarios. The quick decision format encourages repeated play, which helps reinforce learning over time.

Short challenge rounds also make the feature suitable for daily interaction. Users can quickly complete a challenge, learn something new, and return later to improve their performance.

By combining decision-making, storytelling, and feedback, Pick or Pass helps users develop practical home-buying instincts in a fun and interactive way.


# Future Improvements

Future versions of the feature could include:

- Daily challenge leaderboards
- Difficulty levels based on user progress
- More diverse property scenarios
- Achievement badges for learning milestones
- Additional risk categories such as financing, structural issues, or market trends

These improvements could further expand the educational value and replayability of the feature.
