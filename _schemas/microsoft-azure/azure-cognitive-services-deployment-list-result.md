---
description: The list of cognitive services account deployments.
layout: schema
name: DeploymentListResult
properties_list:
- description: An array of deployments.
  name: value
  type: array
- description: The link used to get the next page of deployments.
  name: nextLink
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cognitive-services-deployment-list-result-schema.json
slug: azure-cognitive-services-deployment-list-result
source_filename: azure-cognitive-services-deployment-list-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeploymentListResult\",\n  \"type\": \"object\",\n  \"description\": \"The list of cognitive services account deployments.\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"description\": \"An array of deployments.\"\n    },\n    \"nextLink\": {\n      \"type\": \"string\",\n      \"description\": \"The link used to get the next page of deployments.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cognitive-services-deployment-list-result-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: DeploymentListResult
---
