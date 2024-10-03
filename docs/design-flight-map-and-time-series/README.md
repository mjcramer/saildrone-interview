# **Design Document for FlightRadar24 Features**
## **Flight Map and Flight Time Series**

**Date:** October 4, 2024  
**Author:** Michael Cramer
**Reviewers:** Jeff Wang

---

### **Table of Contents**

1. [**Overview**](./overview.md#overview)
   
   1.1 [Assumptions](./overview.md#assumptions)

2. [**Feature 1: Live View of Flights**](./feature-1-live-flight-view.md)

   2.1. Data Pipeline

   2.2. Data Model

   2.3. Storage Solution

   2.4. Query and API Design

3. [**Feature 2: Time Series Flight Data**](./design-flight-map-and-time-series/feature-2-time-series-flight-data.md)

   3.1. Data Pipeline

   3.2. Data Model

   3.3. Storage Solution

   3.4. Query and API Design

4. [**Architectural Considerations**](./design-flight-map-and-time-series/4.architectural-considerations.md)

   4.1. Scalability

   4.2. Latency

   4.3. Resiliancy / Fault Tolerance 

   4.4. Data Integrity

   4.5. Security 


5. [**Technologies and Tools**](./design-flight-map-and-time-series/5.technologies-and-tools.md)

   5.1 Kafka

   5.2 Tile38

   5.3 Postgres / TimescaleDB

   5.3 Kubenetes 


6. [**Milestones**](./design-flight-map-and-time-series/6.milestones.md)

   6.1 Infrastructure
      a. Data Pipeline
      b. Datbases
      c. Clusters 

   6.2 Streaming Agents

   6.3 API Agents 

   6.4 Feature 1 Complete

   6.5 Feature 2 Complete  
