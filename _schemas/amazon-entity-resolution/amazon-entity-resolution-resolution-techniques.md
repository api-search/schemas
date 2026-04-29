---
description: An object which defines the <code>resolutionType</code> and the <code>ruleBasedProperties</code>
layout: schema
name: ResolutionTechniques
properties_list:
- description: ''
  name: resolutionType
  type: object
- description: ''
  name: ruleBasedProperties
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-resolution-techniques-schema.json
slug: amazon-entity-resolution-resolution-techniques
source_filename: amazon-entity-resolution-resolution-techniques-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-resolution-techniques-schema.json\",\n  \"title\": \"ResolutionTechniques\",\n  \"description\": \"An object which defines the <code>resolutionType</code> and the <code>ruleBasedProperties</code> \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resolutionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolutionType\"\n        },\n        {\n          \"description\": \"There are two types of matching, <code>RULE_MATCHING</code> and <code>ML_MATCHING</code> \"\n        }\n      ]\n    },\n    \"ruleBasedProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleBasedProperties\"\n        },\n        {\n          \"description\": \"An object which defines the list of matching rules to run and\
  \ has a field <code>Rules</code>, which is a list of rule objects.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-resolution-techniques-schema.json
tags:
- Amazon Web Services
- AWS
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: ResolutionTechniques
---
