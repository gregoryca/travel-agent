# Specialized Travel Agents Suite

## 🧭 Overview

This repository contains a suite of specialized AI agents designed to collaborate on complex, personalized, and immersive travel planning. Each agent has a dedicated domain expertise, allowing the system to handle multi-faceted requests—from initial inspiration to detailed itinerary creation.

The primary goal is to research the web, gather rich suggestions, and synthesize them into a cohesive travel plan saved in a structured folder.

## ✨ Core Agents

The system is comprised of the following specialized agents, each responsible for a distinct area of travel planning:

### 🗺️ 1. Destination Agent (`destination-agent`)

* **Primary Role:** Suggesting and detailing ideal travel locations and countries.
* **Scope:** Initial discovery of destinations based on user interests (e.g., culture, beaches, history). It provides high-level context and suggests regions.
* **Interaction:** It acts as the initial filter, helping narrow down the location options before deeper planning begins.

### 🌿 2. Activity Agent (`activity-agent`)

* **Primary Role:** Recommending local activities, tours, and experiences at a given destination.
* **Scope:** Suggesting points of interest, day trips, unique local experiences, and suggesting ways to "capture the vibe" of a place.
* **Interaction:** It builds out the daily itinerary framework once a destination is confirmed.

### 🏨 3. Accommodation Agent (`accommodation-agent`)

* **Primary Role:** Finding and recommending suitable places to stay.
* **Scope:** Suggesting types of lodging (e.g., boutique hotels, rustic inns, budget hostels) that fit the user's style and budget for the specified area.
* **Interaction:** It provides necessary logistical detail to round out the travel plan.

### 🧑‍✈️ 4. Travel Coordinator Agent (`travel-agent`)

* **Primary Role:** The central coordinator. This agent manages the overall workflow, takes high-level requests, integrates input from all specialized agents, manages the timeline, and generates the final, cohesive travel plan.
* **Scope:** Orchestration, constraint checking, and final output formatting.
* **Interaction:** It directs the flow of information, ensuring all parts of the trip (arrival, activities, stay, departure) fit together logically.

## 🍜 Supplementary Research Modules

These modules handle specific categories of suggestions that can be called upon by the primary agents:

* **Dining/Culture:** Suggestions for local restaurants, bars, and unique cultural spots (Historical monuments or Historical tours).
* **Nature:** Identifying beautiful natural places to visit.

## 📂 Workflow & Output Structure

1. **Research:** Agents search the web for suggestions and detailed information.
2. **Context Passing:** If any agent lacks context, the `travel-agent` is responsible for asking the user clarifying questions and passing the retrieved context to the correct specialist agent.
3. **Saving:** Upon completion of the planning phase, the entire research/planning must be saved as a `{country_name}-{arrivaldate}.md` file in the following structure:
    `/destinations/{country_name}/`
    *(The `{country_name}` folder will be created if it doesn't already exist.)*
    *(Make sure to create a new version in the `{country_name}` folder if there already exists a travel plan)*
