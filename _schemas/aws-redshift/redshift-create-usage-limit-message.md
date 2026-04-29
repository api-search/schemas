---
description: CreateUsageLimitMessage schema from Amazon Redshift
layout: schema
name: CreateUsageLimitMessage
properties_list:
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: FeatureType
  type: object
- description: ''
  name: LimitType
  type: object
- description: ''
  name: Amount
  type: object
- description: ''
  name: Period
  type: object
- description: ''
  name: BreachAction
  type: object
- description: ''
  name: Tags
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-create-usage-limit-message-schema.json
slug: redshift-create-usage-limit-message
source_filename: redshift-create-usage-limit-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {},\n    \"FeatureType\": {},\n    \"LimitType\": {},\n    \"Amount\": {},\n    \"Period\": {},\n    \"BreachAction\": {},\n    \"Tags\": {}\n  },\n  \"required\": [\n    \"ClusterIdentifier\",\n    \"FeatureType\",\n    \"LimitType\",\n    \"Amount\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-usage-limit-message-schema.json\",\n  \"title\": \"CreateUsageLimitMessage\",\n  \"description\": \"CreateUsageLimitMessage schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-usage-limit-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: CreateUsageLimitMessage
---
