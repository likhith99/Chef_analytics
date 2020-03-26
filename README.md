# Chef_analytics
**Wiki for Chef analytics:**  an Add-on available for chef <br>

### What is Chef Analytics?
<hr>
The Chef Analytics server collects all of this data and makes it visible from the Chef Analytics user interface.<br>

- Provides real-time visiblity into the chef server
- runs on seperate hardware than the chef server
- provides the logging feature to the chef server for better visibility into the server and troubleshooting
- Gather and consolidate the data from clients and severs

### What are Actions:
<hr>
Actions are action logs from the chef server,
It can give information on who performed what like the administration and policy changes to the chef server. <br>

Actions can occur in different forms like:
- `Knife commands`
- `Management console`
- `Chef clients` 
- `workstations`

All these actions are tracked by the chef analytics and are actionable in form of GUI

- Important as it can be used to predict future failures and actions that can cause a catastrophy.
- The actions in Chef Analytics may be exported as a JSON document or a CSV file.

### How it works:
<hr> 
Chef analytics works as following: 

- Chef analytics pushes communication to the Chef Server
- It does not require any other virtual machine or any seperate cloud server
- Uses the `publish-subsribe messaging platform`
- All the actions are achived into a database and can be customized on how it can be stored.
- All the actions in your organization can be viewed

### What is can do:
<hr>
Chef analytics can help you with the following info:

- Time and Date when a specific user uploaded a cookbook from their workstation to the Chef server
- Time and Date at which a cookbook stopped working or had issues
- Traces of the changes that were made before any issues or when chef stopped working
- Which systems had the latest patch installed?


### Pros of using Chef Analytics:
<hr> 
Advantages having Chef Analytics as follows: 

- The `WebUI` that is available for the dashboard makes data visualization much easier
- All the action data is searchable via web visualization tools and queries can be saved
- How the data is stored is highly customizable
- The data can be presented in different form using any of the tools
- Action log GUI can be used to perform other actions on top of present actions
- Actions can also be viewed at each object level 
- Notifications can be sent out depending on the actions logged to other devops tools
- Allows data mining on the logs for deep analytics for future purposes

### Known Issues 

- Implementation of Chef is comparatively complex and Chef Analytics can cause additional overhead and complexity to the architecture
- Adding chef-analytics required rabbitmq changes

- attributes breaks chef-server
- https://github.com/chef-cookbooks/chef-server/issues/119

- https://github.com/chef-boneyard/chef-analytics/pull/12 issues fixed.


