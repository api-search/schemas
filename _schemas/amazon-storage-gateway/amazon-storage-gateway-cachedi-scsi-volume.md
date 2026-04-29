---
description: Describes an iSCSI cached volume.
layout: schema
name: CachediSCSIVolume
properties_list:
- description: ''
  name: VolumeARN
  type: object
- description: ''
  name: VolumeId
  type: object
- description: ''
  name: VolumeType
  type: object
- description: ''
  name: VolumeStatus
  type: object
- description: ''
  name: VolumeAttachmentStatus
  type: object
- description: ''
  name: VolumeSizeInBytes
  type: object
- description: ''
  name: VolumeProgress
  type: object
- description: ''
  name: SourceSnapshotId
  type: object
- description: ''
  name: VolumeiSCSIAttributes
  type: object
- description: ''
  name: CreatedDate
  type: object
- description: ''
  name: VolumeUsedInBytes
  type: object
- description: ''
  name: KMSKey
  type: object
- description: ''
  name: TargetName
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-cachedi-scsi-volume-schema.json
slug: amazon-storage-gateway-cachedi-scsi-volume
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-cachedi-scsi-volume-schema.json\",\n  \"title\": \"CachediSCSIVolume\",\n  \"description\": \"Describes an iSCSI cached volume.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VolumeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the storage volume.\"\n        }\n      ]\n    },\n    \"VolumeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeId\"\n        },\n        {\n          \"description\": \"The unique identifier of the volume, e.g., vol-AE4B946D.\"\n        }\n      ]\n    },\n    \"VolumeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeType\"\n\
  \        },\n        {\n          \"description\": \"One of the VolumeType enumeration values that describes the type of the volume.\"\n        }\n      ]\n    },\n    \"VolumeStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeStatus\"\n        },\n        {\n          \"description\": \"One of the VolumeStatus values that indicates the state of the storage volume.\"\n        }\n      ]\n    },\n    \"VolumeAttachmentStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeAttachmentStatus\"\n        },\n        {\n          \"description\": \"A value that indicates whether a storage volume is attached to or detached from a gateway. For more information, see <a href=\\\"https://docs.aws.amazon.com/storagegateway/latest/userguide/managing-volumes.html#attach-detach-volume\\\">Moving your volumes to a different gateway</a>.\"\n        }\n      ]\n    },\n    \"VolumeSizeInBytes\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/long\"\n        },\n        {\n          \"description\": \"The size, in bytes, of the volume capacity.\"\n        }\n      ]\n    },\n    \"VolumeProgress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DoubleObject\"\n        },\n        {\n          \"description\": \"Represents the percentage complete if the volume is restoring or bootstrapping that represents the percent of data transferred. This field does not appear in the response if the cached volume is not restoring or bootstrapping.\"\n        }\n      ]\n    },\n    \"SourceSnapshotId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnapshotId\"\n        },\n        {\n          \"description\": \"If the cached volume was created from a snapshot, this field contains the snapshot ID used, e.g., snap-78e22663. Otherwise, this field is not included.\"\n        }\n      ]\n    },\n    \"VolumeiSCSIAttributes\": {\n  \
  \    \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeiSCSIAttributes\"\n        },\n        {\n          \"description\": \"An <a>VolumeiSCSIAttributes</a> object that represents a collection of iSCSI attributes for one stored volume.\"\n        }\n      ]\n    },\n    \"CreatedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedDate\"\n        },\n        {\n          \"description\": \"The date the volume was created. Volumes created prior to March 28, 2017 don\\u2019t have this timestamp.\"\n        }\n      ]\n    },\n    \"VolumeUsedInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeUsedInBytes\"\n        },\n        {\n          \"description\": \"<p>The size of the data stored on the volume in bytes. This value is calculated based on the number of blocks that are touched, instead of the actual amount of data written. This value can be useful for sequential write patterns\
  \ but less accurate for random write patterns. <code>VolumeUsedInBytes</code> is different from the compressed size of the volume, which is the value that is used to calculate your bill.</p> <note> <p>This value is not available for volumes created prior to May 13, 2015, until you store data on the volume.</p> <p>If you use a delete tool that overwrites the data on your volume with random data, your usage will not be reduced. This is because the random data is not compressible. If you want to reduce the amount of billed storage on your volume, we recommend overwriting your files with zeros to compress the data to a negligible amount of actual storage.</p> </note>\"\n        }\n      ]\n    },\n    \"KMSKey\": {\n      \"$ref\": \"#/components/schemas/KMSKey\"\n    },\n    \"TargetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetName\"\n        },\n        {\n          \"description\": \"<p>The name of the iSCSI target used by an initiator to connect\
  \ to a volume and used as a suffix for the target ARN. For example, specifying <code>TargetName</code> as <i>myvolume</i> results in the target ARN of <code>arn:aws:storagegateway:us-east-2:111122223333:gateway/sgw-12A3456B/target/iqn.1997-05.com.amazon:myvolume</code>. The target name must be unique across all volumes on a gateway.</p> <p>If you don't specify a value, Storage Gateway uses the value that was previously used for this volume as the new target name.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-cachedi-scsi-volume-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: CachediSCSIVolume
---
