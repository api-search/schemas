---
description: CampaignList schema
layout: schema
name: CampaignList
properties_list:
- description: ''
  name: campaigns
  type: array
- description: ''
  name: totalCount
  type: integer
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/journey-optimizer-api-campaign-list-schema.json
slug: journey-optimizer-api-campaign-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/journey-optimizer-api-campaign-list-schema.json\",\n  \"title\": \"CampaignList\",\n  \"description\": \"CampaignList schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"campaigns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"description\": {\n            \"type\": \"string\"\n          },\n          \"channel\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"email\",\n              \"push\",\n              \"sms\",\n              \"inApp\"\n            ]\n          },\n          \"status\": {\n            \"type\": \"string\",\n         \
  \   \"enum\": [\n              \"draft\",\n              \"scheduled\",\n              \"live\",\n              \"completed\"\n            ]\n          },\n          \"schedule\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"startDate\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\"\n              },\n              \"endDate\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/journey-optimizer-api-campaign-list-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: CampaignList
---
