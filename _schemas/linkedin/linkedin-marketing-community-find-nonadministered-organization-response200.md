---
description: FindNonadministeredOrganizationResponse200 from LinkedIn API
layout: schema
name: FindNonadministeredOrganizationResponse200
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
schema_file: json-schema/linkedin-marketing-community-find-nonadministered-organization-response200-schema.json
slug: linkedin-marketing-community-find-nonadministered-organization-response200
source_filename: linkedin-marketing-community-find-nonadministered-organization-response200-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-community-find-nonadministered-organization-response200-schema.json\",\n  \"title\": \"FindNonadministeredOrganizationResponse200\",\n  \"description\": \"FindNonadministeredOrganizationResponse200 from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"3803\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"localized\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"en_US\": {\n                      \"type\": \"string\"\n                    }\n                  }\n                },\n                \"preferredLocale\"\
  : {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"country\": {\n                      \"type\": \"string\"\n                    },\n                    \"language\": {\n                      \"type\": \"string\"\n                    }\n                  }\n                }\n              }\n            },\n            \"primaryOrganizationType\": {\n              \"type\": \"string\"\n            },\n            \"vanityName\": {\n              \"type\": \"string\"\n            },\n            \"locations\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"staffCountRange\": {\n                    \"type\": \"string\"\n                  },\n                  \"locationType\": {\n                    \"type\": \"string\"\n                  },\n                  \"address\": {\n                    \"type\": \"object\",\n  \
  \                  \"properties\": {\n                      \"country\": {\n                        \"type\": \"string\"\n                      }\n                    }\n                  }\n                }\n              }\n            },\n            \"localizedName\": {\n              \"type\": \"string\"\n            },\n            \"id\": {\n              \"type\": \"integer\"\n            }\n          }\n        },\n        \"79988552\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"localized\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"en_US\": {\n                      \"type\": \"string\"\n                    }\n                  }\n                },\n                \"preferredLocale\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                \
  \    \"country\": {\n                      \"type\": \"string\"\n                    },\n                    \"language\": {\n                      \"type\": \"string\"\n                    }\n                  }\n                }\n              }\n            },\n            \"primaryOrganizationType\": {\n              \"type\": \"string\"\n            },\n            \"vanityName\": {\n              \"type\": \"string\"\n            },\n            \"locations\": {\n              \"type\": \"array\",\n              \"items\": {}\n            },\n            \"localizedName\": {\n              \"type\": \"string\"\n            },\n            \"id\": {\n              \"type\": \"integer\"\n            }\n          }\n        }\n      }\n    },\n    \"statuses\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"3803\": {\n          \"type\": \"integer\"\n        },\n        \"79988552\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"errors\"\
  : {\n      \"type\": \"object\",\n      \"properties\": {}\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-community-find-nonadministered-organization-response200-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: FindNonadministeredOrganizationResponse200
---
