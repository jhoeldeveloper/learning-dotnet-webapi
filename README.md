# Learning ASP.NET Core Web API - .NET 9.0 with the official documentation

source: https://learn.microsoft.com/en-us/aspnet/core/tutorials/first-web-api?view=aspnetcore-9.0&tabs=visual-studio

**Commands**
```
Install-Package MongoDB.Driver
winget install jqlang.jq

curl.exe -X GET 'https://localhost:7157/api/todoitems/' | jq

curl.exe -X POST 'https://localhost:7157/api/todoitems/' `
-H 'Content-Type: application/json' `
-d '{""id"":""6bb8b868-dba1-4f1a-93b7-24ebce87e243"",
""name"":""A Test Item"",
""notes"": ""asdf"",
""done"": false}' | jq

curl.exe -X PUT 'https://localhost:7157/api/todoitems/' `
-H 'Content-Type: application/json' `
--data '{
  ""id"": ""6bb8b868-dba1-4f1a-93b7-24ebce87e243"",
  ""name"": ""A Test Item"",
  ""notes"": ""test"",
  ""done"": true
}' | jq

curl.exe -X DELETE 'https://localhost:7157/api/todoitems/6bb8b868-dba1-4f1a-93b7-24ebce87e243'

```