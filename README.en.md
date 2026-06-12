# **⚡ Smart Energy-Aware Production Scheduling Platform**

<div align="center">
  <a href="./README.md"><img src="https://img.shields.io/badge/Language-中文-blue" alt="中文"></a>
  <a href="./README.en.md"><img src="https://img.shields.io/badge/Language-English-blue" alt="English"></a>
</div>

This is a next-generation intelligent advanced planning and scheduling algorithm engine platform built for **industrial scheduling, comprehensive energy scenarios**, and complex manufacturing process constraints. The system adopts an architecture that couples front-end machine learning prediction with back-end operations research optimization in multiple stages, maximizing production efficiency while smoothing peak power consumption and meeting dual-carbon constraints.

<div align="center">
  <table border="0" style="border-collapse: collapse; margin: 0 auto; text-align: center; width: 100%; max-width: 900px;">
    <tr>
      <td style="width: 50%; padding: 12px; border: none; text-align: center; vertical-align: middle;">
        <img src="./images/ScreenShot_2026-06-09_214341_943.png" width="100%" style="border-radius: 4px; display: block; margin: 0 auto;">
      </td>
      <td style="width: 50%; padding: 12px; border: none; text-align: center; vertical-align: middle;">
        <img src="./images/ScreenShot_2026-06-09_214358_867.png" width="100%" style="border-radius: 4px; display: block; margin: 0 auto;">
      </td>
     <td style="width: 50%; padding: 12px; border: none; text-align: center; vertical-align: middle;">
        <img src="./images/ScreenShot_2026-06-09_214418_007.png" width="100%" style="border-radius: 4px; display: block; margin: 0 auto;">
      </td>
      <td style="width: 50%; padding: 12px; border: none; text-align: center; vertical-align: middle;">
        <img src="./images/ScreenShot_2026-06-09_214431_574.png" width="100%" style="border-radius: 4px; display: block; margin: 0 auto;">
      </td>
    </tr>
  </table>
</div>

## **🧬 Core Capabilities**

Our capabilities cover but are not limited to the following industrial scenarios and algorithmic frameworks:

### **1\. Industrial Power & Comprehensive Energy Scenarios**

* **Short and Medium-Term Load Analysis & Optimization Suggestions**  
  * **Scenario**: Extracting historical production orders, on-site production rhythms, electricity consumption features, and climate factors to analyze shop-floor energy consumption patterns. Accurately identifying energy efficiency bottlenecks and peak load risks, dynamically outputting load-shifting schemes.  
  * **Core Algorithms**: K-Means++ / Isolation Forest / LightGBM  
* **Short and Ultra-Short-Term Electricity Price Forecasting**  
  * **Scenario**: Forecasting price trends for spot power trading, dynamic time-of-use pricing, tiered pricing, and real-time dynamic fluctuating pricing, guiding adjustments to production plans for the next 1-3 days.  
  * **Core Algorithms**: ARIMA / Prophet / CatBoost / Quantile Regression  
* **Comprehensive Factory Energy Synergy Management**  
  * **Scenario**: Coordinating and optimizing factory distributed photovoltaic power output forecasting, energy storage system charge/discharge strategies, and multi-energy complementary scheduling like diesel generators/waste heat power generation.  
  * **Core Algorithms**: MILP (Mixed Integer Linear Programming)  
* **Flexible Equipment Switching Path Optimization**  
  * **Scenario**: Modeling power and resource consumption switching paths across different equipment states such as processing, standby, sleep, shutdown, and startup/preheating.  
  * **Core Algorithms**: Markov Decision Process / MINLP / CP (Constraint Programming)  
* **Dual-Carbon Goals & Carbon Footprint Constraints**  
  * **Scenario**: Combining the real-time grid green power ratio and real-time carbon emission factors to calculate and smooth out the overall carbon equivalent of scheduling plans.  
  * **Core Algorithms**: NSGA (Non-dominated Sorting Genetic Algorithm)

### **2\. Process Topology, Capacity & Supply Chain Constraints**

* **Complex Process Path Modeling**  
  * **Scenario**: Supporting complex process path topology modeling, automatic splitting and merging of work orders, and complex inter-dependency logic between processes.  
  * **Core Algorithms**: CPM / GCN (Graph Convolutional Network) / TS  
* **Flexible Multi-Alternative Process Modeling**  
  * **Scenario**: Resolving scheduling conflicts when workpieces repeatedly return to the same equipment group (e.g., PCBA, surface treatment, semiconductors) or flow flexibly across workshops.  
  * **Core Algorithms**: TS / CP (Constraint Programming)  
* **Rigid Continuous Production Constraints**  
  * **Scenario**: Strictly controlling the maximum/minimum waiting time between processes to satisfy rigid timing constraints like anti-deterioration and anti-cooling in chemical and die-casting processes.  
  * **Core Algorithms**: CP-SAT  
* **High-Energy Changeover Cost Modeling**  
  * **Scenario**: Performing global optimization for nonlinear changeover times and switching costs formed by cross-dimensional attributes such as color, size, and material.  
  * **Core Algorithms**: LNS (Large Neighborhood Search) / SA / ACO  
* **Dynamic Material Kitting Modeling**  
  * **Scenario**: Introducing rigid constraints of in-transit procurement and dynamic material arrivals into scheduling to avoid work stoppages waiting for materials.  
  * **Core Algorithms**: Rolling Horizon Optimization / Stochastic Programming  
* **Real-time Rescheduling & Dynamic Disturbance Response**  
  * **Scenario**: Highly robust and agile adjustments to sudden on-site states like order insertions, equipment downtime, and material delays.  
  * **Core Algorithms**: PPO (Proximal Policy Optimization) / Incremental Scheduling

## **📦 Delivery System**

We provide a full-cycle delivery solution from "Business Definition" to "Algorithm Source Code" and "Digital Platform":

| Delivery Module | Content & Core Value | Business Model |
| :---- | :---- | :---- |
| **1\. Business Consulting** | **Modeling Boundary Definition**: Accurately distilling colloquial business realities from the manufacturing frontline into structured constraints and optimization goals. **Multi-Objective Decision Trade-offs**: Building a mathematical evaluation system among conflicting metrics such as on-time delivery rate, energy cost, and equipment utilization. | **Paid Project** |
| **2\. Algorithm Delivery** | **Multi-Stage Algorithm Coupling**: Combining front-end prediction with back-end operations scheduling to ensure rapid output of feasible baseline solutions under multiple extreme hard constraints. **Algorithmic Assetization**: Source code follows a strict layered architecture where data, prediction, and optimization are completely decoupled, facilitating secondary development and reuse. | **Paid Project** |
| **3\. Digital Platform** | **Software & Hardware Level Delivery**: Directly providing a microservice-based scheduling foundation platform with decoupled storage, computing, and services, supporting rapid Docker containerized deployment. **Standardized Technical Training**: Gantt chart and energy consumption dashboard training for production management personnel; parameter tuning and model interface maintenance training for technical teams. | **Free Project** |

## **🏗️ System Architecture**

The system adopts a modern cloud-native microservice architecture, equipped with a powerful heterogeneous data cleaning module that can automatically align chaotic on-site ERP / MES / local power monitoring data, achieving seamless decoupling of computing power and data services.

## **💬 Contact Us**

💡 **Discuss specific cooperation details and costs**. If you need customized algorithm validation or PoC testing for your company, please feel free to establish contact with us at any time!

<div align="center">
  <table border="0" style="border-collapse: collapse; margin: 0 auto; text-align: center; width: 40%; max-width: 900px;">
    <tr>
      <td style="width: 50%; padding: 12px; border: none; text-align: center; vertical-align: middle;">
        <img src="./images/20260610165812_180_223.jpg" width="100%" style="border-radius: 4px; display: block; margin: 0 auto;">
      </td>
      <td style="width: 50%; padding: 12px; border: none; text-align: center; vertical-align: middle;">
        <img src="./images/20260610212103_182_223.jpg" width="100%" style="border-radius: 4px; display: block; margin: 0 auto;">      
      </td>
    </tr>
  </table>
</div>
