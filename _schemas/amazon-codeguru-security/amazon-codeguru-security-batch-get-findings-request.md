---
description: BatchGetFindingsRequest schema from Amazon CodeGuru Security
layout: schema
name: BatchGetFindingsRequest
properties_list:
- description: ''
  name: findingIdentifiers
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-batch-get-findings-request-schema.json
slug: amazon-codeguru-security-batch-get-findings-request
source_filename: amazon-codeguru-security-batch-get-findings-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-batch-get-findings-request-schema.json\",\n  \"title\": \"BatchGetFindingsRequest\",\n  \"description\": \"BatchGetFindingsRequest schema from Amazon CodeGuru Security\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"findingIdentifiers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingIdentifiers\"\n        },\n        {\n          \"description\": \"A list of finding identifiers. Each identifier consists of a <code>scanName</code> and a <code>findingId</code>. You retrieve the <code>findingId</code> when you call <code>GetFindings</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"findingIdentifiers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-batch-get-findings-request-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: BatchGetFindingsRequest
---
