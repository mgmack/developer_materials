# developer_materials

Code Commits, Reviews and Merging
When do I need my code reviewed?
All code must be reviewed prior to being merged into develop or master. This is done through a "Pull Request" initiated by the developer in Bitbucket or Github.

What are the code standards?
Mediacurrent JS standards: https://bitbucket.org/mediacurrent/mis_js_standard 
Mediacurrent CSS standards: https://bitbucket.org/mediacurrent/mis_css_standard 
Drupal coding standards: https://www.drupal.org/docs/develop/standards/coding-standards 
Drupal comment standards: https://www.drupal.org/node/1354 
Who is a code reviewer?
Everyone can review PR's once they have reviewed best practices in this document.

Who will review my code?
All code must be reviewed by at least one team member (not involved in code in the PR) before the feature branch is merged into develop.

The preferred order of reviewers:

A member of the project team
How long should a PR review take?
Most should be under 15 minutes.

Code Review Workflow:
(NOTE: See Version Control handbook for guidance on branch naming conventions).

Make sure your feature branch is feature complete.
Push the feature branch to the remote repo.
Review the Bitbucket Pipeline
Create a pull request and assign it to all team members.
The reviewer will review your code and either a) mark issues/questions in the PR and reject b) approve it.
Make the corrections in your branch, push those changes back up again and create a new pull request (or just go back to #2).
Respond to PR comments to respond to the comment.
Once the reviewer has approved your code a project lead will merge the code into the develop branch and remove your remote feature branch (unless it lives in a forked repo).
Note: Not all projects are currently on Bitbucket. If your project is one of these, please follow the steps but instead of creating a pull request please update the OA ticket with the branch name and assign it over to a code reviewer who will follow the standard practice but notes will be made in OA instead of Bitbucket.
Reviewers will be checking for:

Commenting (before functions and inside functions).
Coding Best Practices
Drupal CS -St
Security - Above all, our code must be secure. Follow these without
variation.
Code Efficiency - Did you write 20 lines of code where a single function could have done it in one?
Does the code look correct - If you have to write code to count letters in a paragraph, you probably don't need to access a database parse an RSS file. This is just a general spot check, not testing of your code.
Code Reviewer Training Video: http://youtu.be/uaERJ1u7l70 
Ticket Best Practices
See Ticket Best Practices 3.0 DRAFT for upcoming updates.

Code Standards
Component Theming
Git Refresher
Video: Standardizing on Bitbucket
How to Code Review a Bitbucket Pull Request
Code Commits, Reviews and Merging
Ticket Best Pratices
Purpose
Goals
Ticket Creation & Responsibilities
Ticket Grooming
Ticket Workflows
Ticket Template Best Practices
Ticket Progress and Scope Changes
Glossary

Purpose
The purpose of this document is to improve team communication by adding clarity and predictability to our ticketing process. Employing company-wide best practices will ensure less uncertainty, ambiguity and lead to better efficiency overall.

Goals
Improve communication
Provide clarity on our ticket process
Increase efficiency
Ticket Creation & Responsibilities
Mediacurrent’s goal is to organize the work for clients into a manageable ticket queue that allows us to efficiently represent: completed work, current in-progress work and future work to be planned against. We do this in the form of arranging well-defined, actionable tickets into time-based groupings such as sprints or releases.

This organization of tickets is a shared responsibility between Project Managers/Customer Success Managers and Project leads.

Project Managers/CSMs are responsible for:
Working with the client and project leads to create tickets in JIRA utilizing Ticket Grooming practices below.
With with project leads and team to ensure tickets are groomed and have estimates.
Organizing the tickets into sprints and releases
Work with the client and leads to prioritize the backlog from most important to least
Coordinating ticket assignments based upon forecast, budget and priority
Ensuring ticket queue remains “current” by prompting clients for reviews and closing out completed tickets
This includes entering/updating any changes the client requests and notifying the assignee via Slack or Google Hangouts as early as possible of changes if the ticket is set to “In Progress”
Facilitating discussions with clients when scope changes arise within tickets
Project Leads are responsible for:
Ensuring each ticket has enough detailed information to be actionable
Links to any required documentation
Guidance on technology to be used
What is needed to meet client expectations
This will also be used as reference in testing
Overview of the ticket purpose
Technical documentation
Acceptance criteria
Description
Providing estimates to Project Manager/CSM
Collaborating with Project Manager to provide input on sprint/release planning and task assignments
Reviewing code, providing technical direction and answering questions from the team
Alerting Project Manager to items that are out of scope
Collaborating with Project Manager and developers to ensure ticket estimates are being met and value is delivered to client.
People assigned to work on the tickets are responsible for:
Commenting tickets to reflect progress made, remaining steps to be taken, and time spent on the tasks
Ensuring ticket is followed through to completion. Ensuring ticket does not get stalled in review, QA, UAT, etc.
Utilize 50% rule below ensuring that work expected to go over estimate is raised to lead/PM.
Updating the Acceptance Criteria/Description with any changes the client requests before it is sent to QA
Understand big picture of project and ensuring ticket execution delivers value to client based on time and deliverables.
Alerting Project Manager and Leads to questions, blockers and concerns
Helping facilitate project lead and project manager/csm responsibilities above.
Adding testing steps to the ticket before setting to “Ready for QA”
Go Here: (Provide link to area pertaining to the story also includes any user login information needed)
Do This: (Provide step by steps way to reproduce a passing result)
You Should See This: (What should the QA Engineer see in order to pass the ticket)
Steps include:
Ticket Grooming
Ticket titles, fields and descriptions should be updated as needed to add clarity and refine scope, requirements. It’s important that it’s clear to all parties what is to be accomplished in the ticket. This is primarily handled by the Project Leads and PM/CSM but could sometimes fall to the person working the ticket.

There are many reasons why having groomed tickets is important: resolving billing disputes, keeping clients focused, helping assignees understand exactly what they need to do, reporting, and so on.

The ticket notes should be an up-to-date representation of the scope of work required for that ticket. Assignees should not have to dig through comments to understand what they need to do. If major problems or changes are listed in the comments, you must update the acceptance criteria or the description accordingly to prevent important items from being lost in the comments. When description or acceptance criteria are updated a date/time it was updated should be noted on the case.

Ticket Workflows
The following workflows summarize the general flow of how tickets should be managed.

Bug Ticket Workflow
Clients or QA testers typically will create bug tickets, but anyone who finds a bug can create a bug ticket. Tickets initially are left unassigned and it is up to the PM/CSM or leads to groom and assign. When a bug is fixed and peer reviewed (via a Pull Request), it should be sent back to the reporter for approval.

Once approval is gained by the reporter (If it was not QA) then it will be sent to QA for Pass/Fail testing.

Feature / Task Ticket Workflow
Leads, PMs and CSMs are responsible for creating feature tickets that will then need to be groomed and assigned. Clients can also create tickets and these often require the most grooming. When a ticket is finished and peer reviewed (via a Pull Request), the ticket should be assigned back to the reporter for approval.

Discovery Ticket Workflow
If a ticket is going to take longer than 15-30 minutes to scope, then a discovery-only ticket should be created and approved by the client. The discovery ticket will have as a deliverable a) an estimate and b) a plan. The plan could be notes, a google doc, a mockup, etc..

When the discovery is finished, it should be closed out with the summary added to a new ticket. The new ticket will include the estimate delivered from the old ticket and will need to be approved by the client. The old ticket should be linked from the new ticket under the ‘Links’ heading or field. The new ticket will also have the required fields mentioned above (Technical Requirement, Acceptance Criteria and Description).

For clarity, it is a useful practice to indicate that a ticket is a discovery-only ticket by adding the word ‘Discovery’ to the title of the ticket.

Ticket Template Best Practices
On new project tickets it’s important to designate who will be primarily responsible for creating tickets. Note that clients will often create tickets which makes the practice of ticket grooming critical to maintain an organized issue queue.

Field	Best Practices
Project	Assign the ticket to the appropriate project / billing code.
Issue Type	All tickets should have the appropriate ‘type’ assigned (story, bug, task, epic).
Summary	A clear, 1 sentence summary of the problem or task with the content broken into Page: Section - Brief Description of problem (when applicable) 
- Homepage: Login - Red error at the top of page for logged in users 
- Homepage: Blog - Add a list of 10 most recent blog posts to the right rail of the homepage 
- Good bug example: 
- Good task example:
- Bad example task title: “Homepage changes” 
- Bad example bug title: “Speed is slowing down”
Testing instructions	There is a Testing Instructions section when you edit the ticket, all testing steps should go there in the following format: 
- Go Here: (Provide link to area pertaining to the story) (The link must be the FULL link to the dev or testing environment, no partials and no local urls) 
- Do This: (Provide step by steps way to reproduce a passing result) 
- You Should See This: (What should the QA Engineer see in order to pass the ticket)
Estimate	-All tickets that have a discovery, strategy, theming or dev deliverable must have an estimate. 
-Estimates should always be in one hour increments. 
-Assignee should review the estimate before begining work on the ticket.
Priority	It’s important to set priority so that every ticket isn’t a medium priority which doesn’t help assignees. 
-Highest: Work on tickets marked as important stops until ticket with this status is resolved.
-High: Current priority tickets. These will be actively worked on.
-Medium: Not active in current sprint but is ready to be actively worked on when time becomes available.
-Low/Lowest: Not to be actively worked on currently. Could be awaiting more information, grooming or for a future improvement down the road. If a task with this status is in the current sprint, it will be the lowest priority to be worked on.
Assignee	-This should be only assigned when that person can take actionable steps towards completion of the ticket
-If a ticket is not ready to work on then it should stay with the reporter or be moved to ‘unassigned’
Description	See examples below
Attachment	-Bug tickets should always include a screenshot (Exception: the bug is not visual or creating a screenshot is overly burdensome).
-Screenshots should be included if they can help clarify a task. Inline images are encouraged to help add context around the image being attached.
Label	Labels can be helpful for organizing tickets. These can vary by client.
Environment	OS/Browser, e.g. Win7/ie10, Win7/ie11, iOS/Safari, OS X/Firefox 34.
Epic	Epic’s are typically large milestones or a collection of stories. Epics can help further organize tasks and stories.
Sprint	It’s important to organize tasks into Sprints and have explicit dates for those Sprints (typically a 1-3 week cycle).
Due Date	If the ticket is part of a sprint or has an explicit due date this field should be used.
Description field
“Task” ticket template:
Description

Should be a brief summary of what the ticket will accomplish. This should primarily be written by the client and project manager. It should read non technical about what the outcome of the ticket should be. If transcribing notes, email or a phone call be sure it is condensed and worded in a manner that quickly gets to the core of what will be accomplished.)

Technical Documentation

List any technical documentation vital to the tickets completion. (As needed)

Add view block showing blogs
Filter blogs by taxonomy term of “Sports”
Show only 10 blogs
Show only titles of blog posts.
Add below related content block and above 300x250 ad position.
Links

Functional Spec Link URL: http://foobar.com/ 
Acceptance Criteria

Indicate the criteria by which this ticket is considered complete. This should be written to target a non technical audience.

On page /sports I see a listing of blog post titles below the related content block
“Bug” ticket template:
Description

(Brief summary of the problem. It should read non technical about what the outcome of the ticket should be)

Technical Documentation (when needed)

Steps to reproduce

(Critical. Sometimes client will supply, sometimes it will be inferred by the assignee. Once this has been established the ticket should be updated for future reference.)

Links

(Critical that links are supplied when possible, not just screenshots or a description of the problem.)

Comment Template Best Practices
Aside from writing good ticket descriptions and grooming tickets regularly, status update comments should follow a standard template. Status updates should be made when changing the workflow status & assignee of a ticket or once a day to summarize the work that has been done.

A status update comment should answer the following questions:

What progress has been made so far?
What technical approach was taken to implement?
How can this code be tested?
What steps are needed to deploy this code?
What next steps are remaining?
Attach any screenshots, URLs or User Account credentials needed
Comment status update template:
Description

A one sentence executive summary of work completed. This should be written for a client to understand what has happened so far.

Steps Taken

Developer steps taken to get to this point. Include any research links used, how this affects ticket and project and details regarding implementation. This should be more details to any comments already left in the code. Link to PR or name of feature branch should be included when applicable.

Testing Instructions (if ready for testing) (Also include in testing instructions field)

Steps to show issue no longer exists.

Specific page URL
Username/Password (As needed)
Step by step of the “Go here, Do this and you should See this” method mentioned earlier
What QA should see in order to “Pass” the ticket (Be specific)
Details should be listed including links and screenshots.
Deployment Instructions

List of steps to deploy change (e.g. drush cc all, drush fr -y featurename, etc.)
Next Steps

List of next steps.
Ticket Progress and Scope Changes
During the ticket lifecycle, the ticket scope may require changes. If this occurs, communicate with project leadership: project lead and/or pm, to decide if any of the following applies:

Original ticket's description can be updated without changes to estimate
Original ticket's description can be updated with changes to remaining or original estimate
New ticket's with additional scope and estimates are needed.
The 50% Rule of Thumb
Once you've completed 50% of the tickets estimate hours, ask yourself if you are 50% completed with the ticket's acceptance criteria. If not, communicate with project leadership: project lead and/or pm.

Glossary
CSM - Customer Success Manager
PM - Project Manager
QA - Quality Assurance
