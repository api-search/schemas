---
description: DescribeCachediSCSIVolumesInput schema from Amazon Storage Gateway API
layout: schema
name: DescribeCachediSCSIVolumesInput
properties_list:
- description: ''
  name: VolumeARNs
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-cachedi-scsi-volumes-input-schema.json
slug: amazon-storage-gateway-describe-cachedi-scsi-volumes-input
source_filename: amazon-storage-gateway-describe-cachedi-scsi-volumes-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-cachedi-scsi-volumes-input-schema.json\",\n  \"title\": \"DescribeCachediSCSIVolumesInput\",\n  \"description\": \"DescribeCachediSCSIVolumesInput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VolumeARNs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeARNs\"\n        },\n        {\n          \"description\": \"An array of strings where each string represents the Amazon Resource Name (ARN) of a cached volume. All of the specified cached volumes must be from the same gateway. Use <a>ListVolumes</a> to get volume ARNs for a gateway.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VolumeARNs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-cachedi-scsi-volumes-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeCachediSCSIVolumesInput
---
