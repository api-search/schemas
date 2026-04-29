---
description: SsmParameters schema
layout: schema
name: SsmParameters
properties_list: []
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-ssm-parameters-schema.json
slug: incident-manager-ssm-parameters
source_filename: incident-manager-ssm-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-ssm-parameters-schema.json\",\n  \"title\": \"SsmParameters\",\n  \"description\": \"SsmParameters schema\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"array\",\n    \"items\": {\n      \"$ref\": \"#/components/schemas/SsmParameterValuesMemberString\"\n    },\n    \"minItems\": 0,\n    \"maxItems\": 100\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-ssm-parameters-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: SsmParameters
---
