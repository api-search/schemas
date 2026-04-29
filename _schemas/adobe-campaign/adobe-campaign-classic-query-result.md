---
description: SOAP response containing query result set as XML elements matching the target schema structure.
layout: schema
name: QueryResult
properties_list:
- description: Collection of result records matching the query criteria.
  name: resultSet
  type: object
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-classic-query-result-schema.json
slug: adobe-campaign-classic-query-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-query-result-schema.json\",\n  \"title\": \"QueryResult\",\n  \"description\": \"SOAP response containing query result set as XML elements matching the target schema structure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resultSet\": {\n      \"type\": \"object\",\n      \"description\": \"Collection of result records matching the query criteria.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-query-result-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: QueryResult
---
