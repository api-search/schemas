---
description: BatchGetFindingsResponse schema from Amazon CodeGuru Security
layout: schema
name: BatchGetFindingsResponse
properties_list:
- description: ''
  name: failedFindings
  type: object
- description: ''
  name: findings
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-batch-get-findings-response-schema.json
slug: amazon-codeguru-security-batch-get-findings-response
source_filename: amazon-codeguru-security-batch-get-findings-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-batch-get-findings-response-schema.json\",\n  \"title\": \"BatchGetFindingsResponse\",\n  \"description\": \"BatchGetFindingsResponse schema from Amazon CodeGuru Security\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"failedFindings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchGetFindingsErrors\"\n        },\n        {\n          \"description\": \"A list of errors for individual findings which were not fetched. Each BatchGetFindingsError contains the <code>scanName</code>, <code>findingId</code>, <code>errorCode</code> and error <code>message</code>.\"\n        }\n      ]\n    },\n    \"findings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Findings\"\n        },\n        {\n          \"\
  description\": \" A list of all requested findings.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"failedFindings\",\n    \"findings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-batch-get-findings-response-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: BatchGetFindingsResponse
---
