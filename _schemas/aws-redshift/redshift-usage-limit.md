---
description: Describes a usage limit object for a cluster.
layout: schema
name: UsageLimit
properties_list:
- description: ''
  name: UsageLimitId
  type: object
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
schema_file: json-schema/redshift-usage-limit-schema.json
slug: redshift-usage-limit
source_filename: redshift-usage-limit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UsageLimitId\": {},\n    \"ClusterIdentifier\": {},\n    \"FeatureType\": {},\n    \"LimitType\": {},\n    \"Amount\": {},\n    \"Period\": {},\n    \"BreachAction\": {},\n    \"Tags\": {}\n  },\n  \"description\": \"Describes a usage limit object for a cluster. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-usage-limit-schema.json\",\n  \"title\": \"UsageLimit\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-usage-limit-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: UsageLimit
---
