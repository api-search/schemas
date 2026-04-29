---
description: Represents the criteria to be used in the filter for describing scan entries.
layout: schema
name: FilterCriteria
properties_list:
- description: ''
  name: FilterCriterion
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-filter-criteria-schema.json
slug: guardduty-filter-criteria
source_filename: guardduty-filter-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-filter-criteria-schema.json\",\n  \"title\": \"FilterCriteria\",\n  \"description\": \"Represents the criteria to be used in the filter for describing scan entries.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FilterCriterion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterCriterionList\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"filterCriterion\"\n          },\n          \"description\": \"Represents a condition that when matched will be added to the response of the operation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-filter-criteria-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: FilterCriteria
---
