---
description: A global property definition for classifying targets.
layout: schema
name: GlobalTargetProperty
properties_list:
- description: Unique identifier for the property.
  name: globalTargetPropertyId
  type: string
- description: Name of the property.
  name: propertyName
  type: string
- description: Human-readable display name.
  name: propertyDisplayName
  type: string
- description: Description of the property.
  name: description
  type: string
- description: Data type of the property.
  name: propertyType
  type: string
- description: Whether the property has a constrained value set.
  name: hasValidValues
  type: boolean
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-global-target-property-schema.json
slug: oracle-enterprise-manager-cloud-control-global-target-property
source_filename: oracle-enterprise-manager-cloud-control-global-target-property-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GlobalTargetProperty\",\n  \"type\": \"object\",\n  \"description\": \"A global property definition for classifying targets.\",\n  \"properties\": {\n    \"globalTargetPropertyId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the property.\"\n    },\n    \"propertyName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the property.\"\n    },\n    \"propertyDisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the property.\"\n    },\n    \"propertyType\": {\n      \"type\": \"string\",\n      \"description\": \"Data type of the property.\"\n    },\n    \"hasValidValues\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the property has a constrained value set.\"\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-global-target-property-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: GlobalTargetProperty
---
