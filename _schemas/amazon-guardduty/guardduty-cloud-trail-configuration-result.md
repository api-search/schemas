---
description: Contains information on the status of CloudTrail as a data source for the detector.
layout: schema
name: CloudTrailConfigurationResult
properties_list:
- description: ''
  name: Status
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-cloud-trail-configuration-result-schema.json
slug: guardduty-cloud-trail-configuration-result
source_filename: guardduty-cloud-trail-configuration-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-cloud-trail-configuration-result-schema.json\",\n  \"title\": \"CloudTrailConfigurationResult\",\n  \"description\": \"Contains information on the status of CloudTrail as a data source for the detector.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"Describes whether CloudTrail is enabled as a data source for the detector.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-cloud-trail-configuration-result-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: CloudTrailConfigurationResult
---
