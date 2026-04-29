---
description: Represents a provisioning workflow configured for an application in the Productiv platform.
layout: schema
name: ProvisioningWorkflow
properties_list:
- description: The unique identifier of the workflow.
  name: workflowId
  type: string
- description: The name of the workflow.
  name: workflowName
  type: string
- description: The application associated with the workflow.
  name: applicationId
  type: string
- description: The status of the workflow.
  name: status
  type: string
provider_name: Productiv
provider_slug: productiv
schema_file: json-schema/provisioning-workflow.json
slug: provisioning-workflow
source_json: "{\n  \"$id\": \"provisioning-workflow.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProvisioningWorkflow\",\n  \"description\": \"Represents a provisioning workflow configured for an application in the Productiv platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workflowId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the workflow.\"\n    },\n    \"workflowName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the workflow.\"\n    },\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"description\": \"The application associated with the workflow.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the workflow.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/json-schema/provisioning-workflow.json
tags:
- Application Portfolio
- Provisioning
- SaaS Management
- Spend Management
- Usage Analytics
title: ProvisioningWorkflow
---
