
# Thermal-Hydraulic CFD Analysis of a Plate-Fin Heat Exchanger

### 3D Single-Pass Counter-Current Flow Simulation | COMSOL Multiphysics

**Computational Fluid Dynamics (CFD) | Conjugate Heat Transfer | Thermal Management | Heat Exchanger Analysis**

---

## Project Overview

Plate-Fin Heat Exchangers (PFHEs) are compact thermal systems designed to transfer heat efficiently between two fluid streams while minimizing space and weight requirements. Their high surface-area-to-volume ratio makes them particularly relevant to applications requiring compact, lightweight, and efficient thermal management.

This project investigates the **thermal-hydraulic behaviour of a simplified single-pass section of a Plate-Fin Heat Exchanger** using COMSOL Multiphysics.

The three-dimensional computational model represents two adjacent nitrogen flow passages operating in a **counter-current configuration**, with an aluminium structure incorporating fins and a separating plate.

The analysis focuses on understanding:

- Heat transfer between hot and cold nitrogen streams.
- Velocity distribution within confined flow passages.
- Pressure losses associated with internal fluid flow.
- Temperature variation along the heat exchanger.
- The relationship between thermal performance and hydraulic behaviour.

The objective is to establish a fundamental understanding of coupled fluid flow and heat transfer in compact heat exchanger geometries.

---

## CFD Results and Discussion

### 1. Velocity Distribution

![Velocity Distribution](Velocity%20Contour.png)

The velocity contour illustrates the flow distribution across multiple cross-sectional planes of the heat exchanger.

The simulation shows a nonuniform velocity profile, with higher velocities near the centre of each passage and lower velocities close to the walls due to viscous effects.

**Simulation Results:**

| Parameter | Hot Passage | Cold Passage |
|---|---|---|
| Maximum Velocity | 5.3773 m/s | 4.8012 m/s |
| Average Velocity Magnitude | 2.6495 m/s | 2.4401 m/s |

**Engineering Significance:**

Understanding velocity distribution is important for evaluating flow resistance, identifying regions of nonuniform flow, and examining convective heat-transfer behaviour in compact channels.

---

### 2. Pressure Distribution

![Pressure Distribution](Pressure%20contour.png)

The pressure contour illustrates the pressure variation along the two nitrogen flow passages.

The computed pressure decreases along the respective flow directions, reflecting the pressure losses associated with fluid movement through the confined channels.

**Simulation Results:**

| Parameter | Hot Passage | Cold Passage |
|---|---|---|
| Inlet Pressure | 44.920 Pa | 43.392 Pa |
| Outlet Pressure | 0.095593 Pa | 0.061086 Pa |
| Pressure Drop | 44.82 Pa | 43.33 Pa |

**Engineering Significance:**

Pressure drop is an important consideration in thermal-fluid system design because excessive flow resistance increases pumping or compression requirements.

Characterizing pressure losses helps engineers assess the trade-off between compact heat exchanger geometry, fluid-flow requirements, and system efficiency.

---

### 3. Temperature Distribution

![Temperature Distribution](Temperature%20Contour.png)

The temperature contour shows the thermal distribution within the simplified heat exchanger section.

Under counter-current operation, the hot nitrogen stream transfers thermal energy through the aluminium structure toward the colder nitrogen stream.

The computed temperature fields show significant temperature variation along the passages.

**Simulation Results:**

| Parameter | Hot Passage | Cold Passage |
|---|---|---|
| Inlet Temperature | 126.85°C | 26.85°C |
| Outlet Temperature | 43.24°C | 111.41°C |
| Temperature Change | −83.61°C | +84.56°C |

The cold-side outlet temperature exceeds the hot-side outlet temperature, which is physically possible in counter-current heat exchangers.

**Engineering Significance:**

Temperature distribution analysis is important for assessing thermal transport, identifying temperature gradients, and understanding heat exchanger behaviour under different operating conditions.

These considerations are relevant to thermal management systems where controlled heat transfer and compact component design are essential.

---

### 4. Coupled Temperature and Fluid Flow

![Temperature and Fluid Flow](T%20%26%20F.png)

This visualization combines the temperature distribution with velocity vectors inside the heat exchanger.

It illustrates the interaction between fluid motion and thermal energy transport within the adjacent passages.

The combined visualization provides insight into:

- Convective transport of thermal energy.
- Flow behaviour within narrow channels.
- Thermal interaction between counter-current fluid streams.
- The influence of channel geometry on fluid and thermal behaviour.

**Engineering Significance:**

Coupled thermal-fluid analysis helps engineers understand how fluid-flow characteristics and temperature distributions interact within heat transfer equipment.

Such analysis supports the development and evaluation of compact thermal systems used in demanding operating environments.

---

## Preliminary Thermal Performance

The heat-transfer rate was estimated using:

Q = mc(change in Temperature)

Using the prescribed mass flow rate and an approximate constant specific heat capacity for nitrogen:

| Performance Metric | Estimated Result |
|---|---|
| Heat lost by hot nitrogen | 0.870 W |
| Heat gained by cold nitrogen | 0.879 W |
| Hot-side pressure drop | 44.82 Pa |
| Cold-side pressure drop | 43.33 Pa |

The estimated hot-side heat loss and cold-side heat gain show close agreement, with a preliminary energy-balance difference of approximately 1.1%.

These thermal results are estimates based on the extracted temperatures and constant specific heat assumptions. Further verification using mass-flow-weighted temperatures and mesh refinement is required for quantitative validation.

---


## Industrial Relevance and Applications

Plate-Fin Heat Exchangers (PFHEs) are important components in chemical and process industries, where efficient heat recovery, temperature control, and low pressure losses directly influence plant performance and operating costs.

This project demonstrates the application of CFD and conjugate heat-transfer analysis to understand the thermal-hydraulic behaviour of compact process equipment.

### 1. Chemical Process Equipment Design

Heat exchangers are integral to chemical processing units, including reactors, separation systems, and gas-processing equipment.

Thermal-hydraulic simulations support equipment design by evaluating:

- Fluid velocity and flow distribution within process channels.
- Pressure losses affecting pumping and compression requirements.
- Heat-transfer performance under specified operating conditions.
- The influence of channel geometry on thermal and hydraulic behaviour.

Such analysis provides a foundation for the thermal rating and design evaluation of industrial heat exchangers.

### 2. Refinery and Petrochemical Processing

Heat exchangers play an important role in refinery and petrochemical operations, including feed preheating, product cooling, and process heat recovery.

Efficient heat integration reduces external heating and cooling requirements, improving overall process energy efficiency.

Understanding temperature distributions and pressure drops is essential when evaluating heat-transfer equipment for integration into process systems.

### 3. Gas Processing and Cryogenic Applications

Compact plate-fin heat exchangers are particularly relevant to industrial gas processing, air separation, and cryogenic applications.

Their high surface-area-to-volume ratio enables efficient thermal exchange within compact equipment configurations.

CFD analysis helps investigate flow resistance, temperature gradients, and thermal behaviour in narrow passages, supporting the evaluation of compact gas-to-gas heat exchange systems.

### 4. Process Optimization and Energy Efficiency

In chemical plants, heat-transfer equipment must balance thermal performance against hydraulic losses.

Increasing heat-transfer capability may also increase pressure drop, resulting in greater pumping or compression energy requirements.

Thermal-hydraulic analysis supports engineering decisions involving:

- Heat recovery and utility consumption.
- Equipment sizing and thermal design.
- Pressure-drop constraints.
- Flow distribution and operating performance.
- Energy-efficient process equipment selection.

### 5. Simulation-Driven Equipment Engineering

Numerical simulation provides valuable insight into equipment behaviour before detailed design and physical testing.

By examining velocity, pressure, and temperature fields, engineers can identify potential performance limitations and investigate alternative operating conditions or geometries.

The present simplified PFHE model establishes a foundation for more advanced engineering studies involving thermal rating, design optimization, and integration of compact heat exchangers into chemical processing systems.

---

## Engineering Significance

This project connects fundamental principles of **fluid mechanics, heat transfer, and computational modelling** with practical challenges encountered in chemical process equipment engineering.

It demonstrates preliminary capabilities in:

- CFD-based evaluation of thermal-fluid equipment.
- Pressure-drop and flow-distribution analysis.
- Heat-transfer estimation and energy-balance assessment.
- Interpretation of numerical simulation results.
- Understanding thermal-hydraulic design trade-offs.

These capabilities are relevant to process design, equipment engineering, heat integration, and energy-efficiency improvement in chemical and petrochemical industries.


---

## Scope and Limitations

This study represents a simplified single-pass section rather than a complete industrial Plate-Fin Heat Exchanger.

The simulations were performed using a physics-controlled Normal mesh. Mesh-independence testing and experimental validation were not performed.

The heat-transfer rates are preliminary estimates and should not be interpreted as independently validated performance predictions.

Future extensions could include mesh-convergence studies, heat exchanger effectiveness evaluation, pressure-drop optimization, and comparative analysis of alternative fin geometries.

---

## Tools and Technical Skills

**Simulation Software:** COMSOL Multiphysics

**Technical Areas:**
- Computational Fluid Dynamics (CFD)
- Conjugate Heat Transfer
- Thermal-Hydraulic Analysis
- Laminar Flow Modelling
- Counter-Current Heat Exchange
- Numerical Simulation and Post-Processing
- Velocity, Pressure, and Temperature Field Analysis

---

## Author

**Baljit Kaur**  
Chemical Engineering  
National Institute of Technology Jalandhar

