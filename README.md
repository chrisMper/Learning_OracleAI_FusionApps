# OracleAI_FusionApps
Notes for the course Oracle AI Agent Studio for Fusion Applications offered by Oracle University

## Getting Started with Fusion AI Agent Studio

### Introduction: Fusion AI Agent Studio
- AI agents are built-in
- LLMs Included
- Real-time execution

### AI in Oracle Fusion Application
- AI is Built-in to OCI (Oracle Cloud Infrastructure)
- Hence OCI has AI Database + AI data platform
- Oracle applications include AI Assistants, AI Agents, AI Agent Teams, AI workflow Agents

### Core Concepts of Fusion AI Agents

- Task automation : Powered by LLMs Decides, Plans and acts and call other tools as well
- They can act as an Author, they can answer, they can do actions
- Usage as an Author : Job posting, Email Handling, sales order Acknowledgement etc...
- Usage as an Answer : Payslip agent, Customer chat Agents, Claims Agent
- Usage as an Actor : Shift Scheduling agent, Accounts engagement agent etc...
- Oracle Agent Studio enables you to build agents
- We can expand and customize available agent templates in the Agent studio
- Example of an agent Team  <img width="1365" height="767" alt="image" src="https://github.com/user-attachments/assets/a3cc4d28-03c2-4f74-9f34-e156aa1e7d06" />
- Each Agent has system prompts and topics which we can define and customize instructions
- AI Agent Studio Tools : Document tool, Business Object tool, Email Tool, Deep Link Tool, External Rest tool, User Session tool, Calculator tool
- It also Enables Human-in-the-loop
- AI Agent studio Enables Quality Evaluation of the agent as well
- The roadmap of 'Deployment' : Agent Studio > Agent Platform > End User Experience > Monitoring and Evaluation
-  Embedded and Custom AI <img width="1365" height="767" alt="image" src="https://github.com/user-attachments/assets/9724b028-6fa2-4572-adf5-75fcc6c91129" />

## AI Agent Studio: Tools, Configurations and Demo

### Tool Configuration and Usage
- Best Practices : Clear precise Tool Descriptions, Use Human-in-the-loop Thoughtfully, Limit exposed fields in business objects, Validate inputs, etc...
#### What is a BUSINESS OBJECT?
- It connects AI Agent and Fusion app : AI Agent > Business Object > Fusion API
- It specifies the functions that the Agent can do
- Example : Service Request Object : Get all service requests, Create new service request, Find request by SRNumber, Add message to a service request...

### Oracle AI Agent Studio: Deep Dive into Tools

- Examples for published agents <img width="1365" height="702" alt="image" src="https://github.com/user-attachments/assets/30c7607d-79e4-4495-991f-bdddedb02d2e" />
- Example for Business Object which has Tool code, family, product, description, human approval and its functions <img width="1365" height="767" alt="image" src="https://github.com/user-attachments/assets/707c9b46-a45d-4a16-9c0a-d93a554d0af9" />

#### Creating a Business Object

- When creating a business object you must observe the 'REST API for Oracle Fusion Cloud HCM', it has the documentations for the Endpoints
- Step 1 : Add new business Object
- Step 2 : Pick a Family > pick a product > Give a name > Then a code will be Generated > Give a resource type > Give the resource path (the endpoint of the REST API)
- Step 3 : Add Business object functions : Click on 'Add from Specifications' > it opens a popup 'Select an operation' with the relevant endpoint >  in the dropdown there select a child object > it directs to a scenario
- <img width="1365" height="767" alt="Creating a New Business Object" src="https://github.com/user-attachments/assets/cff700b5-34fc-48b6-b572-163f0068c18d" />
- Step 4 : Add a new Scenario : it has a name,  description, operation type and resource path, headers, Parameters and Business Object Fields, examples Usages
- Step 5 : Under Parameters and business object Fields we can Add Fields from Specification > it gives a set of business object Fields to select <img width="1365" height="767" alt="Adding Fields from specification" src="https://github.com/user-attachments/assets/3967c3a2-5c5a-4132-8dd5-25df0b65a145" />
- Step 6 : Add business object tool : Give a Tool type, Tool Name, tool code, family and product > Add a business object
- Step 7 : Add a new Agent : Give an Agent name, Agent code, family, product, maximum interactions, Description, prompt <img width="1365" height="767" alt="Creating a New Agent" src="https://github.com/user-attachments/assets/8f9f7cf0-df43-4ec4-947b-91c9a5f24d41" />
- Step 8 : Then we will be directed to the Agent definition which has tools and Topics. > add tools and business objects to the tools section > add a topic 
- Step 9 : Add/edit agent team ( agent team is the work flow to perform a set of tasks) > and test

## Building Workflow Agents

### Agentic Patterns - Understanding Workflow Agents

|              | Workflow Agents | Hierarchical Agents |
|Execution Model| Policy-bound orchestration with contextual reasoning | LLM-led decomposition with delegated specialists|
|Optimized for | Predictability, auditability, SLA stability | Discovery, planning, synthesis under uncertainity|
|Best fit | Structured processes where rules/policies are known and outcomes must repeat | Ambiguous problems with many possible paths and evolving goals |
| Strengths | End-to-end steps, approvals, retries, state management, traceability |
| Primary goal | Consistent, compliant outcomes at scale | Find the right plan/ answer under uncertainity|

- Static rule-based workflow engines can execute sequences, but,
  - Can't reason or infer from context
  - Can't Adapt to changing state/ new facts
  - Can't Handle ambiguity without human intervention
  - Can't learn from what happens inside the process

- Workflow AGENTS Enable,
  - Dynamic Path selection
  - Contextual decision-making
  - Multi-turn reasoning
  - Parallel branching
  - Multi agent Collaboration
  - Self-correction when inputs are missing, inconsistent or fail

### Designing Workflow Agents

<img width="1365" height="767" alt="steps-decisions-key Questions" src="https://github.com/user-attachments/assets/7bdc9e0d-ef7a-4ba0-b049-55b188d5f3bc" />

### Workflow Agents : Building Blocks

- There are nodes as building blocks
<img width="1365" height="767" alt="Different types of nodes" src="https://github.com/user-attachments/assets/926299a3-629e-4e73-a64c-3e0f088bf49b" />

## Security and Governance

### Security Concepts
- Enable Role/user based and Pillar (CX, ERP, HCM, SCM) based access

### Security Configurations
- 






