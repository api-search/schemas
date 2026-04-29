---
description: Describes whether Malware Protection for EC2 instances with findings will be enabled as a data source.
layout: schema
name: ScanEc2InstanceWithFindings
properties_list:
- description: ''
  name: EbsVolumes
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-scan-ec2-instance-with-findings-schema.json
slug: guardduty-scan-ec2-instance-with-findings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-ec2-instance-with-findings-schema.json\",\n  \"title\": \"ScanEc2InstanceWithFindings\",\n  \"description\": \"Describes whether Malware Protection for EC2 instances with findings will be enabled as a data source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EbsVolumes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ebsVolumes\"\n          },\n          \"description\": \"Describes the configuration for scanning EBS volumes as data source.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-ec2-instance-with-findings-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ScanEc2InstanceWithFindings
---
