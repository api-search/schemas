---
description: An object that represents the methods by which a subject alternative name on a peer Transport Layer Security (TLS) certificate can be matched.
layout: schema
name: SubjectAlternativeNameMatchers
properties_list:
- description: ''
  name: exact
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-subject-alternative-name-matchers-schema.json
slug: app-mesh-subject-alternative-name-matchers
source_filename: app-mesh-subject-alternative-name-matchers-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"exact\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubjectAlternativeNameList\"\n        },\n        {\n          \"description\": \"The values sent must match the specified values exactly.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"exact\"\n  ],\n  \"description\": \"An object that represents the methods by which a subject alternative name on a peer Transport Layer Security (TLS) certificate can be matched.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-subject-alternative-name-matchers-schema.json\",\n  \"title\": \"SubjectAlternativeNameMatchers\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-subject-alternative-name-matchers-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: SubjectAlternativeNameMatchers
---
