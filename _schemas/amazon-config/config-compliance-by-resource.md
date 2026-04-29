---
description: Indicates whether an Amazon Web Services resource that is evaluated according to one or more Config rules is compliant. A resource is compliant if it complies with all of the rules that evaluate it. A resource is noncompliant if it does not comply with one or more of these rules.
layout: schema
name: ComplianceByResource
properties_list:
- description: ''
  name: ResourceType
  type: object
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: Compliance
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-compliance-by-resource-schema.json
slug: config-compliance-by-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-compliance-by-resource-schema.json\",\n  \"title\": \"ComplianceByResource\",\n  \"description\": \"Indicates whether an Amazon Web Services resource that is evaluated according to one or more Config rules is compliant. A resource is compliant if it complies with all of the rules that evaluate it. A resource is noncompliant if it does not comply with one or more of these rules.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"The type of the Amazon Web Services resource that was evaluated.\"\n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BaseResourceId\"\
  \n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services resource that was evaluated.\"\n        }\n      ]\n    },\n    \"Compliance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Compliance\"\n        },\n        {\n          \"description\": \"Indicates whether the Amazon Web Services resource complies with all of the Config rules that evaluated it.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-compliance-by-resource-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ComplianceByResource
---
