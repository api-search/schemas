---
description: A resource not in compliance with a Firewall Manager policy.
layout: schema
name: ComplianceViolator
properties_list:
- description: ID of the non-compliant resource.
  name: ResourceId
  type: string
- description: Reason the resource is not compliant.
  name: ViolationReason
  type: string
- description: AWS resource type.
  name: ResourceType
  type: string
provider_name: Amazon Firewall Manager
provider_slug: amazon-firewall-manager
schema_file: json-schema/amazon-firewall-manager-compliance-violator-schema.json
slug: amazon-firewall-manager-compliance-violator
source_filename: amazon-firewall-manager-compliance-violator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-firewall-manager/refs/heads/main/json-schema/amazon-firewall-manager-compliance-violator-schema.json\",\n  \"title\": \"ComplianceViolator\",\n  \"description\": \"A resource not in compliance with a Firewall Manager policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the non-compliant resource.\"\n    },\n    \"ViolationReason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason the resource is not compliant.\"\n    },\n    \"ResourceType\": {\n      \"type\": \"string\",\n      \"description\": \"AWS resource type.\"\n    }\n  },\n  \"required\": []\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-firewall-manager/refs/heads/main/json-schema/amazon-firewall-manager-compliance-violator-schema.json
tags:
- Compliance
- Firewall
- Network Security
- Security
title: ComplianceViolator
---
