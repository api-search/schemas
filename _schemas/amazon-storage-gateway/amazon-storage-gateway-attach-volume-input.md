---
description: AttachVolumeInput
layout: schema
name: AttachVolumeInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: TargetName
  type: object
- description: ''
  name: VolumeARN
  type: object
- description: ''
  name: NetworkInterfaceId
  type: object
- description: ''
  name: DiskId
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-attach-volume-input-schema.json
slug: amazon-storage-gateway-attach-volume-input
source_filename: amazon-storage-gateway-attach-volume-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-attach-volume-input-schema.json\",\n  \"title\": \"AttachVolumeInput\",\n  \"description\": \"AttachVolumeInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the gateway that you want to attach the volume to.\"\n        }\n      ]\n    },\n    \"TargetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetName\"\n        },\n        {\n          \"description\": \"<p>The name of the iSCSI target used by an initiator to connect to a volume and used as a suffix for the target ARN. For example, specifying <code>TargetName</code> as <i>myvolume</i>\
  \ results in the target ARN of <code>arn:aws:storagegateway:us-east-2:111122223333:gateway/sgw-12A3456B/target/iqn.1997-05.com.amazon:myvolume</code>. The target name must be unique across all volumes on a gateway.</p> <p>If you don't specify a value, Storage Gateway uses the value that was previously used for this volume as the new target name.</p>\"\n        }\n      ]\n    },\n    \"VolumeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the volume to attach to the specified gateway.\"\n        }\n      ]\n    },\n    \"NetworkInterfaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkInterfaceId\"\n        },\n        {\n          \"description\": \"<p>The network interface of the gateway on which to expose the iSCSI target. Only IPv4 addresses are accepted. Use <a>DescribeGatewayInformation</a> to get a list of\
  \ the network interfaces available on a gateway.</p> <p>Valid Values: A valid IP address.</p>\"\n        }\n      ]\n    },\n    \"DiskId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DiskId\"\n        },\n        {\n          \"description\": \"The unique device ID or other distinguishing data that identifies the local disk used to create the volume. This value is only required when you are attaching a stored volume.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GatewayARN\",\n    \"VolumeARN\",\n    \"NetworkInterfaceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-attach-volume-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: AttachVolumeInput
---
