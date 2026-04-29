---
description: ModifyUsageLimitMessage schema from Amazon Redshift
layout: schema
name: ModifyUsageLimitMessage
properties_list:
- description: ''
  name: UsageLimitId
  type: object
- description: ''
  name: Amount
  type: object
- description: ''
  name: BreachAction
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-modify-usage-limit-message-schema.json
slug: redshift-modify-usage-limit-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UsageLimitId\": {},\n    \"Amount\": {},\n    \"BreachAction\": {}\n  },\n  \"required\": [\n    \"UsageLimitId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-usage-limit-message-schema.json\",\n  \"title\": \"ModifyUsageLimitMessage\",\n  \"description\": \"ModifyUsageLimitMessage schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-usage-limit-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ModifyUsageLimitMessage
---
