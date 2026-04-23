# InvokingApexMethodForAgentActions
agent actions are essentially supposed to be monitored and if agent starts firing the multiple actions in a single conversational methods. sometime it may hit a transactional limits. 


My approach for the solution:

- Building a complex agent to handle all complex multiple actions in a reasoning loop.
- Started hitting some exceptional errors after a post deployment in production.
- occured mainly under a heavy concurrent usage of agent.

Primary approach:
- Auditing all the avaialble agent actions.
- Methods to overcome all the bulkification problem.
- Moved to collection based SOQL.
- Offloaded to perform all async Queueable jobs.
- Tried to replace all the large dataset traversal.
  
