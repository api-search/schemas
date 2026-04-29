---
description: Worker configuration defining the compute resources allocated to a CloudHub application, including the number of workers and their size.
layout: schema
name: WorkerConfig
properties_list:
- description: Number of worker instances
  name: amount
  type: integer
- description: Worker type defining the vCore size and memory
  name: type
  type: object
provider_name: MuleSoft
provider_slug: mulesoft
schema_file: json-schema/mulesoft-anypoint-platform-worker-config-schema.json
slug: mulesoft-anypoint-platform-worker-config
source_filename: mulesoft-anypoint-platform-worker-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkerConfig\",\n  \"type\": \"object\",\n  \"description\": \"Worker configuration defining the compute resources allocated to a CloudHub application, including the number of workers and their size.\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of worker instances\"\n    },\n    \"type\": {\n      \"type\": \"object\",\n      \"description\": \"Worker type defining the vCore size and memory\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mulesoft/refs/heads/main/json-schema/mulesoft-anypoint-platform-worker-config-schema.json
tags:
- API Gateway
- API Management
- Enterprise
- Integration
title: WorkerConfig
---
