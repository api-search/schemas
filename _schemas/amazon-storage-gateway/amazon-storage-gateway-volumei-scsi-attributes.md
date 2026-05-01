---
description: Lists iSCSI information about a volume.
layout: schema
name: VolumeiSCSIAttributes
properties_list:
- description: ''
  name: TargetARN
  type: object
- description: ''
  name: NetworkInterfaceId
  type: object
- description: ''
  name: NetworkInterfacePort
  type: object
- description: ''
  name: LunNumber
  type: object
- description: ''
  name: ChapEnabled
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-volumei-scsi-attributes-schema.json
slug: amazon-storage-gateway-volumei-scsi-attributes
source_filename: amazon-storage-gateway-volumei-scsi-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-volumei-scsi-attributes-schema.json\",\n  \"title\": \"VolumeiSCSIAttributes\",\n  \"description\": \"Lists iSCSI information about a volume.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TargetARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the volume target.\"\n        }\n      ]\n    },\n    \"NetworkInterfaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkInterfaceId\"\n        },\n        {\n          \"description\": \"The network interface identifier.\"\n        }\n      ]\n    },\n    \"NetworkInterfacePort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/integer\"\
  \n        },\n        {\n          \"description\": \"The port used to communicate with iSCSI targets.\"\n        }\n      ]\n    },\n    \"LunNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveIntObject\"\n        },\n        {\n          \"description\": \"The logical disk number.\"\n        }\n      ]\n    },\n    \"ChapEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/boolean\"\n        },\n        {\n          \"description\": \"Indicates whether mutual CHAP is enabled for the iSCSI target.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-volumei-scsi-attributes-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: VolumeiSCSIAttributes
---
