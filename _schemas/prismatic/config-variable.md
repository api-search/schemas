---
description: A config variable defines a configurable parameter for an integration that can be set per-instance to customize behavior for each customer.
layout: schema
name: Prismatic Config Variable
properties_list:
- description: Unique identifier for the config variable
  name: id
  type: string
- description: Key used to reference the config variable
  name: key
  type: string
- description: Stable key that persists across integration versions
  name: stableKey
  type: string
- description: Description of the config variable
  name: description
  type: string
- description: Data type of the config variable
  name: dataType
  type: string
- description: Default value for the config variable
  name: defaultValue
  type: string
- description: Collection type if the config variable holds multiple values
  name: collectionType
  type: string
- description: List of options when dataType is picklist
  name: pickList
  type: array
- description: Whether the config variable is visible to customer users during deployment
  name: visibleToCustomerDeployer
  type: boolean
- description: Whether the config variable is visible to organization users during deployment
  name: visibleToOrgDeployer
  type: boolean
- description: Current value of the config variable for a specific instance
  name: value
  type: string
provider_name: Prismatic
provider_slug: prismatic
schema_file: json-schema/config-variable.json
slug: config-variable
source_filename: config-variable.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/json-schema/config-variable.json\",\n  \"title\": \"Prismatic Config Variable\",\n  \"description\": \"A config variable defines a configurable parameter for an integration that can be set per-instance to customize behavior for each customer.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"key\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the config variable\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Key used to reference the config variable\"\n    },\n    \"stableKey\": {\n      \"type\": \"string\",\n      \"description\": \"Stable key that persists across integration versions\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the config variable\"\n\
  \    },\n    \"dataType\": {\n      \"type\": \"string\",\n      \"enum\": [\"string\", \"date\", \"timestamp\", \"picklist\", \"schedule\", \"code\", \"boolean\", \"number\", \"objectSelection\", \"objectFieldMap\", \"jsonForm\", \"connection\"],\n      \"description\": \"Data type of the config variable\"\n    },\n    \"defaultValue\": {\n      \"type\": \"string\",\n      \"description\": \"Default value for the config variable\"\n    },\n    \"collectionType\": {\n      \"type\": \"string\",\n      \"enum\": [\"\", \"valuelist\", \"keyvaluelist\"],\n      \"description\": \"Collection type if the config variable holds multiple values\"\n    },\n    \"pickList\": {\n      \"type\": \"array\",\n      \"description\": \"List of options when dataType is picklist\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"visibleToCustomerDeployer\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the config variable is visible to customer users during\
  \ deployment\"\n    },\n    \"visibleToOrgDeployer\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the config variable is visible to organization users during deployment\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Current value of the config variable for a specific instance\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/json-schema/config-variable.json
tags:
- Embedded iPaaS
- Integrations
- Workflows
title: Prismatic Config Variable
---
