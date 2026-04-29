---
description: A configuration property of a target.
layout: schema
name: TargetProperty
properties_list:
- description: Property name.
  name: name
  type: string
- description: Property value.
  name: value
  type: string
- description: Whether the property is read-only.
  name: isReadOnly
  type: boolean
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-target-property-schema.json
slug: oracle-enterprise-manager-cloud-control-target-property
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TargetProperty\",\n  \"type\": \"object\",\n  \"description\": \"A configuration property of a target.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Property name.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Property value.\"\n    },\n    \"isReadOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the property is read-only.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-target-property-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: TargetProperty
---
