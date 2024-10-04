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

  2.1. [`Kafka` for Message Queue / Data Pipeline](./2.system-design.md#21-message-queue--data-pipeline)

  2.2. [`Kubernetes` for Container Orchestration](./2.system-design.md#22-kubernetes-for-container-orchestration)

  2.3. [`Tile38` for Real-Time Geospatial Querying](./2.system-design.md#23-tile38-for-real-time-geospatial-querying)

  2.4. [`Postgres` with `TimescaleDB` extension for Geospatial Time Series Data Storage](./2.system-design.md#24-postgres-with-timescaledb-extension-for-geospatial-time-series-data-storage)

3. [Feature 1: Live View of Flights](./3.feature-1-live-flight-view.md)

  3.1. [Active Flight Data Updater](./3.feature-1-live-flight-view.md#31-active-flight-data-update)

  3.2. [Active Flight API](./3.feature-1-live-flight-view.md#32-active-flight-api)

  3.3. [Cleaner](./3.feature-1-live-flight-view.md#33-cleaner)


4. [Feature 2: Time Series Flight Data](./4.feature-2-time-series-flight-data.md)

   ## 4.1. [Data Model](./4.feature-2-time-series-flight-data.md#41-data-model)

   ## 4.2. [Historical Flight Data Aggregator](./4.feature-2-time-series-flight-data.md#42-historical-flight-data-aggregator)

   ## 4.3. [Historical Flight Data API](./4.feature-2-time-series-flight-data.md#43-historical-flight-data-api)

   ## 4.4. [Cleaner](./4.feature-2-time-series-flight-data.md#44-cleaner)


5. [Architectural Considerations](./5.architectural-considerations.md)

   5.1. [Scalability](./5.architectural-considerations.md#51-scalability)

   5.2. [Latency](./5.architectural-considerations.md#52-latency)

   5.3. [Resiliancy](./5.architectural-considerations.md#53-resiliancy)

   5.4. [Data Integrity](./5.architectural-considerations.md#54-data-integrity)

   5.5. [Security](./5.architectural-considerations.md#55-security)

   5.6. [Monitoring and Alerting](./5.architectural-considerations.md#56-monitoring-and-alerting)
   