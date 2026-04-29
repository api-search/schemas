---
description: PackageRequest schema from Apache OpenWhisk
layout: schema
name: PackageRequest
properties_list:
- description: ''
  name: annotations
  type: array
- description: ''
  name: parameters
  type: array
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-package-request-schema.json
slug: apache-openwhisk-package-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-package-request-schema.json\",\n  \"title\": \"PackageRequest\",\n  \"description\": \"PackageRequest schema from Apache OpenWhisk\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"annotations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KeyValue\"\n      }\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/KeyValue\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-package-request-schema.json
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: PackageRequest
---
