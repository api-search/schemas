---
description: BatchGetOnAdministeredResponse200 from LinkedIn API
layout: schema
name: BatchGetOnAdministeredResponse200
properties_list:
- description: ''
  name: results
  type: object
- description: ''
  name: statuses
  type: object
- description: ''
  name: errors
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-community-batch-get-on-administered-response200-schema.json
slug: linkedin-marketing-community-batch-get-on-administered-response200
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-community-batch-get-on-administered-response200-schema.json\",\n  \"title\": \"BatchGetOnAdministeredResponse200\",\n  \"description\": \"BatchGetOnAdministeredResponse200 from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"89758488\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"vanityName\": {\n              \"type\": \"string\"\n            },\n            \"localizedName\": {\n              \"type\": \"string\"\n            },\n            \"website\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"localized\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"\
  en_US\": {\n                      \"type\": \"string\"\n                    }\n                  }\n                },\n                \"preferredLocale\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"country\": {\n                      \"type\": \"string\"\n                    },\n                    \"language\": {\n                      \"type\": \"string\"\n                    }\n                  }\n                }\n              }\n            },\n            \"groups\": {\n              \"type\": \"array\",\n              \"items\": {}\n            },\n            \"versionTag\": {\n              \"type\": \"string\"\n            },\n            \"defaultLocale\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"country\": {\n                  \"type\": \"string\"\n                },\n                \"language\": {\n                  \"type\": \"string\"\n                }\n \
  \             }\n            },\n            \"alternativeNames\": {\n              \"type\": \"array\",\n              \"items\": {}\n            },\n            \"specialties\": {\n              \"type\": \"array\",\n              \"items\": {}\n            },\n            \"parentRelationship\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"relationshipStatus\": {\n                  \"type\": \"string\"\n                },\n                \"parent\": {\n                  \"type\": \"string\"\n                }\n              }\n            },\n            \"localizedSpecialties\": {\n              \"type\": \"array\",\n              \"items\": {}\n            },\n            \"industries\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"name\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"\
  localized\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"en_US\": {\n                      \"type\": \"string\"\n                    }\n                  }\n                },\n                \"preferredLocale\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"country\": {\n                      \"type\": \"string\"\n                    },\n                    \"language\": {\n                      \"type\": \"string\"\n                    }\n                  }\n                }\n              }\n            },\n            \"primaryOrganizationType\": {\n              \"type\": \"string\"\n            },\n            \"id\": {\n              \"type\": \"integer\"\n            },\n            \"autoCreated\": {\n              \"type\": \"boolean\"\n            },\n            \"localizedWebsite\": {\n              \"type\": \"string\"\n            }\n          }\n      \
  \  }\n      }\n    },\n    \"statuses\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"35625943\": {\n          \"type\": \"integer\"\n        },\n        \"89758488\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"errors\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"35625943\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"message\": {\n              \"type\": \"string\"\n            },\n            \"status\": {\n              \"type\": \"integer\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-community-batch-get-on-administered-response200-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: BatchGetOnAdministeredResponse200
---
