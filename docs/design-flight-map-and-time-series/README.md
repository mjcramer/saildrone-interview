# **Design Document for FlightRadar24 Features**
## **Flight Map and Flight Time Series**

**Date:** October 4, 2024  
**Author:** Michael Cramer
**Reviewers:** Jeff Wang

---

### **Table of Contents**

1. [**Overview**](./1.overview.md#overview)
   
   1.1 [Assumptions](./1.overview.md#assumptions)

2. [System Design](./2.system-design.md)



3. [**Feature 1: Live View of Flights**](./3.feature-1-live-flight-view.md)

   3.1. Data Pipeline

   3.2. Data Model

   3.3. Storage Solution

   3.4. Query and API Design

4. [**Feature 2: Time Series Flight Data**](./4.feature-2-time-series-flight-data.md)

   4.1. Data Pipeline

   4.2. Data Model

   4.3. Storage Solution

   4.4. Query and API Design

5. [**Architectural Considerations**](./5.architectural-considerations.md)

   5.1. Scalability

   5.2. Latency

   5.3. Resiliancy / Fault Tolerance 

   5.4. Data Integrity

   5.5. Security 


6. [**Technologies and Tools**](./6.technologies-and-tools.md)

   6.1 Kafka

   6.2 Tile38

   6.3 Postgres / TimescaleDB

   6.3 Kubenetes 


7. [**Milestones**](./7.milestones.md)

   7.1 Infrastructure
      a. Data Pipeline
      b. Datbases
      c. Clusters 

   7.2 Streaming Agents

   7.3 API Agents 

   7.4 Feature 1 Complete

   7.5 Feature 2 Complete  
