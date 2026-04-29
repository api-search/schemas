---
description: UsageLimits schema from Amazon Redshift
layout: schema
name: UsageLimits
properties_list: []
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-usage-limits-schema.json
slug: redshift-usage-limits
source_filename: redshift-usage-limits-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"UsageLimitId\": {},\n      \"ClusterIdentifier\": {},\n      \"FeatureType\": {},\n      \"LimitType\": {},\n      \"Amount\": {},\n      \"Period\": {},\n      \"BreachAction\": {},\n      \"Tags\": {}\n    },\n    \"description\": \"Describes a usage limit object for a cluster. \"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-usage-limits-schema.json\",\n  \"title\": \"UsageLimits\",\n  \"description\": \"UsageLimits schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-usage-limits-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: UsageLimits
---
