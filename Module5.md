# MODULE-V: PROJECT MANAGEMENT

## 1. Software Project Management

Software Project Management is the art and science of planning and leading software projects. It is a sub-discipline of project management in which software projects are planned, implemented, monitored and controlled.

## 2. Estimation

Software cost estimation is the process of predicting the amount of effort required to build a software system.

### LOC (Lines of Code) Based Estimation
*   A simple model that uses the projected number of lines of code in the finished product to estimate the cost and effort.
*   **Process:**
    1.  Estimate the size of the software in Lines of Code (LOC).
    2.  Use historical data to calculate the productivity (LOC per person-month).
    3.  Calculate the effort (Person-Months) = Total LOC / Productivity.
*   **Pros:** Simple to use.
*   **Cons:** Difficult to estimate LOC accurately in the early stages, language dependent.

### FP (Function Point) Based Estimation
*   A method of measuring the size of a software application by the functions it delivers to the user. It is independent of the programming language used.
*   **Process:**
    1.  Count the number of function points (e.g., inputs, outputs, inquiries, files).
    2.  Apply complexity adjustment factors.
    3.  Calculate the Function Points (FP).
    4.  Use historical data to convert FP to effort.
*   **Pros:** Language independent, can be estimated from requirements.
*   **Cons:** Subjective counting of function points.

### Make/Buy Decision
*   The decision of whether to build a software system from scratch, buy a commercial off-the-shelf (COTS) product, or outsource the development.
*   **Factors to consider:** Cost, time to market, availability of expertise, strategic importance.

### COCOMO I & II Model (Constructive Cost Model)
*   An algorithmic software cost estimation model developed by Barry Boehm.
*   **COCOMO I:**
    *   Has three models: Basic, Intermediate, and Detailed.
    *   **Basic:** A static, single-valued model that computes software development effort (and cost) as a function of program size expressed in estimated lines of code (LOC).
    *   **Intermediate:** Computes software development effort as a function of program size and a set of "cost drivers" that include subjective assessments of product, hardware, personnel and project attributes.
    *   **Detailed:** Incorporates all characteristics of the intermediate version with an assessment of the cost driver's impact on each step (analysis, design, etc.) of the software engineering process.
*   **COCOMO II:**
    *   A more comprehensive model that can be applied to modern software development processes.
    *   It is a suite of three models: Application Composition, Early Design, and Post-Architecture.

## 3. Project Scheduling

Project scheduling is the process of defining project activities, sequencing them in a logical order, and assigning resources to them.

### Scheduling
*   The process of creating a project schedule, which is a timeline that shows when each activity should start and end.
*   **Tools:** Gantt charts, PERT charts.

### Earned Value Analysis (EVA)
*   A project management technique for measuring project performance and progress in an objective manner.
*   It combines measures of scope, schedule, and cost in a single integrated system.
*   **Key Metrics:**
    *   **Planned Value (PV):** The budgeted cost of work scheduled.
    *   **Earned Value (EV):** The budgeted cost of work performed.
    *   **Actual Cost (AC):** The actual cost of work performed.
    *   **Schedule Variance (SV) = EV - PV**
    *   **Cost Variance (CV) = EV - AC**

## 4. Planning

### Project Plan
*   A formal, approved document that is used to guide both project execution and project control.
*   The primary uses of the project plan are to document planning assumptions and decisions, facilitate communication among stakeholders, and document approved scope, cost, and schedule baselines.

### Planning Process
1.  **Scope Planning:** Defining the project scope.
2.  **Resource Planning:** Determining what resources (people, equipment, materials) are needed.
3.  **Cost Planning:** Estimating the cost of the project.
4.  **Schedule Planning:** Developing the project schedule.
5.  **Risk Planning:** Identifying and planning for potential risks.
6.  **Quality Planning:** Identifying which quality standards are relevant to the project and determining how to satisfy them.
7.  **Communication Planning:** Determining the information and communication needs of the stakeholders.

### RFP (Request for Proposal)
*   A document that solicits proposals, often made through a bidding process, by an agency or company interested in procurement of a commodity, service, or valuable asset, to potential suppliers to submit business proposals.

## 5. Risk Management

Risk management is the process of identifying, assessing, and controlling threats to an organization's capital and earnings.

### Risk Identification
*   The process of determining risks that could potentially prevent the program, enterprise, or investment from achieving its objectives.
*   **Techniques:** Brainstorming, checklists, interviews.

### Risk Projection (Risk Analysis)
*   The process of assessing the likelihood and impact of identified risks.
*   **Risk = Probability of Occurrence * Impact**

### RMMM Plan (Risk Mitigation, Monitoring, and Management Plan)
*   A document that outlines how the project team will manage and mitigate risks.
*   **Mitigation:** Taking steps to reduce the probability or impact of a risk.
*   **Monitoring:** Tracking the identified risks and looking for new ones.
*   **Management:** Developing contingency plans for risks that occur.

```mermaid
graph TD
    A[Risk Identification] --> B[Risk Projection (Analysis)];
    B --> C[RMMM Plan];
```

## 6. CASE TOOLS (Computer-Aided Software Engineering)

CASE tools are software to support software development and evolution processes.

### Types of CASE Tools:
*   **Upper CASE (Front-end tools):** Used in the early stages of development (planning, analysis, design).
*   **Lower CASE (Back-end tools):** Used in the later stages (implementation, testing, maintenance).
*   **Integrated CASE (I-CASE):** Provide support for the full life cycle.

### Examples:
*   **Diagramming tools:** For creating DFDs, UML diagrams, etc.
*   **Code generators:** For automatically generating code from design models.
*   **Testing tools:** For automating the testing process.
*   **Project management tools:** For planning and tracking projects.