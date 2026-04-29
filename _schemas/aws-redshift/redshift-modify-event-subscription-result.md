---
description: ModifyEventSubscriptionResult schema from Amazon Redshift
layout: schema
name: ModifyEventSubscriptionResult
properties_list:
- description: Describes event subscriptions.
  name: EventSubscription
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-modify-event-subscription-result-schema.json
slug: redshift-modify-event-subscription-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"EventSubscription\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"CustomerAwsId\": {},\n        \"CustSubscriptionId\": {},\n        \"SnsTopicArn\": {},\n        \"Status\": {},\n        \"SubscriptionCreationTime\": {},\n        \"SourceType\": {},\n        \"SourceIdsList\": {},\n        \"EventCategoriesList\": {},\n        \"Severity\": {},\n        \"Enabled\": {},\n        \"Tags\": {}\n      },\n      \"description\": \"Describes event subscriptions.\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-event-subscription-result-schema.json\",\n  \"title\": \"ModifyEventSubscriptionResult\",\n  \"description\": \"ModifyEventSubscriptionResult schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-modify-event-subscription-result-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ModifyEventSubscriptionResult
---
