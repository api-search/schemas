---
description: DataSource schema from Amazon GuardDuty API
layout: schema
name: DataSource
properties_list: []
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-data-source-schema.json
slug: guardduty-data-source
source_filename: guardduty-data-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-data-source-schema.json\",\n  \"title\": \"DataSource\",\n  \"description\": \"DataSource schema from Amazon GuardDuty API\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"FLOW_LOGS\",\n    \"CLOUD_TRAIL\",\n    \"DNS_LOGS\",\n    \"S3_LOGS\",\n    \"KUBERNETES_AUDIT_LOGS\",\n    \"EC2_MALWARE_SCAN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-data-source-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: DataSource
---
