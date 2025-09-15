# MODULE-V: PROJECT MANAGEMENT

## 1. Software Project Management

Software Project Management is the application of knowledge, skills, tools, and techniques to software project activities to meet the project requirements. It involves balancing the competing constraints of scope, time, cost, and quality.

## 2. Estimation

Software cost estimation is a crucial activity in project management. An accurate estimation is essential for proper project planning and budgeting.

### LOC (Lines of Code) Based Estimation
*   A size-oriented metric that uses the number of lines of code as the primary input for estimation.
*   **Process:**
    1.  Estimate the size of the software in thousands of Lines of Code (KLOC).
    2.  Use historical data to calculate productivity (e.g., KLOC per person-month).
    3.  Calculate the effort (Person-Months) = Total KLOC / Productivity.
    4.  Calculate the cost = Effort * Cost per person-month.
*   **Pros:** Simple and easy to use.
*   **Cons:** Highly dependent on the programming language and coding style. It is difficult to estimate LOC accurately in the early stages of a project.

### FP (Function Point) Based Estimation
*   A function-oriented metric that measures the functionality of the software from the user's point of view.
*   **Process:**
    1.  Count the number of function points:
        *   **External Inputs (EIs):** Data going into the system.
        *   **External Outputs (EOs):** Data coming out of the system.
        *   **External Inquiries (EQs):** Requests for information from the system.
        *   **Internal Logical Files (ILFs):** Data stored within the system.
        *   **External Interface Files (EIFs):** Data shared with other systems.
    2.  Assign a complexity (low, average, high) to each function point.
    3.  Calculate the Unadjusted Function Point (UFP) count.
    4.  Calculate the Value Adjustment Factor (VAF) based on 14 General System Characteristics (GSCs) like performance, usability, and reusability.
    5.  Calculate the final Function Point (FP) count = UFP * VAF.
    6.  Use historical data to convert FP to effort.
*   **Pros:** Independent of the programming language. Can be estimated from the requirements.
*   **Cons:** The process can be subjective and time-consuming.

### Make/Buy Decision
*   A strategic decision that organizations face when they need a new software system.
*   **Factors to consider:**
    *   **Cost:** Is it cheaper to build or buy?
    *   **Time:** Can we build it in time, or is a COTS solution faster?
    *   **Expertise:** Do we have the in-house expertise to build it?
    *   **Customization:** How much customization does the COTS solution require?
    *   **Competitive Advantage:** Will a custom-built solution provide a competitive advantage?

### COCOMO I & II Model (Constructive Cost Model)
*   An algorithmic cost estimation model.
*   **COCOMO I:**
    *   **Basic:** A simple model for a quick, rough estimate.
    *   **Intermediate:** Considers 15 cost drivers (e.g., required reliability, database size, personnel capability).
    *   **Detailed:** A more detailed model that considers the cost drivers for each phase of the project.
*   **COCOMO II:**
    *   An updated version of COCOMO that is better suited for modern software development practices.
    *   It includes models for different stages of the project:
        *   **Application Composition:** For projects built using existing components.
        *   **Early Design:** For early-stage estimation before the architecture is finalized.
        *   **Post-Architecture:** For estimation after the architecture has been designed.

## 3. Project Scheduling

Project scheduling is the process of allocating resources and sequencing tasks to complete a project within a given timeframe.

### Scheduling
*   **Work Breakdown Structure (WBS):** A hierarchical decomposition of the total scope of work to be carried out by the project team.
*   **Tools:**
    *   **Gantt Charts:** A bar chart that illustrates the project schedule. It shows the start and finish dates of the terminal elements and summary elements of a project.
    *   **PERT (Program Evaluation and Review Technique) Charts:** A network diagram that shows the dependencies between tasks. It is used to identify the critical path (the longest sequence of tasks that must be completed on time for the project to be completed on schedule).

### Earned Value Analysis (EVA)
*   A powerful technique for tracking project performance.
*   **Key Metrics:**
    *   **Planned Value (PV):** The budgeted cost for the work scheduled to be completed.
    *   **Earned Value (EV):** The value of the work actually completed.
    *   **Actual Cost (AC):** The actual cost incurred for the work completed.
    *   **Schedule Variance (SV) = EV - PV:** A positive SV means the project is ahead of schedule.
    *   **Cost Variance (CV) = EV - AC:** A positive CV means the project is under budget.
    *   **Schedule Performance Index (SPI) = EV / PV:** An SPI > 1 means the project is ahead of schedule.
    *   **Cost Performance Index (CPI) = EV / AC:** A CPI > 1 means the project is under budget.

## 4. Planning

### Project Plan
*   A comprehensive document that defines the project's objectives, scope, schedule, budget, and resources. It serves as a roadmap for the project.

### Planning Process
1.  **Scope Planning:** Defining what is and is not included in the project.
2.  **Resource Planning:** Identifying the people, equipment, and materials needed.
3.  **Cost Planning:** Estimating the cost and setting the budget.
4.  **Schedule Planning:** Defining the tasks, dependencies, and timeline.
5.  **Risk Planning:** Identifying potential risks and planning how to respond to them.
6.  **Quality Planning:** Defining the quality standards and how they will be met.
7.  **Communication Planning:** Defining how information will be communicated to stakeholders.

### RFP (Request for Proposal)
*   A document used to solicit proposals from potential vendors for a product or service. It typically includes a description of the project, the requirements, and the evaluation criteria.

## 5. Risk Management

Risk management is the process of identifying, assessing, and mitigating risks to minimize their impact on the project.

### Risk Identification
*   The process of identifying potential risks.
*   **Techniques:** Brainstorming, checklists, interviews, SWOT analysis.

### Risk Projection (Risk Analysis)
*   The process of assessing the probability and impact of each identified risk.
*   **Risk Exposure = Probability * Impact**

### RMMM Plan (Risk Mitigation, Monitoring, and Management Plan)
*   A plan for how to deal with risks.
*   **Mitigation:** Taking steps to reduce the probability or impact of a risk (e.g., using a more reliable technology).
*   **Monitoring:** Continuously monitoring the identified risks and looking for new ones.
*   **Management (Contingency Planning):** Developing a plan for what to do if a risk occurs (e.g., having a backup server).

```mermaid
graph TD
    A[Risk Identification] --> B[Risk Projection (Analysis)];
    B --> C[RMMM Plan];
```

## 6. CASE TOOLS (Computer-Aided Software Engineering)

CASE tools are software applications that are used to support and automate software development activities.

### Types of CASE Tools:
*   **Upper CASE:** Tools that support the early phases of the SDLC (requirements analysis, design).
*   **Lower CASE:** Tools that support the later phases (coding, testing, maintenance).
*   **Integrated CASE:** Tools that support the entire SDLC.

### Examples:
*   **Diagramming tools:** Microsoft Visio, Lucidchart.
*   **Code generators:** Tools that can generate code from UML diagrams.
*   **Testing tools:** Selenium, JUnit.
*   **Project management tools:** Jira, Trello, Microsoft Project.