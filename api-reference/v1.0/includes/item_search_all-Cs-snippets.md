
```Cs

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var search = await graphClient.Me.Drive.Search('{search-query}')
	.Request()
	.GetAsync();

```