# Functions versus Logic Apps

Functions and Logic Apps can both create complex orchestrations. An orchestration is a collection of functions or steps that are executed to accomplish a complex task.

- **With Functions**, you write code to complete each step.
- **With Logic Apps**, you use a GUI to define the actions and how they relate to one another.

You can mix and match services when you build an orchestration, calling functions from Logic Apps and calling Logic Apps from functions.

## Common Differences Between Functions and Logic Apps

| Aspect               | Functions                                   | Logic Apps                                  |
|----------------------|--------------------------------------------|--------------------------------------------|
| **State**            | Normally stateless, but Durable Functions provide state. | Stateful.                                   |
| **Development**      | Code-first (imperative).                   | Designer-first (declarative).              |
| **Connectivity**     | About a dozen built-in binding types. Write code for custom bindings. | Large collection of connectors. Enterprise Integration Pack for B2B scenarios. Build custom connectors. |
| **Actions**          | Each activity is an Azure function. Write code for activity functions. | Large collection of ready-made actions.    |
| **Monitoring**       | Azure Application Insights.                | Azure portal, Log Analytics.               |
| **Management**       | REST API, Visual Studio.                   | Azure portal, REST API, PowerShell, Visual Studio. |
| **Execution Context** | Can run locally or in the cloud.           | Runs only in the cloud.                    |