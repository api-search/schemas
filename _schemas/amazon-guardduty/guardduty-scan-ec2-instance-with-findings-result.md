---
description: An object that contains information on the status of whether Malware Protection for EC2 instances with findings will be enabled as a data source.
layout: schema
name: ScanEc2InstanceWithFindingsResult
properties_list:
- description: ''
  name: EbsVolumes
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-scan-ec2-instance-with-findings-result-schema.json
slug: guardduty-scan-ec2-instance-with-findings-result
source_filename: guardduty-scan-ec2-instance-with-findings-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-ec2-instance-with-findings-result-schema.json\",\n  \"title\": \"ScanEc2InstanceWithFindingsResult\",\n  \"description\": \"An object that contains information on the status of whether Malware Protection for EC2 instances with findings will be enabled as a data source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EbsVolumes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EbsVolumesResult\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ebsVolumes\"\n          },\n          \"description\": \"Describes the configuration of scanning EBS volumes as a data source.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-scan-ec2-instance-with-findings-result-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ScanEc2InstanceWithFindingsResult
---
