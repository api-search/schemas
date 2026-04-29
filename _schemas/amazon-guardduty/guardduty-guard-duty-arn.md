---
description: GuardDutyArn schema from Amazon GuardDuty API
layout: schema
name: GuardDutyArn
properties_list: []
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-guard-duty-arn-schema.json
slug: guardduty-guard-duty-arn
source_filename: guardduty-guard-duty-arn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-guard-duty-arn-schema.json\",\n  \"title\": \"GuardDutyArn\",\n  \"description\": \"GuardDutyArn schema from Amazon GuardDuty API\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:[A-Za-z_.-]{1,20}:guardduty:[A-Za-z0-9_/.-]{0,63}:\\\\d+:detector/[A-Za-z0-9_/.-]{32,264}$\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-guard-duty-arn-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: GuardDutyArn
---
