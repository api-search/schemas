---
description: <p/>
layout: schema
name: ModifyEventSubscriptionMessage
properties_list:
- description: ''
  name: SubscriptionName
  type: object
- description: ''
  name: SnsTopicArn
  type: object
- description: ''
  name: SourceType
  type: object
- description: ''
  name: SourceIds
  type: object
- description: ''
  name: EventCategories
  type: object
- description: ''
  name: Severity
  type: object
- description: ''
  name: Enabled
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-modify-event-subscription-message-schema.json
slug: redshift-modify-event-subscription-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SubscriptionName\": {},\n    \"SnsTopicArn\": {},\n    \"SourceType\": {},\n    \"SourceIds\": {},\n    \"EventCategories\": {},\n    \"Severity\": {},\n    \"Enabled\": {}\n  },\n  \"required\": [\n    \"SubscriptionName\"\n  ],\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-event-subscription-message-schema.json\",\n  \"title\": \"ModifyEventSubscriptionMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-event-subscription-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ModifyEventSubscriptionMessage
---
