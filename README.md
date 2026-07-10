# Travel Planning Agent Suite

## 🧭 Repository Purpose

This repository is a specialized agent framework designed to facilitate the planning and coordination of complex travel itineraries. It houses multiple specialized AI agents, each responsible for a distinct aspect of trip planning (destinations, activities, accommodations, and overall travel coordination). The goal is to provide a structured, multi-faceted approach to creating detailed, personalized, and immersive travel guides, particularly focusing on off-the-beaten-path experiences.

## ✨ Available Agents

The following specialized agents are available within the `.github/agents` folder and can be invoked to handle specific tasks:

* **`destination-agent`**: Responsible for suggesting and detailing ideal travel locations.
* **`activity-agent`**: Focuses on recommending local activities, tours, and experiences at a given destination.
* **`accommodation-agent`**: Specializes in finding and recommending suitable places to stay, adhering to preferences like boutique hotels or budget options.
* **`travel-agent`**: The primary coordinator. This agent takes high-level requests, integrates input from the other agents, manages the overall timeline, and generates the final, cohesive travel plan.

## 📚 Instructions & Usage

The `.github/instructions` folder contains detailed instruction files for each agent. These files define the operational scope, constraints, and expected output format for the agents, ensuring consistency and quality in their output.

**File Structure Note:** All generated and finalized travel plans will be saved in a dedicated directory structure: `/destination/{destination_name}`, where `{destination_name}` is the name of the primary destination (e.g., `/destination/italy`).

### 🚀 How to Use the `travel-agent`

To use the full capabilities of the system, you should direct your requests to the `travel-agent`. Here are two example prompts demonstrating different use cases:

### Example 1: Initial High-Level Planning

Use this prompt when starting a new trip with general preferences.

> "i want to travel to italy in august. I would like to stay around two weeks preferably in a boutique hotel. I would like to visit castles and some villages. I would like to travel to place where there are not a lot of tourists to really capture the vibe of italy. Can you make a planning and save it to a folder named italy in the attached folder ?"

### Example 2: Iterative Planning & Modification

Use this prompt when refining an existing plan (e.g., switching out a region).

> "Thanks for the travel plan ! i discussed it with my wife and she says that "Puglia" is too far. Can you switch it out for another destination ? Save the travel plan to a V2 version of the attached file to leave this one intact"

---
*This documentation was generated to guide users on interacting with the travel planning agents.*
