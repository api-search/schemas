---
description: 'A JSON object containing the following fields:'
layout: schema
name: DescribeCachediSCSIVolumesOutput
properties_list:
- description: ''
  name: CachediSCSIVolumes
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-cachedi-scsi-volumes-output-schema.json
slug: amazon-storage-gateway-describe-cachedi-scsi-volumes-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-cachedi-scsi-volumes-output-schema.json\",\n  \"title\": \"DescribeCachediSCSIVolumesOutput\",\n  \"description\": \"A JSON object containing the following fields:\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CachediSCSIVolumes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CachediSCSIVolumes\"\n        },\n        {\n          \"description\": \"An array of objects where each object contains metadata about one cached volume.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-cachedi-scsi-volumes-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeCachediSCSIVolumesOutput
---
