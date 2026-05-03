---
description: A security rule defines access control policies for Qlik Sense resources. Rules use a condition expression, resource filter, and action bitmask to control which users can perform which operations on which resources. Rules can apply in the QMC context, the Hub context, or both.
layout: schema
name: Qlik Sense Security Rule
properties_list:
- description: Unique identifier (GUID) assigned by the repository
  name: id
  type: string
- description: ISO 8601 timestamp when the rule was created
  name: createdDate
  type: string
- description: ISO 8601 timestamp when the rule was last modified
  name: modifiedDate
  type: string
- description: Username of the user who last modified the rule
  name: modifiedByUserName
  type: string
- description: Display name of the security rule
  name: name
  type: string
- description: Rule category (e.g., Security, Sync)
  name: category
  type: string
- description: Rule type identifier
  name: type
  type: integer
- description: Rule condition expression using Qlik Sense security rule syntax. Evaluates user and resource properties to determine access.
  name: rule
  type: string
- description: Resource filter expression defining which resources the rule applies to (e.g., App_*, Stream_*)
  name: resourceFilter
  type: string
- description: 'Bitwise combination of allowed actions: 1=Create, 2=Read, 4=Update, 8=Delete, 16=Export, 32=Publish, 64=ChangeOwner, 128=ChangeRole'
  name: actions
  type: integer
- description: Human-readable description or comment about the rule's purpose
  name: comment
  type: string
- description: Whether the rule is currently disabled
  name: disabled
  type: boolean
- description: Context in which the rule applies
  name: ruleContext
  type: integer
- description: Tags applied to the security rule
  name: tags
  type: array
- description: List of privileges the current user has on this rule
  name: privileges
  type: array
- description: Schema path identifying the entity type in the QRS
  name: schemaPath
  type: string
provider_name: Qlik Sense Enterprise
provider_slug: qlik-sense-enterprise
schema_file: json-schema/qlik-sense-enterprise-security-rule-schema.json
slug: qlik-sense-enterprise-security-rule
source_filename: qlik-sense-enterprise-security-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.api.dev/qlik-sense-enterprise/security-rule.json\",\n  \"title\": \"Qlik Sense Security Rule\",\n  \"description\": \"A security rule defines access control policies for Qlik Sense resources. Rules use a condition expression, resource filter, and action bitmask to control which users can perform which operations on which resources. Rules can apply in the QMC context, the Hub context, or both.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier (GUID) assigned by the repository\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the rule was created\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO\
  \ 8601 timestamp when the rule was last modified\"\n    },\n    \"modifiedByUserName\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the user who last modified the rule\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the security rule\",\n      \"minLength\": 1\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Rule category (e.g., Security, Sync)\"\n    },\n    \"type\": {\n      \"type\": \"integer\",\n      \"description\": \"Rule type identifier\"\n    },\n    \"rule\": {\n      \"type\": \"string\",\n      \"description\": \"Rule condition expression using Qlik Sense security rule syntax. Evaluates user and resource properties to determine access.\"\n    },\n    \"resourceFilter\": {\n      \"type\": \"string\",\n      \"description\": \"Resource filter expression defining which resources the rule applies to (e.g., App_*, Stream_*)\"\n    },\n    \"actions\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"Bitwise combination of allowed actions: 1=Create, 2=Read, 4=Update, 8=Delete, 16=Export, 32=Publish, 64=ChangeOwner, 128=ChangeRole\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description or comment about the rule's purpose\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the rule is currently disabled\",\n      \"default\": false\n    },\n    \"ruleContext\": {\n      \"type\": \"integer\",\n      \"description\": \"Context in which the rule applies\",\n      \"enum\": [0, 1, 2],\n      \"default\": 0\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TagReference\"\n      },\n      \"description\": \"Tags applied to the security rule\"\n    },\n    \"privileges\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of privileges\
  \ the current user has on this rule\"\n    },\n    \"schemaPath\": {\n      \"type\": \"string\",\n      \"description\": \"Schema path identifying the entity type in the QRS\"\n    }\n  },\n  \"required\": [\"name\", \"rule\", \"resourceFilter\", \"actions\"],\n  \"$defs\": {\n    \"TagReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/json-schema/qlik-sense-enterprise-security-rule-schema.json
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Enterprise
- REST API
title: Qlik Sense Security Rule
---
