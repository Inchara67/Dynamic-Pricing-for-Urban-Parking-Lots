# Dynamic Pricing for Smart Parking using Pathway

## Overview

This project is a real-time dynamic pricing engine for smart parking systems. Using a live data stream, it simulates parking lot status and calculates optimal prices based on occupancy, demand, competition, and other real-world metrics. The project leverages **Pathway**, a real-time data processing engine, to demonstrate how dynamic pricing adapts on the fly for maximum efficiency and revenue.

---

## Tech Stack Used

- **Python 3**
- **Pathway** – for real-time data stream processing
- **Pandas / NumPy** – for data handling and computation
- **Bokeh** – for real-time visualizations
- **Jupyter Notebook / Google Colab** – for development and experimentation

---

## Architecture Diagram

```mermaid
graph TD
    A[CSV Dataset] --> B[Pathway Streaming Engine]
    B --> C[Model 1 - Linear Pricing]
    B --> D[Model 2 - Demand Based Pricing]
    B --> E[Model 3 - Competitive Pricing]
    C --> F[Pricing Output]
    D --> F
    E --> F
    F --> G[Bokeh Dashboard]
