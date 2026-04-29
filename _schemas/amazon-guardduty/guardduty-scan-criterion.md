---
description: Represents a map of resource properties that match specified conditions and values when triggering malware scans.
layout: schema
name: ScanCriterion
properties_list: []
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-scan-criterion-schema.json
slug: guardduty-scan-criterion
source_filename: guardduty-scan-criterion-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-criterion-schema.json\",\n  \"title\": \"ScanCriterion\",\n  \"description\": \"Represents a map of resource properties that match specified conditions and values when triggering malware scans.\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"$ref\": \"#/components/schemas/ScanCondition\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-criterion-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ScanCriterion
---
