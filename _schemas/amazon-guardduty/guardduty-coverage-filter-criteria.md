---
description: Represents the criteria used in the filter.
layout: schema
name: CoverageFilterCriteria
properties_list:
- description: ''
  name: FilterCriterion
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-coverage-filter-criteria-schema.json
slug: guardduty-coverage-filter-criteria
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-coverage-filter-criteria-schema.json\",\n  \"title\": \"CoverageFilterCriteria\",\n  \"description\": \"Represents the criteria used in the filter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FilterCriterion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageFilterCriterionList\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"filterCriterion\"\n          },\n          \"description\": \"Represents a condition that when matched will be added to the response of the operation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-coverage-filter-criteria-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: CoverageFilterCriteria
---
