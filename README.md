# LLMReasoningPersonalHealthData
Repository for the paper "Exploring Large Language Model Reasoning Capabilities Over Personal Health Data"

## Folder Structure

This repository contains the following folders:

### 1) `Prompt`
The `Prompt` folder contains the prompt for the large language model (LLM). The prompt is divided into three parts:

- **Task**: The specific task that the LLM is being asked to perform.
- **Structured Background Knowledge**: Relevant structured background knowledge in TURTLE language that is provided to the LLM to assist with accurate reasoning. This includes: **Monitoring Rule** and **Violation**.
- **Structured Input Data**: The description of the PatientX use case encoded in TURTLE.

### 2) `Results`
The `Results` folder contains the result file for the following tasks:

#### 2.1 Reason and Decide
This task involves determining if a violation has occurred based on the provided health data. The LLM has to provide a simple YES/NO answer, showing the reasoning behind its decision.

#### 2.2 Generate Two Explanations
For this task, the LLM generates two types of explanations based on the decision made:

- **Detailed Explanation for the User**: A simple and comprehensible explanation for the patient. The goal is to make the reasoning clear and accessible.

- **Detailed Explanation for the Physician**: A more technical explanation tailored to medical professionals, providing precise terminology and a detailed rationale for the decision.

### NOTE 
- Structured Knowledge is taken from the [FuS-KG GitHub repository](https://github.com/IDA-FBK/FuS-KG). Please, refer to the repo for further details.
- **Monitoring rule** and **Violation** descriptions can be found in the [Guidelines](https://github.com/IDA-FBK/FuS-KG/blob/main/ontology/TBox/fuskg-guidelines.ttl) and [User](https://github.com/IDA-FBK/FuS-KG/blob/main/ontology/TBox/fuskg-user.ttl) modules of FuS-KG.

## Authors
- Gianluca Apriceno: apriceno@fbk.eu
- Tania Bailoni: tbailoni@fbk.eu
- Mauro Dragoni: dragoni@fbk.eu
