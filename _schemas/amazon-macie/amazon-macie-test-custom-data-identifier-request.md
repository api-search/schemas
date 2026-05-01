---
description: TestCustomDataIdentifierRequest schema from Amazon Macie API
layout: schema
name: TestCustomDataIdentifierRequest
properties_list:
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
  name: regex
  type: object
- description: ''
  name: sampleText
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-test-custom-data-identifier-request-schema.json
slug: amazon-macie-test-custom-data-identifier-request
source_filename: amazon-macie-test-custom-data-identifier-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-test-custom-data-identifier-request-schema.json\",\n  \"title\": \"TestCustomDataIdentifierRequest\",\n  \"description\": \"TestCustomDataIdentifierRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ignoreWords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"An array that lists specific character sequences (<i>ignore words</i>) to exclude from the results. If the text matched by the regular expression contains any string in this array, Amazon Macie ignores it. The array can contain as many as 10 ignore words. Each ignore word can contain 4-90 UTF-8 characters. Ignore words are case sensitive.\"\n        }\n      ]\n    },\n    \"keywords\": {\n    \
  \  \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"An array that lists specific character sequences (<i>keywords</i>), one of which must precede and be within proximity (maximumMatchDistance) of the regular expression to match. The array can contain as many as 50 keywords. Each keyword can contain 3-90 UTF-8 characters. Keywords aren't case sensitive.\"\n        }\n      ]\n    },\n    \"maximumMatchDistance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The maximum number of characters that can exist between the end of at least one complete character sequence specified by the keywords array and the end of the text that matches the regex pattern. If a complete keyword precedes all the text that matches the pattern and the keyword is within the specified distance, Amazon Macie includes the result. The\
  \ distance can be 1-300 characters. The default value is 50.\"\n        }\n      ]\n    },\n    \"regex\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The regular expression (<i>regex</i>) that defines the pattern to match. The expression can contain as many as 512 characters.\"\n        }\n      ]\n    },\n    \"sampleText\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The sample text to inspect by using the custom data identifier. The text can contain as many as 1,000 characters.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"regex\",\n    \"sampleText\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-test-custom-data-identifier-request-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: TestCustomDataIdentifierRequest
---
