---
description: Provides quota and aggregated usage data for an Amazon Macie account.
layout: schema
name: UsageRecord
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: automatedDiscoveryFreeTrialStartDate
  type: object
- description: ''
  name: freeTrialStartDate
  type: object
- description: ''
  name: usage
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-usage-record-schema.json
slug: amazon-macie-usage-record
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-usage-record-schema.json\",\n  \"title\": \"UsageRecord\",\n  \"description\": \"Provides quota and aggregated usage data for an Amazon Macie account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the Amazon Web Services account that the data applies to.\"\n        }\n      ]\n    },\n    \"automatedDiscoveryFreeTrialStartDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when the free trial of automated sensitive data discovery started for the\
  \ account. If the account is a member account in an organization, this value is the same as the value for the organization's Amazon Macie administrator account.\"\n        }\n      ]\n    },\n    \"freeTrialStartDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when the Amazon Macie free trial started for the account.\"\n        }\n      ]\n    },\n    \"usage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfUsageByAccount\"\n        },\n        {\n          \"description\": \"An array of objects that contains usage data and quotas for the account. Each object contains the data for a specific usage metric and the corresponding quota.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-usage-record-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: UsageRecord
---
