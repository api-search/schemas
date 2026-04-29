---
description: Name of the parameter from the Review policy.
layout: schema
name: PolicyParameter
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: Values
  type: object
- description: ''
  name: MapEntries
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-policy-parameter-schema.json
slug: amazon-mechanical-turk-policy-parameter
source_filename: amazon-mechanical-turk-policy-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-policy-parameter-schema.json\",\n  \"title\": \"PolicyParameter\",\n  \"description\": \" Name of the parameter from the Review policy. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" Name of the parameter from the list of Review Polices. \"\n        }\n      ]\n    },\n    \"Values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \" The list of values of the Parameter\"\n        }\n      ]\n    },\n    \"MapEntries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ParameterMapEntryList\"\n      \
  \  },\n        {\n          \"description\": \" List of ParameterMapEntry objects. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-policy-parameter-schema.json
tags:
- AWS
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: PolicyParameter
---
