---
description: <p>Provides summary information for an App Runner service.</p> <p>This type contains limited information about a service. It doesn't include configuration details. It's returned by the <a href="https://docs.aws.amazon.com/apprunner/latest/api/API_ListServices.html">ListServices</a> action. Complete service information is returned by the <a href="https://docs.aws.amazon.com/apprunner/latest/api/API_CreateService.html">CreateService</a>, <a href="https://docs.aws.amazon.com/apprunner/latest/api/API_DescribeService.html">DescribeService</a>, and <a href="https://docs.aws.amazon.com/apprunner/latest/api/API_DeleteService.html">DeleteService</a> actions using the <a href="https://docs.aws.amazon.com/apprunner/latest/api/API_Service.html">Service</a> type.</p>
layout: schema
name: ServiceSummary
properties_list:
- description: ''
  name: ServiceName
  type: object
- description: ''
  name: ServiceId
  type: object
- description: ''
  name: ServiceArn
  type: object
- description: ''
  name: ServiceUrl
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: UpdatedAt
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-servicesummary-schema.json
slug: amazon-app-runner-servicesummary
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ServiceSummary\",\n  \"description\": \"<p>Provides summary information for an App Runner service.</p> <p>This type contains limited information about a service. It doesn't include configuration details. It's returned by the <a href=\\\"https://docs.aws.amazon.com/apprunner/latest/api/API_ListServices.html\\\">ListServices</a> action. Complete service information is returned by the <a href=\\\"https://docs.aws.amazon.com/apprunner/latest/api/API_CreateService.html\\\">CreateService</a>, <a href=\\\"https://docs.aws.amazon.com/apprunner/latest/api/API_DescribeService.html\\\">DescribeService</a>, and <a href=\\\"https://docs.aws.amazon.com/apprunner/latest/api/API_DeleteService.html\\\">DeleteService</a> actions using the <a href=\\\"https://docs.aws.amazon.com/apprunner/latest/api/API_Service.html\\\">Service</a> type.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceName\": {},\n\
  \    \"ServiceId\": {},\n    \"ServiceArn\": {},\n    \"ServiceUrl\": {},\n    \"CreatedAt\": {},\n    \"UpdatedAt\": {},\n    \"Status\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-servicesummary-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: ServiceSummary
---
