# EXPERIMENT 4 – PROMPT ENGINEERING PATTERNS

# Experiment No.: 4
# Name: siddharth g
# Register Number: 212223060263

---

## AIM

To write prompts for different prompt engineering patterns, execute them using different AI tools, compare the generated responses, and evaluate the results using a **Rubric-based evaluation method**.

The following prompt patterns are used:

1. Zero-Shot Prompting
2. Few-Shot Prompting
3. Chain-of-Thought Prompting
4. Persona Pattern
5. Reverse Prompting
6. Graph Prompting
7. Active Prompting

---

# 1. SCENARIO AND USE CASE

## Scenario

The manufacturing industry is looking to reduce manual monitoring and increase efficiency through automation.

The proposed system uses **IoT devices, sensors, embedded controllers, cloud platforms, and AI/ML techniques** to automate equipment monitoring, analyze machine performance, and enable predictive maintenance.

The system continuously collects machine parameters such as temperature, vibration, pressure, current, energy consumption, and machine operating status.

The collected data is analyzed to identify abnormal conditions and predict possible machine failures before they occur.

## Use Case

### IoT-Based Smart Manufacturing and Predictive Maintenance

The system is designed to monitor industrial machines in real time and predict failures before they cause unexpected downtime.

## Target Audience

The system is mainly intended for:

* Automotive manufacturing industries
* Electronics manufacturing industries
* Food processing industries
* Heavy machinery industries
* Industrial automation companies

## Main Objectives

* Improve production efficiency by **30%**.
* Minimize machinery downtime using predictive maintenance.
* Enable real-time monitoring of manufacturing systems.
* Enable remote monitoring and control.
* Reduce energy consumption through process optimization.
* Detect machine abnormalities at an early stage.
* Improve overall machine reliability and maintenance planning.

---

# 2. ZERO-SHOT PROMPTING

## Definition

Zero-shot prompting is a prompting technique in which the AI model is given a task **without providing any examples**.

The model generates the response using only the information and instructions provided in the prompt.

## Prompt

```text
Explain how an IoT-based predictive maintenance system can be implemented in a smart manufacturing industry. Describe the role of IoT sensors, embedded controllers, cloud platforms, AI models, real-time monitoring, and predictive maintenance. Explain how the system can reduce downtime, improve production efficiency, and reduce energy consumption. Present the answer in simple technical terms.
```

## Generated Response

An IoT-based predictive maintenance system continuously collects machine data using sensors such as temperature, vibration, pressure, and current sensors.

An embedded controller processes the sensor readings and sends the collected data to a cloud platform. AI and machine-learning models analyze the data to identify abnormal machine behavior and predict possible failures.

A monitoring dashboard displays the machine status in real time. When the system detects a possible failure, it generates an alert for the maintenance team.

This approach helps industries perform maintenance before a machine breaks down. It reduces unexpected downtime, improves production efficiency, increases machine reliability, and helps reduce unnecessary energy consumption.

## Evaluation

* Relevance: **5/5**
* Technical Accuracy: **4/5**
* Completeness: **4/5**
* Clarity: **5/5**
* Total Score: **18/20**

## Observation

Zero-shot prompting is simple and effective for general questions. However, the response may not always follow a specific format or provide highly detailed information.

---

# 3. FEW-SHOT PROMPTING

## Definition

Few-shot prompting provides the AI model with **a few examples** before asking it to solve a similar problem.

The examples help the AI understand the expected format, style, and type of response.

## Prompt

```text
Example 1:

Input:
Machine temperature is continuously increasing.

Output:
The system should generate a warning because increasing temperature may indicate overheating or component failure.


Example 2:

Input:
Machine vibration suddenly increases.

Output:
The system should identify the abnormal vibration and recommend inspection of bearings, motors, or rotating components.


Example 3:

Input:
Energy consumption is higher than normal.

Output:
The system should generate an energy alert and recommend checking machine efficiency and operating conditions.


Now analyze this situation:

A manufacturing machine shows increasing temperature, abnormal vibration, and higher energy consumption simultaneously. Predict the possible problem and recommend suitable maintenance actions.
```

## Generated Response

The machine may be experiencing one or more of the following problems:

* Bearing damage
* Motor problems
* Mechanical wear
* Poor lubrication
* Mechanical misalignment
* Excessive machine load

Since temperature, vibration, and energy consumption are increasing simultaneously, the machine can be classified as being in a **high-risk abnormal condition**.

### Recommended Maintenance Actions

1. Inspect the motor and bearings.
2. Check the lubrication system.
3. Examine mechanical alignment.
4. Check the machine load.
5. Reduce unnecessary machine load.
6. Schedule preventive maintenance.
7. Continue monitoring the sensor readings.

## Evaluation

* Relevance: **5/5**
* Technical Accuracy: **5/5**
* Completeness: **5/5**
* Clarity: **5/5**
* Total Score: **20/20**

## Observation

Few-shot prompting produces more consistent and structured responses because examples are provided to guide the AI.

---

# 4. CHAIN-OF-THOUGHT PROMPTING

## Definition

Chain-of-thought prompting is used to guide an AI model to solve a complex problem through a **logical sequence of steps**.

It is useful for problems that require analysis, diagnosis, or multiple stages of decision-making.

## Prompt

```text
Analyze the following smart manufacturing problem systematically.

A machine has a normal temperature of 60°C, but its temperature has increased to 85°C. Its vibration level has also increased significantly and its energy consumption is 20% higher than normal.

Determine the likely causes, identify the risk level, suggest maintenance actions, and explain how an IoT predictive-maintenance system should respond.

Provide the answer as a clear sequence of reasoning steps without revealing private internal reasoning.
```

## Generated Response

### Step 1 – Identify Abnormal Parameters

The machine temperature has increased from 60°C to 85°C.

The vibration level has also increased, and energy consumption is 20% higher than normal.

Therefore, multiple machine parameters indicate abnormal operation.

### Step 2 – Identify Possible Causes

Possible causes include:

* Bearing wear
* Motor problems
* Poor lubrication
* Mechanical misalignment
* Excessive machine load
* Component friction

### Step 3 – Determine Risk Level

The simultaneous increase in temperature, vibration, and energy consumption indicates a potentially serious machine condition.

The system should classify the machine as a **high-risk condition**.

### Step 4 – Generate Alert

The IoT monitoring system should generate a high-priority maintenance alert.

### Step 5 – Perform Maintenance

The maintenance team should inspect:

* Motor
* Bearings
* Lubrication
* Mechanical alignment
* Machine load

### Step 6 – Continue Monitoring

After maintenance, the system should continue monitoring the machine parameters to confirm that the machine has returned to normal operation.

## Evaluation

* Relevance: **5/5**
* Logical Organization: **5/5**
* Technical Accuracy: **5/5**
* Clarity: **4/5**
* Total Score: **19/20**

## Observation

Chain-of-thought style prompting is useful for complex problems because it encourages a structured and step-by-step solution.

---

# 5. PERSONA PATTERN

## Definition

Persona prompting assigns a specific **role or professional identity** to the AI.

This allows the AI to generate a response from the perspective of a particular expert.

## Prompt

```text
Act as an experienced Industrial IoT Engineer specializing in smart manufacturing and predictive maintenance.

Design an IoT-based predictive-maintenance solution for an automotive manufacturing plant.

Explain the sensors required, embedded controller, communication technology, cloud platform, AI/ML model, monitoring dashboard, alerts, and maintenance process.

Also explain how the solution can improve production efficiency by 30%, reduce downtime, and optimize energy consumption.

Give the answer as a professional engineering proposal.
```

## Generated Response

As an Industrial IoT Engineer, the proposed smart manufacturing system can be divided into several layers.

### 1. Sensor Layer

Sensors collect machine parameters such as:

* Temperature
* Vibration
* Pressure
* Current
* Energy consumption

These sensors provide real-time information about the machine condition.

### 2. Embedded Controller Layer

An embedded controller receives data from the sensors.

It performs basic processing and sends the required information to the communication gateway.

### 3. Communication Layer

Communication technologies and protocols such as MQTT can be used to transfer machine data to the cloud or industrial server.

### 4. Cloud Layer

The cloud platform stores and processes machine data.

It provides scalability and enables remote monitoring.

### 5. AI/ML Layer

AI and machine-learning models analyze historical and real-time machine data.

The model can identify abnormal behavior and predict possible machine failures.

### 6. Monitoring Layer

A dashboard displays:

* Machine health
* Machine status
* Temperature
* Vibration
* Energy consumption
* Maintenance alerts

### 7. Maintenance Layer

When a possible failure is predicted, the maintenance team receives an alert.

The team can perform maintenance before the machine experiences a major failure.

## Evaluation

* Professional Perspective: **5/5**
* Technical Accuracy: **5/5**
* Completeness: **5/5**
* Practicality: **5/5**
* Total Score: **20/20**

## Observation

Persona prompting produces more professional and domain-specific responses because the AI is instructed to behave like an expert.

---

# 6. REVERSE PROMPTING

## Definition

Reverse prompting starts with a **desired output** and asks the AI to identify the necessary requirements and construct an optimized prompt.

It is useful when the user knows what output is required but is not sure how to write an effective prompt.

## Prompt

```text
I want to create an AI-generated solution for an IoT-based predictive maintenance system in a smart manufacturing plant.

The final response should include system architecture, sensors, embedded controller, communication, cloud platform, AI/ML model, real-time monitoring, failure prediction, alerts, energy optimization, and expected benefits.

First, determine what information a high-quality prompt should contain.

Then create an optimized prompt that can be used to generate this complete solution.
```

## Generated Response

The AI identifies the following important requirements:

* Manufacturing environment
* Machine parameters
* IoT sensors
* Embedded controller
* Communication protocol
* Cloud infrastructure
* Data processing
* AI/ML prediction
* Monitoring dashboard
* Maintenance alerts
* Energy optimization
* Performance objectives
* Required output format

## Optimized Prompt Generated by AI

```text
Act as an Industrial IoT and AI expert.

Design a complete IoT-based predictive maintenance system for a smart manufacturing plant.

Include system architecture, sensors, embedded controller, communication protocols, cloud infrastructure, data processing, AI/ML model, real-time dashboard, failure prediction, alert mechanism, remote monitoring, and energy optimization.

Explain the working process step by step and describe how the solution can reduce downtime, improve production efficiency, and reduce energy consumption.

Present the solution in a structured engineering format.
```

## Evaluation

* Requirement Identification: **5/5**
* Prompt Quality: **5/5**
* Completeness: **5/5**
* Clarity: **5/5**
* Total Score: **20/20**

## Observation

Reverse prompting helps users create better prompts by first identifying the requirements of the desired output.

---

# 7. GRAPH PROMPTING

## Definition

Graph prompting represents information using **nodes and relationships**.

It is useful for representing system architecture, relationships between components, and data flow.

## Prompt

```text
Represent an IoT-based predictive maintenance system for smart manufacturing as a graph.

Use nodes for:

Sensors,
Embedded Controller,
Gateway,
Cloud Platform,
Database,
AI/ML Model,
Monitoring Dashboard,
Alert System,
Maintenance Team,
and Machine.

Show the relationships and direction of data flow between the nodes.

After creating the graph structure, explain the function of each node.
```

## Generated Graph

```text
                    +----------------------+
                    | Manufacturing       |
                    | Machine             |
                    +----------+-----------+
                               |
                               v
                    +----------------------+
                    | IoT Sensors          |
                    | Temperature          |
                    | Vibration            |
                    | Pressure             |
                    | Current              |
                    +----------+-----------+
                               |
                               v
                    +----------------------+
                    | Embedded Controller  |
                    +----------+-----------+
                               |
                               v
                    +----------------------+
                    | IoT Gateway          |
                    +----------+-----------+
                               |
                               v
                    +----------------------+
                    | Cloud Platform        |
                    +----------+-----------+
                               |
                    +----------+----------+
                    |                     |
                    v                     v
          +----------------+    +----------------+
          | Database       |    | AI / ML Model  |
          +----------------+    +-------+--------+
                                        |
                                        v
                              +-------------------+
                              | Monitoring        |
                              | Dashboard         |
                              +---------+---------+
                                        |
                                        v
                              +-------------------+
                              | Alert System      |
                              +---------+---------+
                                        |
                                        v
                              +-------------------+
                              | Maintenance Team  |
                              +-------------------+
```

## Component Explanation

### Machine

The manufacturing machine is the equipment being monitored.

### IoT Sensors

Sensors collect real-time machine parameters such as temperature, vibration, pressure, and current.

### Embedded Controller

The controller receives sensor data and performs initial processing.

### IoT Gateway

The gateway transfers processed data from the local manufacturing environment to the cloud platform.

### Cloud Platform

The cloud platform stores and processes large amounts of machine data.

### Database

The database stores historical and real-time machine information.

### AI/ML Model

The AI/ML model analyzes machine data and predicts possible failures.

### Monitoring Dashboard

The dashboard displays machine status, sensor values, machine health, and energy consumption.

### Alert System

The alert system notifies the maintenance team when abnormal conditions or possible failures are detected.

### Maintenance Team

The maintenance team takes corrective action based on the alerts generated by the system.

## Evaluation

* Graph Structure: **5/5**
* Data Flow Representation: **5/5**
* Completeness: **5/5**
* Clarity: **5/5**
* Total Score: **20/20**

## Observation

Graph prompting is highly useful for representing complex systems because it clearly shows the relationship and flow between different components.

---

# 8. ACTIVE PROMPTING

## Definition

Active prompting allows the AI to **ask questions and collect missing information** before generating the final solution.

This is useful when the initial requirements are incomplete.

## Prompt

```text
You are designing an IoT-based predictive maintenance system for a manufacturing plant.

Before providing the final design, actively identify the missing information required to make the solution accurate.

Ask me up to 5 important questions about:

1. Machine type
2. Sensor parameters
3. Communication technology
4. Cloud requirements
5. Maintenance objectives

After receiving the answers, generate the final system design.
```

## Generated Interaction

### Question 1

**AI:** What type of manufacturing machine needs to be monitored?

**User:** CNC machines.

### Question 2

**AI:** Which parameters should be monitored?

**User:** Temperature, vibration, current, and energy consumption.

### Question 3

**AI:** Is cloud-based monitoring required?

**User:** Yes.

### Question 4

**AI:** Should remote control be supported?

**User:** Yes.

### Question 5

**AI:** What is the main maintenance objective?

**User:** Predict machine failures before they cause downtime.

## Final Generated Solution

Based on the collected requirements, an IoT-based predictive maintenance system can be designed specifically for CNC machines.

The system includes:

* Temperature sensors
* Vibration sensors
* Current sensors
* Energy monitoring
* Embedded controller
* IoT gateway
* Cloud platform
* AI/ML failure prediction
* Real-time monitoring dashboard
* Maintenance alerts
* Remote monitoring and control

The collected sensor data is analyzed using AI/ML techniques to identify abnormal conditions and predict possible failures.

## Evaluation

* Requirement Gathering: **5/5**
* Relevance: **5/5**
* Accuracy: **5/5**
* Adaptability: **5/5**
* Total Score: **20/20**

## Observation

Active prompting improves the quality of the final solution by collecting important information before generating the response.

---

# 9. RUBRIC-BASED EVALUATION

The generated responses are evaluated using the **Rubric Method**.

The following criteria are used:

### 1. Relevance

Measures how well the generated response addresses the given problem and use case.

### 2. Technical Accuracy

Measures whether the technical information provided by the AI is correct.

### 3. Completeness

Measures whether all important requirements of the use case are covered.

### 4. Clarity

Measures how easily the generated response can be understood.

### 5. Practicality

Measures whether the generated solution can be useful in a real-world manufacturing environment.

## Scoring Scale

```text
5 – Excellent
4 – Very Good
3 – Good
2 – Needs Improvement
1 – Poor
```

---

# 10. OVERALL EVALUATION

## Zero-Shot Prompting

**Score: 18/20**

The response was relevant and easy to understand, but it provided less detailed information compared with more structured prompting techniques.

## Few-Shot Prompting

**Score: 20/20**

The examples helped the AI understand the expected response format and produce a consistent result.

## Chain-of-Thought Prompting

**Score: 19/20**

The prompt produced a logical and systematic approach for analyzing machine abnormalities.

## Persona Pattern

**Score: 20/20**

The AI generated a professional engineering response by taking the role of an Industrial IoT Engineer.

## Reverse Prompting

**Score: 20/20**

The AI successfully identified the requirements and generated an optimized prompt for producing the desired solution.

## Graph Prompting

**Score: 20/20**

The graph clearly represented the relationship and data flow between the components of the IoT system.

## Active Prompting

**Score: 20/20**

The AI collected missing requirements before generating the final solution, resulting in a more customized design.

---

# 11. COMPARISON OF DIFFERENT AI TOOLS

The same prompts can be executed using different AI tools such as:

* ChatGPT
* Google Gemini
* Microsoft Copilot

The generated responses can be evaluated using the same rubric.

## ChatGPT

ChatGPT generated structured and detailed responses for the IoT-based predictive maintenance use case. It performed particularly well for persona, few-shot, reverse, graph, and active prompting.

## Google Gemini

Gemini was able to understand the prompts and generate technically relevant responses. It also produced structured explanations for the manufacturing use case.

## Microsoft Copilot

Copilot generated relevant responses and provided useful technical explanations for the given scenario.

> **Note:** The following scores are sample evaluation values. Actual scores may vary depending on the AI model, prompt version, and evaluation process.

### ChatGPT

```text
Zero-Shot Prompting       : 18/20
Few-Shot Prompting        : 20/20
Chain-of-Thought          : 19/20
Persona Pattern           : 20/20
Reverse Prompting         : 20/20
Graph Prompting           : 20/20
Active Prompting          : 20/20
```

### Google Gemini

```text
Zero-Shot Prompting       : 18/20
Few-Shot Prompting        : 19/20
Chain-of-Thought          : 19/20
Persona Pattern           : 19/20
Reverse Prompting         : 19/20
Graph Prompting           : 19/20
Active Prompting          : 19/20
```

### Microsoft Copilot

```text
Zero-Shot Prompting       : 17/20
Few-Shot Prompting        : 18/20
Chain-of-Thought          : 18/20
Persona Pattern           : 19/20
Reverse Prompting         : 18/20
Graph Prompting           : 18/20
Active Prompting          : 19/20
```

---

# 12. COMPARISON OF PROMPT PATTERNS

### Zero-Shot Prompting

Used when a direct answer is required without examples.

### Few-Shot Prompting

Used when examples are available and the AI needs to follow a particular pattern.

### Chain-of-Thought Prompting

Used for complex problems that require systematic analysis.

### Persona Pattern

Used when an expert or specific professional perspective is required.

### Reverse Prompting

Used to create an effective prompt from a desired output.

### Graph Prompting

Used to represent relationships, dependencies, and data flow.

### Active Prompting

Used when additional information is required before generating the final answer.

---

# 13. KEY FINDINGS

The experiment produced the following observations:

1. Prompt structure has a significant impact on AI-generated output.
2. Zero-shot prompting is simple and suitable for general questions.
3. Few-shot prompting improves consistency by providing examples.
4. Chain-of-thought prompting is useful for complex problem-solving tasks.
5. Persona prompting provides domain-specific and professional responses.
6. Reverse prompting helps users create optimized prompts.
7. Graph prompting is useful for system architecture and relationship representation.
8. Active prompting helps identify missing requirements.
9. Different AI tools may generate different responses for the same prompt.
10. Rubric-based evaluation provides a systematic way to compare AI-generated responses.

---

# 14. CONCLUSION

The different prompt engineering patterns, namely **Zero-Shot Prompting, Few-Shot Prompting, Chain-of-Thought Prompting, Persona Pattern, Reverse Prompting, Graph Prompting, and Active Prompting**, were successfully designed and evaluated for the **IoT-Based Smart Manufacturing and Predictive Maintenance** use case.

The experiment demonstrates that the quality of an AI-generated response depends significantly on the type and structure of the prompt.

Simple prompts such as zero-shot prompting are useful for direct questions, while few-shot, persona, reverse, graph, and active prompting can provide more structured and context-specific results.

The generated responses were evaluated using a **Rubric-based evaluation method** based on relevance, technical accuracy, completeness, clarity, and practicality.

Thus, prompt engineering techniques can be effectively used to improve the quality, reliability, and usefulness of AI-generated solutions for real-world industrial applications.

---

# RESULT

The required prompts for **Zero-Shot, Few-Shot, Chain-of-Thought, Persona, Reverse, Graph, and Active Prompting** were successfully created and evaluated.

The prompts were applied to the **IoT-based Smart Manufacturing and Predictive Maintenance** use case, and the generated outputs were compared using a **Rubric-based evaluation method**.

**Hence, the experiment was successfully completed.**
