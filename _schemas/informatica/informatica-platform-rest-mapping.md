---
description: Represents a data integration mapping definition that specifies data transformation logic between sources and targets.
layout: schema
name: Mapping
properties_list:
- description: The resource type identifier.
  name: '@type'
  type: string
- description: The unique identifier for the mapping.
  name: id
  type: string
- description: The organization ID that owns the mapping.
  name: orgId
  type: string
- description: The name of the mapping.
  name: name
  type: string
- description: A description of the mapping.
  name: description
  type: string
- description: The time the mapping was created.
  name: createTime
  type: string
- description: The time the mapping was last updated.
  name: updateTime
  type: string
- description: The user who created the mapping.
  name: createdBy
  type: string
- description: The user who last updated the mapping.
  name: updatedBy
  type: string
- description: The associated bundle ID if applicable.
  name: bundleObjectId
  type: string
- description: The associated bundle version.
  name: bundleVersion
  type: string
- description: The internal template identifier.
  name: templateId
  type: string
- description: The time the mapping was deployed.
  name: deployTime
  type: string
- description: Whether the mapping includes parameters.
  name: hasParameters
  type: boolean
- description: Whether the mapping is in a valid state.
  name: valid
  type: boolean
- description: Whether the mapping uses fixed connections.
  name: fixedConnection
  type: boolean
- description: Whether parameters are deployed.
  name: hasParametersDeployed
  type: boolean
- description: Whether fixed connections are deployed.
  name: fixedConnectionDeployed
  type: boolean
- description: The internal deployed template identifier.
  name: deployedTemplateId
  type: string
- description: The count of tasks using this mapping.
  name: tasks
  type: integer
- description: The collection of mapping parameters.
  name: parameters
  type: array
- description: The collection of in-out parameters.
  name: inOutParameters
  type: array
- description: References to related objects.
  name: references
  type: array
provider_name: Informatica
provider_slug: informatica
schema_file: json-schema/informatica-platform-rest-mapping-schema.json
slug: informatica-platform-rest-mapping
source_filename: informatica-platform-rest-mapping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Mapping\",\n  \"type\": \"object\",\n  \"description\": \"Represents a data integration mapping definition that specifies data transformation logic between sources and targets.\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type identifier.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the mapping.\"\n    },\n    \"orgId\": {\n      \"type\": \"string\",\n      \"description\": \"The organization ID that owns the mapping.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the mapping.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the mapping.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the mapping was created.\"\n   \
  \ },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the mapping was last updated.\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"The user who created the mapping.\"\n    },\n    \"updatedBy\": {\n      \"type\": \"string\",\n      \"description\": \"The user who last updated the mapping.\"\n    },\n    \"bundleObjectId\": {\n      \"type\": \"string\",\n      \"description\": \"The associated bundle ID if applicable.\"\n    },\n    \"bundleVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The associated bundle version.\"\n    },\n    \"templateId\": {\n      \"type\": \"string\",\n      \"description\": \"The internal template identifier.\"\n    },\n    \"deployTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the mapping was deployed.\"\n    },\n    \"hasParameters\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the mapping includes parameters.\"\
  \n    },\n    \"valid\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the mapping is in a valid state.\"\n    },\n    \"fixedConnection\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the mapping uses fixed connections.\"\n    },\n    \"hasParametersDeployed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether parameters are deployed.\"\n    },\n    \"fixedConnectionDeployed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether fixed connections are deployed.\"\n    },\n    \"deployedTemplateId\": {\n      \"type\": \"string\",\n      \"description\": \"The internal deployed template identifier.\"\n    },\n    \"tasks\": {\n      \"type\": \"integer\",\n      \"description\": \"The count of tasks using this mapping.\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"The collection of mapping parameters.\"\n    },\n    \"inOutParameters\": {\n      \"type\": \"array\",\n      \"\
  description\": \"The collection of in-out parameters.\"\n    },\n    \"references\": {\n      \"type\": \"array\",\n      \"description\": \"References to related objects.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/json-schema/informatica-platform-rest-mapping-schema.json
tags:
- Address Verification
- B2B Gateway
- Cloud Services
- Data Governance
- Data Integration
- Data Profiling
- Data Quality
- Enterprise Software
- ETL
- IDMC
- IICS
- Master Data Management
- Reference Data Management
title: Mapping
---
