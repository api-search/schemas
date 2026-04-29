---
description: Ranger security policy definition
layout: schema
name: Policy
properties_list:
- description: Policy identifier
  name: id
  type: integer
- description: Policy name
  name: name
  type: string
- description: Service type this policy applies to (hdfs, hive, hbase)
  name: serviceType
  type: string
- description: Service name this policy applies to
  name: serviceName
  type: string
- description: Policy description
  name: description
  type: string
- description: Whether the policy is active
  name: isEnabled
  type: boolean
- description: Whether audit logging is enabled
  name: isAuditEnabled
  type: boolean
- description: Resources protected by this policy
  name: resources
  type: object
- description: ''
  name: policyItems
  type: array
provider_name: Apache Ranger
provider_slug: apache-ranger
schema_file: json-schema/apache-ranger-policy-schema.json
slug: apache-ranger-policy
source_filename: apache-ranger-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-policy-schema.json\",\n  \"title\": \"Policy\",\n  \"description\": \"Ranger security policy definition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Policy identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Policy name\"\n    },\n    \"serviceType\": {\n      \"type\": \"string\",\n      \"description\": \"Service type this policy applies to (hdfs, hive, hbase)\"\n    },\n    \"serviceName\": {\n      \"type\": \"string\",\n      \"description\": \"Service name this policy applies to\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Policy description\"\n    },\n    \"isEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"\
  Whether the policy is active\"\n    },\n    \"isAuditEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether audit logging is enabled\"\n    },\n    \"resources\": {\n      \"type\": \"object\",\n      \"description\": \"Resources protected by this policy\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/PolicyResource\"\n      }\n    },\n    \"policyItems\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PolicyItem\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-policy-schema.json
tags:
- Access Control
- Authorization
- Hadoop
- Policy Management
- Security
- Apache
- Open Source
title: Policy
---
