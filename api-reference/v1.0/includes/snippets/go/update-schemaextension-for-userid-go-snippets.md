---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


// Code snippets are only available for the latest major version. Current major version is $v1.*

// Dependencies
import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-sdk-go/models"
	  //other-imports
)

requestBody := graphmodels.NewUser()
additionalData := map[string]interface{}{
ext55gb1l09_msLearnCourses := graphmodels.New()
courseType := "Admin"
ext55gb1l09_msLearnCourses.SetCourseType(&courseType) 
	requestBody.SetExt55gb1l09_msLearnCourses(ext55gb1l09_msLearnCourses)
}
requestBody.SetAdditionalData(additionalData)

// To initialize your graphClient, see https://learn.microsoft.com/en-us/graph/sdks/create-client?from=snippets&tabs=go
users, err := graphClient.Users().ByUserId("user-id").Patch(context.Background(), requestBody, nil)


```