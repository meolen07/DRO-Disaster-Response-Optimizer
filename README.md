# DRO – Disaster Response Optimizer

DRO is an AI + quantum optimization decision-support concept for disaster response simulations in Central Vietnam.

## Overview

DRO helps disaster response coordinators prioritize victims and allocate rescue resources using AI risk scoring and QUBO-based optimization.

## Problem

Floods, storms, and landslides create fragmented SOS signals, blocked roads, limited rescue teams, and changing hospital capacity. Manual coordination can delay high-risk case prioritization.

## Solution

DRO proposes a web-based dashboard that:
- Scores victim and area risk using AI
- Formulates rescue dispatch as a QUBO problem
- Uses quantum or quantum-inspired optimization to assign teams, routes, and hospitals
- Compares optimized dispatch plans with greedy baselines in simulation

## Demo Scenario

The MVP scenario focuses on Thua Thien Hue, Central Vietnam, using simulated flood and landslide response data.

## AI Component

AI risk scoring uses features such as:
- Injury severity
- Flood depth
- Isolation time
- Victim vulnerability
- Road accessibility
- SOS message content

## Quantum Component

The dispatch problem is formulated as QUBO with binary variables representing whether rescue team i is assigned to victim or area j.

Objective:
- Minimize weighted response time
- Prioritize high-risk victims
- Penalize unsafe roads and capacity violations

Solvers:
- Quantum-inspired simulated annealing for MVP
- QAOA or quantum annealing for future experiments

## Current Status

This repository currently contains the SEA Quantathon proposal materials. A Streamlit prototype may be added in future iterations.

## Deliverables

- One-page summary
- Slide deck
- System architecture
- Future Streamlit simulation prototype

## Roadmap

Months 1–3: Data model, scenario pack, AI risk scoring MVP  
Months 4–6: QUBO formulation, dashboard, baseline comparison  
Months 7–12: API, NLP, benchmarks, pilot testing  
Months 13–24: Live data adapters, drone imagery, QPU trials, regional scale-out

## Disclaimer

DRO is designed for simulation, planning, and drill support. It does not replace human command authority or professional emergency response judgment.
