---
description: GetFindingsFilterResponse schema from Amazon Macie API
layout: schema
name: GetFindingsFilterResponse
properties_list:
- description: ''
  name: action
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: findingCriteria
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: position
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-findings-filter-response-schema.json
slug: amazon-macie-get-findings-filter-response
source_filename: amazon-macie-get-findings-filter-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-findings-filter-response-schema.json\",\n  \"title\": \"GetFindingsFilterResponse\",\n  \"description\": \"GetFindingsFilterResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingsFilterAction\"\n        },\n        {\n          \"description\": \"The action that's performed on findings that match the filter criteria (findingCriteria). Possible values are: ARCHIVE, suppress (automatically archive) the findings; and, NOOP, don't perform any action on the findings.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource\
  \ Name (ARN) of the filter.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom description of the filter.\"\n        }\n      ]\n    },\n    \"findingCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingCriteria\"\n        },\n        {\n          \"description\": \"The criteria that's used to filter findings.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the filter.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom name of the filter.\"\n        }\n      ]\n    },\n    \"position\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The position of the filter in the list of saved filters on the Amazon Macie console. This value also determines the order in which the filter is applied to findings, relative to other filters that are also applied to the findings.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A map of key-value pairs that specifies which tags (keys and values) are associated with the filter.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-findings-filter-response-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetFindingsFilterResponse
---
