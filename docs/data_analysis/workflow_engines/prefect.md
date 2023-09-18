# Prefect
##### tags: `#TA2` `#TA3`

[The Prefect Hybrid Model](https://medium.com/the-prefect-blog/the-prefect-hybrid-model-1b70c7fd296) allowing for seperation of workflow management and workflow processing. This means the management can be done on one server while the data and the procession is done on different servers.


## Functionality

* [Scheduling](https://docs.prefect.io/concepts/schedules/)
* [Retries](https://docs.prefect.io/concepts/tasks/#task-arguments)
* [Logging](https://docs.prefect.io/concepts/logs/)
* [Caching](https://docs.prefect.io/concepts/tasks/#caching)
* [Notifications](https://docs.prefect.io/ui/notifications/)
* [Observability](https://docs.prefect.io/ui/overview/)


## Flows & Tasks

[Flows](https://docs.prefect.io/concepts/flows/) are like functions. They can take inputs, perform work, and return an output.

A [task](https://docs.prefect.io/concepts/tasks/) is a function that represents a discrete unit of work in a Prefect workflow. They are special because they receive metadata about upstream dependencies and the state of those dependencies before they run, even if they don't receive any explicit data inputs from them. This gives you the opportunity to, for example, have a task wait on the completion of another task before executing.


## Agents

Agents run inside a user's architecture, and are responsible for starting and monitoring flow runs.

* Local
* Docker
* Kubernetes
* [More...](https://docs-v1.prefect.io/orchestration/agents/overview.html#agent-types)


## Server

It is possible to deploy our own [Prefect Cloud](https://docs.prefect.io/getting-started/overview/#get-started-with-prefect-2) (Prefect Hybrid Model), where we run one server instance, while connecting multiple storage & compute instances.


# Questions

How would we manage the workflows across multiple instances? How would we route the execution of the workflow to be done on the instances where the data is already available?