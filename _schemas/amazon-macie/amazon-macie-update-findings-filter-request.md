---
description: UpdateFindingsFilterRequest schema from Amazon Macie API
layout: schema
name: UpdateFindingsFilterRequest
properties_list:
- description: ''
  name: action
  type: object
- description: ''
  name: clientToken
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: findingCriteria
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: position
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-update-findings-filter-request-schema.json
slug: amazon-macie-update-findings-filter-request
source_filename: amazon-macie-update-findings-filter-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-findings-filter-request-schema.json\",\n  \"title\": \"UpdateFindingsFilterRequest\",\n  \"description\": \"UpdateFindingsFilterRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingsFilterAction\"\n        },\n        {\n          \"description\": \"The action to perform on findings that match the filter criteria (findingCriteria). Valid values are: ARCHIVE, suppress (automatically archive) the findings; and, NOOP, don't perform any action on the findings.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A unique,\
  \ case-sensitive token that you provide to ensure the idempotency of the request.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>A custom description of the filter. The description can contain as many as 512 characters.</p> <p>We strongly recommend that you avoid including any sensitive data in the description of a filter. Other users of your account might be able to see this description, depending on the actions that they're allowed to perform in Amazon Macie.</p>\"\n        }\n      ]\n    },\n    \"findingCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingCriteria\"\n        },\n        {\n          \"description\": \"The criteria to use to filter findings.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n  \
  \      },\n        {\n          \"description\": \"<p>A custom name for the filter. The name must contain at least 3 characters and can contain as many as 64 characters.</p> <p>We strongly recommend that you avoid including any sensitive data in the name of a filter. Other users of your account might be able to see this name, depending on the actions that they're allowed to perform in Amazon Macie.</p>\"\n        }\n      ]\n    },\n    \"position\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The position of the filter in the list of saved filters on the Amazon Macie console. This value also determines the order in which the filter is applied to findings, relative to other filters that are also applied to the findings.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-findings-filter-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: UpdateFindingsFilterRequest
---
