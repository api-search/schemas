---
description: FindAdministeredOrganizationBrandsResponse200 from LinkedIn API
layout: schema
name: FindAdministeredOrganizationBrandsResponse200
properties_list:
- description: ''
  name: paging
  type: object
- description: ''
  name: elements
  type: array
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-community-find-administered-organization-brands-response200-schema.json
slug: linkedin-marketing-community-find-administered-organization-brands-response200
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-community-find-administered-organization-brands-response200-schema.json\",\n  \"title\": \"FindAdministeredOrganizationBrandsResponse200\",\n  \"description\": \"FindAdministeredOrganizationBrandsResponse200 from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"paging\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"start\": {\n          \"type\": \"integer\"\n        },\n        \"count\": {\n          \"type\": \"integer\"\n        },\n        \"links\": {\n          \"type\": \"array\",\n          \"items\": {}\n        },\n        \"total\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"elements\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\"\
  : {\n            \"type\": \"object\",\n            \"properties\": {\n              \"localized\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"en_US\": {\n                    \"type\": \"string\"\n                  }\n                }\n              },\n              \"preferredLocale\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"country\": {\n                    \"type\": \"string\"\n                  },\n                  \"language\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          },\n          \"primaryOrganizationType\": {\n            \"type\": \"string\"\n          },\n          \"vanityName\": {\n            \"type\": \"string\"\n          },\n          \"locations\": {\n            \"type\": \"array\",\n            \"items\": {}\n          },\n          \"localizedName\": {\n            \"type\"\
  : \"string\"\n          },\n          \"id\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-community-find-administered-organization-brands-response200-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: FindAdministeredOrganizationBrandsResponse200
---
