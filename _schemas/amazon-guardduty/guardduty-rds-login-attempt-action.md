---
description: Indicates that a login attempt was made to the potentially compromised database from a remote IP address.
layout: schema
name: RdsLoginAttemptAction
properties_list:
- description: ''
  name: RemoteIpDetails
  type: object
- description: ''
  name: LoginAttributes
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-rds-login-attempt-action-schema.json
slug: guardduty-rds-login-attempt-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-rds-login-attempt-action-schema.json\",\n  \"title\": \"RdsLoginAttemptAction\",\n  \"description\": \"Indicates that a login attempt was made to the potentially compromised database from a remote IP address.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RemoteIpDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemoteIpDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"remoteIpDetails\"\n          }\n        }\n      ]\n    },\n    \"LoginAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoginAttributes\"\n        },\n        {\n          \"description\": \"Indicates the login attributes used in the login attempt.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-rds-login-attempt-action-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: RdsLoginAttemptAction
---
