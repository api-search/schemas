---
description: Request body for searching contacts with filter criteria
layout: schema
name: ContactSearchRequest
properties_list:
- description: Root condition set for the search
  name: conditionSet
  type: object
- description: Attributes to include in the search results
  name: returnAttributes
  type: array
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-contact-search-request-schema.json
slug: salesforce-marketing-cloud-contact-search-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContactSearchRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for searching contacts with filter criteria\",\n  \"properties\": {\n    \"conditionSet\": {\n      \"type\": \"object\",\n      \"description\": \"Root condition set for the search\"\n    },\n    \"returnAttributes\": {\n      \"type\": \"array\",\n      \"description\": \"Attributes to include in the search results\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-contact-search-request-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: ContactSearchRequest
---
