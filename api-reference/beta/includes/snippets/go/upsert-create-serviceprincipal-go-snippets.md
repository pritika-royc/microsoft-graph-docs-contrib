---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


// Code snippets are only available for the latest major version. Current major version is $v0.*

// Dependencies
import (
	  "context"
	  abstractions "github.com/microsoft/kiota-abstractions-go"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-beta-sdk-go/models"
	  graphserviceprincipals(appid='{appid}') "github.com/microsoftgraph/msgraph-beta-sdk-go/serviceprincipals(appid='{appid}')"
	  //other-imports
)

headers := abstractions.NewRequestHeaders()
headers.Add("Prefer", "create-if-missing")

configuration := &graphserviceprincipals(appid='{appid}').ServicePrincipals(appId='{appId}')RequestBuilderPatchRequestConfiguration{
	Headers: headers,
}
requestBody := graphmodels.NewServicePrincipal()
displayName := "My app instance"
requestBody.SetDisplayName(&displayName) 

// To initialize your graphClient, see https://learn.microsoft.com/en-us/graph/sdks/create-client?from=snippets&tabs=go
appId := "{appId}"
servicePrincipals, err := graphClient.ServicePrincipalsWithAppId(&appId).Patch(context.Background(), requestBody, configuration)


```