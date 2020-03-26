# Chef_analytics
Wiki for Chef_analytics: add-on to chef

- Provides real-time visiblity into the chef server
- runs on seperate hardware than the chef server
- provides the logging feature to the chef server for better visibility into the server and troubleshooting
- Gather and consolidate the data from clients and severs

### Actions
<hr>
Actions are action logs from the chef server 
It can give information on who performed what like the administration and policy changes to the chef server

Actions can occur in different forms like:
- `Knife commands`
- `Management console`
- `Chef clients` 
- `workstations`

All these actions are tracked by the chef analytics and are actionable in form of GUI

- Important as it can be used to predict future failures and actions that can cause a catastrophy.

### How it works:
<hr> 
Chef analytics works as following: 

- Chef analytics pushes communication to the Chef Server
- It does not require any other virtual machine or any seperate cloud server
- Uses the `publish-subsribe messaging platform`
- All the actions are achived into a database and can be customized on how it can be stored.
- All the actions in your organization can be viewed



### Pros
<hr> 
Advantages having Chef Analytics as follows: 

- All the action data is searchable via web visualization tools
- How the data is stored is highly customizable
- The data can be presented in different form using any of the tools
- Action log GUI can be used to perform other actions on top of present actions
- Actions can also be viewed at each object level 
- Notifications can be sent out depending on the actions logged to other devops tools
- Allows data mining on the logs for deep analytics for future purposes

### Known Issues 

- Adding chef-analytics required rabbitmq changes
- attributes breaks chef-server
- https://github.com/chef-cookbooks/chef-server/issues/119

- https://github.com/chef-boneyard/chef-analytics/pull/12 issues fixed.


