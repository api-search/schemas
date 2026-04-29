---
description: <p>A JSON object containing one or more of the following fields:</p> <ul> <li> <p> <a>CreateStorediSCSIVolumeInput$DiskId</a> </p> </li> <li> <p> <a>CreateStorediSCSIVolumeInput$NetworkInterfaceId</a> </p> </li> <li> <p> <a>CreateStorediSCSIVolumeInput$PreserveExistingData</a> </p> </li> <li> <p> <a>CreateStorediSCSIVolumeInput$SnapshotId</a> </p> </li> <li> <p> <a>CreateStorediSCSIVolumeInput$TargetName</a> </p> </li> </ul>
layout: schema
name: CreateStorediSCSIVolumeInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: DiskId
  type: object
- description: ''
  name: SnapshotId
  type: object
- description: ''
  name: PreserveExistingData
  type: object
- description: ''
  name: TargetName
  type: object
- description: ''
  name: NetworkInterfaceId
  type: object
- description: ''
  name: KMSEncrypted
  type: object
- description: ''
  name: KMSKey
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-create-storedi-scsi-volume-input-schema.json
slug: amazon-storage-gateway-create-storedi-scsi-volume-input
source_filename: amazon-storage-gateway-create-storedi-scsi-volume-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-storedi-scsi-volume-input-schema.json\",\n  \"title\": \"CreateStorediSCSIVolumeInput\",\n  \"description\": \"<p>A JSON object containing one or more of the following fields:</p> <ul> <li> <p> <a>CreateStorediSCSIVolumeInput$DiskId</a> </p> </li> <li> <p> <a>CreateStorediSCSIVolumeInput$NetworkInterfaceId</a> </p> </li> <li> <p> <a>CreateStorediSCSIVolumeInput$PreserveExistingData</a> </p> </li> <li> <p> <a>CreateStorediSCSIVolumeInput$SnapshotId</a> </p> </li> <li> <p> <a>CreateStorediSCSIVolumeInput$TargetName</a> </p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"DiskId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DiskId\"\n\
  \        },\n        {\n          \"description\": \"The unique identifier for the gateway local disk that is configured as a stored volume. Use <a href=\\\"https://docs.aws.amazon.com/storagegateway/latest/userguide/API_ListLocalDisks.html\\\">ListLocalDisks</a> to list disk IDs for a gateway.\"\n        }\n      ]\n    },\n    \"SnapshotId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnapshotId\"\n        },\n        {\n          \"description\": \"The snapshot ID (e.g., \\\"snap-1122aabb\\\") of the snapshot to restore as the new stored volume. Specify this field if you want to create the iSCSI storage volume from a snapshot; otherwise, do not include this field. To list snapshots for your account use <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/ApiReference-query-DescribeSnapshots.html\\\">DescribeSnapshots</a> in the <i>Amazon Elastic Compute Cloud API Reference</i>.\"\n        }\n      ]\n    },\n    \"PreserveExistingData\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/boolean\"\n        },\n        {\n          \"description\": \"<p>Set to <code>true</code> if you want to preserve the data on the local disk. Otherwise, set to <code>false</code> to create an empty volume.</p> <p>Valid Values: <code>true</code> | <code>false</code> </p>\"\n        }\n      ]\n    },\n    \"TargetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetName\"\n        },\n        {\n          \"description\": \"<p>The name of the iSCSI target used by an initiator to connect to a volume and used as a suffix for the target ARN. For example, specifying <code>TargetName</code> as <i>myvolume</i> results in the target ARN of <code>arn:aws:storagegateway:us-east-2:111122223333:gateway/sgw-12A3456B/target/iqn.1997-05.com.amazon:myvolume</code>. The target name must be unique across all volumes on a gateway.</p> <p>If you don't specify a value, Storage Gateway uses\
  \ the value that was previously used for this volume as the new target name.</p>\"\n        }\n      ]\n    },\n    \"NetworkInterfaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkInterfaceId\"\n        },\n        {\n          \"description\": \"<p>The network interface of the gateway on which to expose the iSCSI target. Only IPv4 addresses are accepted. Use <a>DescribeGatewayInformation</a> to get a list of the network interfaces available on a gateway.</p> <p>Valid Values: A valid IP address.</p>\"\n        }\n      ]\n    },\n    \"KMSEncrypted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Set to <code>true</code> to use Amazon S3 server-side encryption with your own KMS key, or <code>false</code> to use a key managed by Amazon S3. Optional.</p> <p>Valid Values: <code>true</code> | <code>false</code> </p>\"\n        }\n      ]\n    },\n   \
  \ \"KMSKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KMSKey\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of a symmetric customer master key (CMK) used for Amazon S3 server-side encryption. Storage Gateway does not support asymmetric CMKs. This value can only be set when <code>KMSEncrypted</code> is <code>true</code>. Optional.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"<p>A list of up to 50 tags that can be assigned to a stored volume. Each tag is a key-value pair.</p> <note> <p>Valid characters for key and value are letters, spaces, and numbers representable in UTF-8 format, and the following special characters: + - = . _ : / @. The maximum length of a tag's key is 128 characters, and the maximum length for a tag's value is 256.</p> </note>\"\n        }\n      ]\n    }\n\
  \  },\n  \"required\": [\n    \"GatewayARN\",\n    \"DiskId\",\n    \"PreserveExistingData\",\n    \"TargetName\",\n    \"NetworkInterfaceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-storedi-scsi-volume-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: CreateStorediSCSIVolumeInput
---
