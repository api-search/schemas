---
description: <p>Describes an App Runner service. It can describe a service in any state, including deleted services.</p> <p>This type contains the full information about a service, including configuration details. It's returned by the <a href="https://docs.aws.amazon.com/apprunner/latest/api/API_CreateService.html">CreateService</a>, <a href="https://docs.aws.amazon.com/apprunner/latest/api/API_DescribeService.html">DescribeService</a>, and <a href="https://docs.aws.amazon.com/apprunner/latest/api/API_DeleteService.html">DeleteService</a> actions. A subset of this information is returned by the <a href="https://docs.aws.amazon.com/apprunner/latest/api/API_ListServices.html">ListServices</a> action using the <a href="https://docs.aws.amazon.com/apprunner/latest/api/API_ServiceSummary.html">ServiceSummary</a> type.</p>
layout: schema
name: Service
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
  name: DeletedAt
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: SourceConfiguration
  type: object
- description: ''
  name: InstanceConfiguration
  type: object
- description: ''
  name: EncryptionConfiguration
  type: object
- description: ''
  name: HealthCheckConfiguration
  type: object
- description: ''
  name: AutoScalingConfigurationSummary
  type: object
- description: ''
  name: NetworkConfiguration
  type: object
- description: ''
  name: ObservabilityConfiguration
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-service-schema.json
slug: amazon-app-runner-service
source_filename: amazon-app-runner-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Service\",\n  \"description\": \"<p>Describes an App Runner service. It can describe a service in any state, including deleted services.</p> <p>This type contains the full information about a service, including configuration details. It's returned by the <a href=\\\"https://docs.aws.amazon.com/apprunner/latest/api/API_CreateService.html\\\">CreateService</a>, <a href=\\\"https://docs.aws.amazon.com/apprunner/latest/api/API_DescribeService.html\\\">DescribeService</a>, and <a href=\\\"https://docs.aws.amazon.com/apprunner/latest/api/API_DeleteService.html\\\">DeleteService</a> actions. A subset of this information is returned by the <a href=\\\"https://docs.aws.amazon.com/apprunner/latest/api/API_ListServices.html\\\">ListServices</a> action using the <a href=\\\"https://docs.aws.amazon.com/apprunner/latest/api/API_ServiceSummary.html\\\">ServiceSummary</a> type.</p>\",\n  \"type\": \"object\",\n\
  \  \"properties\": {\n    \"ServiceName\": {},\n    \"ServiceId\": {},\n    \"ServiceArn\": {},\n    \"ServiceUrl\": {},\n    \"CreatedAt\": {},\n    \"UpdatedAt\": {},\n    \"DeletedAt\": {},\n    \"Status\": {},\n    \"SourceConfiguration\": {},\n    \"InstanceConfiguration\": {},\n    \"EncryptionConfiguration\": {},\n    \"HealthCheckConfiguration\": {},\n    \"AutoScalingConfigurationSummary\": {},\n    \"NetworkConfiguration\": {},\n    \"ObservabilityConfiguration\": {}\n  },\n  \"required\": [\n    \"ServiceName\",\n    \"ServiceId\",\n    \"ServiceArn\",\n    \"CreatedAt\",\n    \"UpdatedAt\",\n    \"Status\",\n    \"SourceConfiguration\",\n    \"InstanceConfiguration\",\n    \"AutoScalingConfigurationSummary\",\n    \"NetworkConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-service-schema.json
tags:
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: Service
---
