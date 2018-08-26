---
swagger: "2.0"
x-collection-name: AWS Elastic Beanstalk
x-complete: 1
info:
  title: AWS Elastic Beanstalk API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateApplicationResourceLifecycle:
    get:
      summary: Update Application Resource Lifecycle
      description: Modifies lifecycle settings for an application.
      operationId: updateApplicationResourceLifecycle
      x-api-path-slug: actionupdateapplicationresourcelifecycle-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application
        type: string
      - in: query
        name: ResourceLifecycleConfig
        description: The lifecycle configuration
        type: string
      responses:
        200:
          description: OK
      tags:
      - Application Resource Lifecycle
---