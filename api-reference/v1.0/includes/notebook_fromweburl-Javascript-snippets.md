
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const CopyNotebookModel = {webUrl:"webUrl value"};

let res = await client.api('/me/onenote/notebooks/GetNotebookFromWebUrl')
	.post(CopyNotebookModel);

```