---
description: Describes event subscriptions.
layout: schema
name: EventSubscription
properties_list:
- description: ''
  name: CustomerAwsId
  type: object
- description: ''
  name: CustSubscriptionId
  type: object
- description: ''
  name: SnsTopicArn
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: SubscriptionCreationTime
  type: object
- description: ''
  name: SourceType
  type: object
- description: ''
  name: SourceIdsList
  type: object
- description: ''
  name: EventCategoriesList
  type: object
- description: ''
  name: Severity
  type: object
- description: ''
  name: Enabled
  type: object
- description: ''
  name: Tags
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-event-subscription-schema.json
slug: redshift-event-subscription
source_filename: redshift-event-subscription-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"CustomerAwsId\": {},\n    \"CustSubscriptionId\": {},\n    \"SnsTopicArn\": {},\n    \"Status\": {},\n    \"SubscriptionCreationTime\": {},\n    \"SourceType\": {},\n    \"SourceIdsList\": {},\n    \"EventCategoriesList\": {},\n    \"Severity\": {},\n    \"Enabled\": {},\n    \"Tags\": {}\n  },\n  \"description\": \"Describes event subscriptions.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-event-subscription-schema.json\",\n  \"title\": \"EventSubscription\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-event-subscription-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: EventSubscription
---
