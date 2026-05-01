---
description: Specifies the type of security service and its configuration for a Firewall Manager policy.
layout: schema
name: SecurityServicePolicyData
properties_list:
- description: The service type.
  name: Type
  type: string
- description: Service-specific configuration details as JSON.
  name: ManagedServiceData
  type: string
provider_name: Amazon Firewall Manager
provider_slug: amazon-firewall-manager
schema_file: json-schema/amazon-firewall-manager-security-service-policy-data-schema.json
slug: amazon-firewall-manager-security-service-policy-data
source_filename: amazon-firewall-manager-security-service-policy-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-firewall-manager/refs/heads/main/json-schema/amazon-firewall-manager-security-service-policy-data-schema.json\",\n  \"title\": \"SecurityServicePolicyData\",\n  \"description\": \"Specifies the type of security service and its configuration for a Firewall Manager policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"WAF\",\n        \"WAFV2\",\n        \"SHIELD_ADVANCED\",\n        \"SECURITY_GROUPS_COMMON\",\n        \"SECURITY_GROUPS_CONTENT_AUDIT\",\n        \"SECURITY_GROUPS_USAGE_AUDIT\",\n        \"NETWORK_FIREWALL\",\n        \"DNS_FIREWALL\",\n        \"THIRD_PARTY_FIREWALL\",\n        \"IMPORT_NETWORK_FIREWALL\"\n      ],\n      \"description\": \"The service type.\"\n    },\n    \"ManagedServiceData\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Service-specific configuration details as JSON.\"\n    }\n  },\n  \"required\": [\n    \"Type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-firewall-manager/refs/heads/main/json-schema/amazon-firewall-manager-security-service-policy-data-schema.json
tags:
- Compliance
- Firewall
- Network Security
- Security
title: SecurityServicePolicyData
---
