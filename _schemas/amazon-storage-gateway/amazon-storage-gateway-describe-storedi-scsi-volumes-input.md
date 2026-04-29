---
description: A JSON object containing a list of <a>DescribeStorediSCSIVolumesInput$VolumeARNs</a>.
layout: schema
name: DescribeStorediSCSIVolumesInput
properties_list:
- description: ''
  name: VolumeARNs
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-storedi-scsi-volumes-input-schema.json
slug: amazon-storage-gateway-describe-storedi-scsi-volumes-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-storedi-scsi-volumes-input-schema.json\",\n  \"title\": \"DescribeStorediSCSIVolumesInput\",\n  \"description\": \"A JSON object containing a list of <a>DescribeStorediSCSIVolumesInput$VolumeARNs</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VolumeARNs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeARNs\"\n        },\n        {\n          \"description\": \"An array of strings where each string represents the Amazon Resource Name (ARN) of a stored volume. All of the specified stored volumes must be from the same gateway. Use <a>ListVolumes</a> to get volume ARNs for a gateway.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VolumeARNs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-storedi-scsi-volumes-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeStorediSCSIVolumesInput
---
