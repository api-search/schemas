---
description: Contains information about the criteria used for querying findings.
layout: schema
name: FindingCriteria
properties_list:
- description: ''
  name: Criterion
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-finding-criteria-schema.json
slug: guardduty-finding-criteria
source_filename: guardduty-finding-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-finding-criteria-schema.json\",\n  \"title\": \"FindingCriteria\",\n  \"description\": \"Contains information about the criteria used for querying findings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Criterion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Criterion\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"criterion\"\n          },\n          \"description\": \"Represents a map of finding properties that match specified conditions and values when querying findings.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-finding-criteria-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: FindingCriteria
---
