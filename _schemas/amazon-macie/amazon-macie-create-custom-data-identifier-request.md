---
description: CreateCustomDataIdentifierRequest schema from Amazon Macie API
layout: schema
name: CreateCustomDataIdentifierRequest
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: description
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
schema_file: json-schema/amazon-macie-create-custom-data-identifier-request-schema.json
slug: amazon-macie-create-custom-data-identifier-request
source_filename: amazon-macie-create-custom-data-identifier-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-create-custom-data-identifier-request-schema.json\",\n  \"title\": \"CreateCustomDataIdentifierRequest\",\n  \"description\": \"CreateCustomDataIdentifierRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A unique, case-sensitive token that you provide to ensure the idempotency of the request.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>A custom description of the custom data identifier. The description can contain as many as 512 characters.</p> <p>We\
  \ strongly recommend that you avoid including any sensitive data in the description of a custom data identifier. Other users of your account might be able to see this description, depending on the actions that they're allowed to perform in Amazon Macie.</p>\"\n        }\n      ]\n    },\n    \"ignoreWords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"An array that lists specific character sequences (<i>ignore words</i>) to exclude from the results. If the text matched by the regular expression contains any string in this array, Amazon Macie ignores it. The array can contain as many as 10 ignore words. Each ignore word can contain 4-90 UTF-8 characters. Ignore words are case sensitive.\"\n        }\n      ]\n    },\n    \"keywords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"description\": \"An\
  \ array that lists specific character sequences (<i>keywords</i>), one of which must precede and be within proximity (maximumMatchDistance) of the regular expression to match. The array can contain as many as 50 keywords. Each keyword can contain 3-90 UTF-8 characters. Keywords aren't case sensitive.\"\n        }\n      ]\n    },\n    \"maximumMatchDistance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The maximum number of characters that can exist between the end of at least one complete character sequence specified by the keywords array and the end of the text that matches the regex pattern. If a complete keyword precedes all the text that matches the pattern and the keyword is within the specified distance, Amazon Macie includes the result. The distance can be 1-300 characters. The default value is 50.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n   \
  \       \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>A custom name for the custom data identifier. The name can contain as many as 128 characters.</p> <p>We strongly recommend that you avoid including any sensitive data in the name of a custom data identifier. Other users of your account might be able to see this name, depending on the actions that they're allowed to perform in Amazon Macie.</p>\"\n        }\n      ]\n    },\n    \"regex\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The regular expression (<i>regex</i>) that defines the pattern to match. The expression can contain as many as 512 characters.\"\n        }\n      ]\n    },\n    \"severityLevels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SeverityLevelList\"\n        },\n        {\n          \"description\": \"<p>The severity to assign to\
  \ findings that the custom data identifier produces, based on the number of occurrences of text that matches the custom data identifier's detection criteria. You can specify as many as three SeverityLevel objects in this array, one for each severity: LOW, MEDIUM, or HIGH. If you specify more than one, the occurrences thresholds must be in ascending order by severity, moving from LOW to HIGH. For example, 1 for LOW, 50 for MEDIUM, and 100 for HIGH. If an S3 object contains fewer occurrences than the lowest specified threshold, Amazon Macie doesn't create a finding.</p> <p>If you don't specify any values for this array, Macie creates findings for S3 objects that contain at least one occurrence of text that matches the detection criteria, and Macie assigns the MEDIUM severity to those findings.</p>\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"<p>A map\
  \ of key-value pairs that specifies the tags to associate with the custom data identifier.</p> <p>A custom data identifier can have a maximum of 50 tags. Each tag consists of a tag key and an associated tag value. The maximum length of a tag key is 128 characters. The maximum length of a tag value is 256 characters.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"regex\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-create-custom-data-identifier-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: CreateCustomDataIdentifierRequest
---
