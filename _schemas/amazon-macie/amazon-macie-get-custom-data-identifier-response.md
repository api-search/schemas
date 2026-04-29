---
description: GetCustomDataIdentifierResponse schema from Amazon Macie API
layout: schema
name: GetCustomDataIdentifierResponse
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: deleted
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: ignoreWords
  type: object
- description: ''
  name: keywords
  type: object
- description: ''
  name: maximumMatchDistance
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: regex
  type: object
- description: ''
  name: severityLevels
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-custom-data-identifier-response-schema.json
slug: amazon-macie-get-custom-data-identifier-response
source_filename: amazon-macie-get-custom-data-identifier-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-custom-data-identifier-response-schema.json\",\n  \"title\": \"GetCustomDataIdentifierResponse\",\n  \"description\": \"GetCustomDataIdentifierResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the custom data identifier.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when the custom data identifier was created.\"\n        }\n      ]\n    },\n    \"deleted\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the custom data identifier was deleted. If you delete a custom data identifier, Amazon Macie doesn't delete it permanently. Instead, it soft deletes the identifier.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom description of the custom data identifier.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the custom data identifier.\"\n        }\n      ]\n    },\n    \"ignoreWords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\"\
  : \"An array that lists specific character sequences (<i>ignore words</i>) to exclude from the results. If the text matched by the regular expression contains any string in this array, Amazon Macie ignores it. Ignore words are case sensitive.\"\n        }\n      ]\n    },\n    \"keywords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"An array that lists specific character sequences (<i>keywords</i>), one of which must precede and be within proximity (maximumMatchDistance) of the regular expression to match. Keywords aren't case sensitive.\"\n        }\n      ]\n    },\n    \"maximumMatchDistance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The maximum number of characters that can exist between the end of at least one complete character sequence specified by the keywords array and the\
  \ end of the text that matches the regex pattern. If a complete keyword precedes all the text that matches the pattern and the keyword is within the specified distance, Amazon Macie includes the result. Otherwise, Macie excludes the result.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom name of the custom data identifier.\"\n        }\n      ]\n    },\n    \"regex\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The regular expression (<i>regex</i>) that defines the pattern to match.\"\n        }\n      ]\n    },\n    \"severityLevels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SeverityLevelList\"\n        },\n        {\n          \"description\": \"Specifies the severity that's assigned to findings that the custom\
  \ data identifier produces, based on the number of occurrences of text that matches the custom data identifier's detection criteria. By default, Amazon Macie creates findings for S3 objects that contain at least one occurrence of text that matches the detection criteria, and Macie assigns the MEDIUM severity to those findings.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A map of key-value pairs that identifies the tags (keys and values) that are associated with the custom data identifier.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-custom-data-identifier-response-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetCustomDataIdentifierResponse
---
