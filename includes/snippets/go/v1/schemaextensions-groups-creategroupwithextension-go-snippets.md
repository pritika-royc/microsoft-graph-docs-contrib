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

requestBody := graphmodels.NewGroup()
displayName := "New Managers March 2024"
requestBody.SetDisplayName(&displayName) 
description := "New Managers training course for March 2024"
requestBody.SetDescription(&description) 
groupTypes := []string {
	"Unified",
}
requestBody.SetGroupTypes(groupTypes)
mailEnabled := true
requestBody.SetMailEnabled(&mailEnabled) 
mailNickname := "newMan202403"
requestBody.SetMailNickname(&mailNickname) 
securityEnabled := false
requestBody.SetSecurityEnabled(&securityEnabled) 
additionalData := map[string]interface{}{
bellowscollege_courses := graphmodels.New()
courseId := "123"
bellowscollege_courses.SetCourseId(&courseId) 
courseName := "New Managers"
bellowscollege_courses.SetCourseName(&courseName) 
courseType := "Online"
bellowscollege_courses.SetCourseType(&courseType) 
	requestBody.SetBellowscollege_courses(bellowscollege_courses)
}
requestBody.SetAdditionalData(additionalData)

// To initialize your graphClient, see https://learn.microsoft.com/en-us/graph/sdks/create-client?from=snippets&tabs=go
groups, err := graphClient.Groups().Post(context.Background(), requestBody, nil)


```