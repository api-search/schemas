---
description: SecurityGroups schema from Amazon GuardDuty API
layout: schema
name: SecurityGroups
properties_list: []
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-security-groups-schema.json
slug: guardduty-security-groups
source_filename: guardduty-security-groups-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-security-groups-schema.json\",\n  \"title\": \"SecurityGroups\",\n  \"description\": \"SecurityGroups schema from Amazon GuardDuty API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/SecurityGroup\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-security-groups-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: SecurityGroups
---
