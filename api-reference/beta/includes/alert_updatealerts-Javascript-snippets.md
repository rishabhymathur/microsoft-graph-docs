
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const alert = {
  value: [
    {
      assignedTo: "String",
      closedDateTime: "String (timestamp)",
      comments: ["String"],
      feedback: {@odata.type: "microsoft.graph.alertFeedback"},
      id: "String (identifier)",
      status: {@odata.type: "microsoft.graph.alertStatus"},
      tags: ["String"],
      vendorInformation:
        {
          provider: "String",
          vendor: "String"
        }
    }
  ]
};

let res = await client.api('/security/alerts/updateAlerts')
	.version('beta')
	.post(alert);

```