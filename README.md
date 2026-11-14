AI Lead Scoring for a B2B CRM: Business Analysis Case Study
A business analysis portfolio project that defines how an AI feature can score and label sales leads inside a B2B CRM (working product name: LeadFlow CRM). The project covers the full analysis chain: business requirements, functional requirements with user stories, an AI scoring specification, a sample dataset, a Power BI dashboard and a Jira backlog.
> **Note:** All data in this repository is synthetic and created for demonstration only. Scoring points and thresholds are default values that would be validated with real sales data in a live project.
Problem
Sales teams in B2B companies have no objective way to identify which leads are most likely to convert. Leads are prioritised by judgement, which delays contact with high-intent leads and wastes effort on low-intent ones.
Solution in brief
The AI scores every lead from 0 to 100 in the background and assigns a Hot, Warm or Cold label.
Scoring combines structured rules (lead source, company size, activity) with analysis of the lead's enquiry message.
Each score shows its main reasons (up to three factors), so sales executives can trust it.
The AI never contacts a lead. All customer communication stays with the sales team.
Sales Managers can configure thresholds and points. Sales Executives can override a label with a recorded reason.
Deliverables
#	Deliverable	Description
1	Business Requirements Document	Problem, objectives, scope, business requirements and success measures
2	Functional Requirements Document and User Stories	Functional requirements, business rules and 11 user stories with acceptance criteria
3	AI Scoring Specification	Signals, points, scoring formula, explanation output, guardrails and edge cases
4	Dataset and Excel dashboard	200 synthetic leads with formula-driven scores and labels, plus an Assumptions sheet
5	Power BI dashboard (PDF)	Conversion and response-time reporting by label and by lead source
6	Jira backlog screenshots	5 epics and 13 user stories with traceability to functional requirements
Scoring model (default values)
Signal	Points
Lead requested a quotation or demo	+30
Message states quantity, budget or deadline	+20
Lead answered a call or replied to an email	+15
Lead visited the website more than once	+10
Company size in the target range	+10
Lead came from a high-converting source	+10
No response for 7 days	-15
The score is limited to the range 0 to 100. Default labels: Hot 60 to 100, Warm 30 to 59, Cold 0 to 29.
Dashboard results (synthetic data)
Label	Leads	Conversion rate	Avg. days to first contact
Hot	45	35.6%	1.1
Warm	67	7.5%	2.4
Cold	88	0.0%	6.1
Overall conversion across 200 leads is 10.5%. By source, Referral (17.4%), Trade Show (14.3%) and IndiaMART (14.0%) convert best in this sample, and Cold Call converts lowest (6.5%). These figures are illustrative, since the outcomes were generated to show how the dashboard would read.
Product backlog
The 13 user stories are grouped into 5 epics in Jira:
Lead Scoring and Labelling
Lead Prioritisation (Executive)
Scoring Configuration (Manager)
Reporting and Insights
Security, Privacy and AI Guardrails
Backlog refinement identified requirements without a user story. These were added as stories and linked to their functional requirements, keeping the chain from business objective to business requirement, functional requirement and user story complete.
Skills demonstrated
Business and functional requirements documentation (BRD, FRD)
User stories with Given/When/Then acceptance criteria
Requirements traceability from objectives to user stories
Specifying an AI feature, including explainability, human override and guardrails
Data modelling and formula-driven analysis in Excel
Dashboard design in Power BI
Backlog management in Jira
Repository structure
```
docs/        BRD, FRD with user stories, AI scoring specification (PDF)
data/        Synthetic dataset and Excel workbook, CSV used for Power BI
dashboard/   Power BI dashboard export
jira/        Backlog screenshots
```
Limitations
The dataset is synthetic, so conversion figures do not represent real sales performance.
Points, thresholds, high-converting sources and target company sizes are assumptions to be validated with real data.
This is an analysis and specification project. No AI model was built or trained.
Author
Snehal Mishra
