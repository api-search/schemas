---
description: A collection of the names of Amazon Web Services services.
layout: schema
name: ServiceCollection
properties_list:
- description: ''
  name: ServiceNames
  type: object
provider_name: Amazon DevOps Guru
provider_slug: amazon-devops-guru
schema_file: json-schema/amazon-devops-guru-service-collection-schema.json
slug: amazon-devops-guru-service-collection
source_filename: amazon-devops-guru-service-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-service-collection-schema.json\",\n  \"title\": \"ServiceCollection\",\n  \"description\": \"A collection of the names of Amazon Web Services services.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceNames\"\n        },\n        {\n          \"description\": \"An array of strings that each specifies the name of an Amazon Web Services service.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-devops-guru/refs/heads/main/json-schema/amazon-devops-guru-service-collection-schema.json
tags:
- Anomaly Detection
- DevOps
- Machine Learning
- Operational Intelligence
title: ServiceCollection
---
