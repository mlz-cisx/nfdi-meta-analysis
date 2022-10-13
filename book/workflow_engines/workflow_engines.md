# Workflow Engines
##### tags: `#TA2` `#TA3`

A workflow engine manages and monitors the state of activities in a workflow, such as the processing and approval of a loan application form, and determines which new activity to transition to according to defined processes (workflows).
A workflow engine facilitates the flow of information, tasks, and events. Workflow engines may also be referred to as Workflow Orchestration Engines.


Workflow engines mainly have three functions:

* Verification of the current process status: Check whether it is valid executing a task, given current status.
* Determine the authority of users: Check if the current user is permitted to execute the task.
* Executing condition script: After passing the previous two steps, the workflow engine executes the task, and if the execution successfully completes, it returns the success, if not, it reports the error to trigger and roll back the change.