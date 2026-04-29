---
description: An Amazon Launch Wizard deployment of an enterprise application.
layout: schema
name: Deployment
properties_list:
- description: The ID of the deployment.
  name: id
  type: string
- description: The name of the deployment.
  name: name
  type: string
- description: The name of the workload.
  name: workloadName
  type: string
- description: The current status of the deployment.
  name: status
  type: string
- description: The time the deployment was created.
  name: createdAt
  type: string
- description: The time the deployment was deleted.
  name: deletedAt
  type: string
provider_name: Amazon Launch Wizard
provider_slug: amazon-launch-wizard
schema_file: json-schema/amazon-launch-wizard-deployment-schema.json
slug: amazon-launch-wizard-deployment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-launch-wizard/refs/heads/main/json-schema/amazon-launch-wizard-deployment-schema.json\",\n  \"title\": \"Deployment\",\n  \"description\": \"An Amazon Launch Wizard deployment of an enterprise application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the deployment.\",\n      \"example\": \"deployment-abc12345\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the deployment.\",\n      \"example\": \"sap-hana-production\"\n    },\n    \"workloadName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the workload.\",\n      \"example\": \"SAP HANA\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the deployment.\",\n      \"example\": \"COMPLETED\"\
  ,\n      \"enum\": [\n        \"COMPLETED\",\n        \"CREATING\",\n        \"FAILED\",\n        \"IN_PROGRESS\",\n        \"VALIDATING\"\n      ]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The time the deployment was created.\",\n      \"format\": \"date-time\"\n    },\n    \"deletedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The time the deployment was deleted.\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-launch-wizard/refs/heads/main/json-schema/amazon-launch-wizard-deployment-schema.json
tags:
- AWS
- Deployment
- Enterprise Applications
- SAP
- SQL Server
title: Deployment
---
