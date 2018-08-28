---
swagger: "2.0"
x-collection-name: AWS Elasticsearch Service
x-complete: 0
info:
  title: Amazon Elasticsearch Service API Update Elasticsearch Domain Config
  version: 1.0.0
  description: |-
    Modifies the configuration of an Amazon ES domain, such as the instance type and the
                    number of instances. Use the POST HTTP method with this
                    operation.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2015-01-01/es/domain/{domain_name}/config:
    post:
      summary: Update Elasticsearch Domain Config
      description: |-
        Modifies the configuration of an Amazon ES domain, such as the instance type and the
                        number of instances. Use the POST HTTP method with this
                        operation.
      operationId: updateElasticsearchDomainConfig
      x-api-path-slug: 20150101esdomaindomain-nameconfig-post
      responses:
        200:
          description: OK
      tags:
      - Domains
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---