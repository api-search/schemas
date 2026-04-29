---
description: FetchFullLeadDataResponse200 from LinkedIn API
layout: schema
name: FetchFullLeadDataResponse200
properties_list:
- description: ''
  name: owner
  type: object
- description: ''
  name: submitter
  type: string
- description: ''
  name: leadType
  type: string
- description: ''
  name: leadMetadata
  type: object
- description: ''
  name: versionedLeadGenFormUrn
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: submittedAt
  type: integer
- description: ''
  name: testLead
  type: boolean
- description: ''
  name: associatedEntity
  type: object
- description: ''
  name: formResponse
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-leads-fetch-full-lead-data-response200-schema.json
slug: linkedin-marketing-leads-fetch-full-lead-data-response200
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-leads-fetch-full-lead-data-response200-schema.json\",\n  \"title\": \"FetchFullLeadDataResponse200\",\n  \"description\": \"FetchFullLeadDataResponse200 from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"owner\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"sponsoredAccount\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"submitter\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"leadType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"leadMetadata\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"sponsoredLeadMetadata\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"campaign\": {\n             \
  \ \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"versionedLeadGenFormUrn\": {\n      \"type\": \"string\",\n      \"example\": \"urn:li:organization:123456\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"123456\"\n    },\n    \"submittedAt\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"testLead\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"associatedEntity\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"associatedCreative\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"formResponse\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"consentResponses\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"accepted\": {\n                \"type\": \"boolean\"\n              },\n              \"consentId\": {\n           \
  \     \"type\": \"integer\"\n              }\n            }\n          }\n        },\n        \"answers\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"answerDetails\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"textQuestionAnswer\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"answer\": {\n                        \"type\": \"string\"\n                      }\n                    }\n                  }\n                }\n              },\n              \"questionId\": {\n                \"type\": \"integer\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-leads-fetch-full-lead-data-response200-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: FetchFullLeadDataResponse200
---
