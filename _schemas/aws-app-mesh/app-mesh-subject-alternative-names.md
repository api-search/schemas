---
description: An object that represents the subject alternative names secured by the certificate.
layout: schema
name: SubjectAlternativeNames
properties_list:
- description: ''
  name: match
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-subject-alternative-names-schema.json
slug: app-mesh-subject-alternative-names
source_filename: app-mesh-subject-alternative-names-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"match\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubjectAlternativeNameMatchers\"\n        },\n        {\n          \"description\": \"An object that represents the criteria for determining a SANs match.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"match\"\n  ],\n  \"description\": \"An object that represents the subject alternative names secured by the certificate.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-subject-alternative-names-schema.json\",\n  \"title\": \"SubjectAlternativeNames\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-subject-alternative-names-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: SubjectAlternativeNames
---
