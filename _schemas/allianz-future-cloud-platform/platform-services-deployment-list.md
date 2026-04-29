---
description: Paginated list of deployment records
layout: schema
name: DeploymentList
properties_list:
- description: Total number of deployments
  name: total
  type: integer
- description: List of deployment records
  name: items
  type: array
provider_name: Allianz Future Cloud Platform
provider_slug: allianz-future-cloud-platform
schema_file: json-schema/platform-services-deployment-list-schema.json
slug: platform-services-deployment-list
source_filename: platform-services-deployment-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-deployment-list-schema.json\",\n  \"title\": \"DeploymentList\",\n  \"description\": \"Paginated list of deployment records\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of deployments\",\n      \"example\": 45\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"List of deployment records\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Deployment\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-deployment-list-schema.json
tags:
- Cloud Platform
- Enterprise
- Financial Services
- Insurance
- Platform Engineering
- Kubernetes
title: DeploymentList
---
