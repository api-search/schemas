---
description: A JSON object containing the Amazon Resource Name (ARN) of the iSCSI volume target.
layout: schema
name: DescribeChapCredentialsInput
properties_list:
- description: ''
  name: TargetARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-chap-credentials-input-schema.json
slug: amazon-storage-gateway-describe-chap-credentials-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-chap-credentials-input-schema.json\",\n  \"title\": \"DescribeChapCredentialsInput\",\n  \"description\": \"A JSON object containing the Amazon Resource Name (ARN) of the iSCSI volume target.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TargetARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the iSCSI volume target. Use the <a>DescribeStorediSCSIVolumes</a> operation to return to retrieve the TargetARN for specified VolumeARN.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TargetARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-chap-credentials-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeChapCredentialsInput
---
