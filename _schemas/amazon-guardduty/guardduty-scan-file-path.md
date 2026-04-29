---
description: Contains details of infected file including name, file path and hash.
layout: schema
name: ScanFilePath
properties_list:
- description: ''
  name: FilePath
  type: object
- description: ''
  name: VolumeArn
  type: object
- description: ''
  name: Hash
  type: object
- description: ''
  name: FileName
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-scan-file-path-schema.json
slug: guardduty-scan-file-path
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-file-path-schema.json\",\n  \"title\": \"ScanFilePath\",\n  \"description\": \"Contains details of infected file including name, file path and hash.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FilePath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"filePath\"\n          },\n          \"description\": \"The file path of the infected file.\"\n        }\n      ]\n    },\n    \"VolumeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"volumeArn\"\n          },\n          \"description\": \"EBS volume Arn details of the infected file.\"\n        }\n      ]\n  \
  \  },\n    \"Hash\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hash\"\n          },\n          \"description\": \"The hash value of the infected file.\"\n        }\n      ]\n    },\n    \"FileName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fileName\"\n          },\n          \"description\": \"File name of the infected file.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-file-path-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ScanFilePath
---
