---
description: Describes the configuration of scanning EBS volumes as a data source.
layout: schema
name: EbsVolumesResult
properties_list:
- description: ''
  name: Status
  type: object
- description: ''
  name: Reason
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-ebs-volumes-result-schema.json
slug: guardduty-ebs-volumes-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-ebs-volumes-result-schema.json\",\n  \"title\": \"EbsVolumesResult\",\n  \"description\": \"Describes the configuration of scanning EBS volumes as a data source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"Describes whether scanning EBS volumes is enabled as a data source.\"\n        }\n      ]\n    },\n    \"Reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"reason\"\n          },\n          \"description\": \"Specifies the reason why scanning\
  \ EBS volumes (Malware Protection) was not enabled as a data source.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-ebs-volumes-result-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: EbsVolumesResult
---
