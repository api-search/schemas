---
description: TagResourceRequest schema from Amazon CodeGuru Security
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: tags
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-tag-resource-request-schema.json
slug: amazon-codeguru-security-tag-resource-request
source_filename: amazon-codeguru-security-tag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"description\": \"TagResourceRequest schema from Amazon CodeGuru Security\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"<p>An array of key-value pairs used to tag an existing scan. A tag is a custom attribute label with two parts:</p> <ul> <li> <p>A tag key. For example, <code>CostCenter</code>, <code>Environment</code>, or <code>Secret</code>. Tag keys are case sensitive.</p> </li> <li> <p>An optional tag value field. For example, <code>111122223333</code>, <code>Production</code>, or a team name. Omitting the tag value is the same as using\
  \ an empty string. Tag values are case sensitive.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-tag-resource-request-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: TagResourceRequest
---
