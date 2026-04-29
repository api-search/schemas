---
description: Represents a condition that when matched will be added to the response of the operation. Irrespective of using any filter criteria, an administrator account can view the scan entries for all of its member accounts. However, each member account can view the scan entries only for their own account.
layout: schema
name: FilterCriterion
properties_list:
- description: ''
  name: CriterionKey
  type: object
- description: ''
  name: FilterCondition
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-filter-criterion-schema.json
slug: guardduty-filter-criterion
source_filename: guardduty-filter-criterion-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-filter-criterion-schema.json\",\n  \"title\": \"FilterCriterion\",\n  \"description\": \"Represents a condition that when matched will be added to the response of the operation. Irrespective of using any filter criteria, an administrator account can view the scan entries for all of its member accounts. However, each member account can view the scan entries only for their own account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CriterionKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CriterionKey\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"criterionKey\"\n          },\n          \"description\": \"An enum value representing possible scan properties to match with given scan entries.\"\n        }\n      ]\n    },\n    \"\
  FilterCondition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterCondition\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"filterCondition\"\n          },\n          \"description\": \"Contains information about the condition.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-filter-criterion-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: FilterCriterion
---
