---
description: Represents a virtual tape that is archived in the virtual tape shelf (VTS).
layout: schema
name: TapeArchive
properties_list:
- description: ''
  name: TapeARN
  type: object
- description: ''
  name: TapeBarcode
  type: object
- description: ''
  name: TapeCreatedDate
  type: object
- description: ''
  name: TapeSizeInBytes
  type: object
- description: ''
  name: CompletionTime
  type: object
- description: ''
  name: RetrievedTo
  type: object
- description: ''
  name: TapeStatus
  type: object
- description: ''
  name: TapeUsedInBytes
  type: object
- description: ''
  name: KMSKey
  type: object
- description: ''
  name: PoolId
  type: object
- description: ''
  name: Worm
  type: object
- description: ''
  name: RetentionStartDate
  type: object
- description: ''
  name: PoolEntryDate
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-tape-archive-schema.json
slug: amazon-storage-gateway-tape-archive
source_filename: amazon-storage-gateway-tape-archive-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-tape-archive-schema.json\",\n  \"title\": \"TapeArchive\",\n  \"description\": \"Represents a virtual tape that is archived in the virtual tape shelf (VTS).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TapeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of an archived virtual tape.\"\n        }\n      ]\n    },\n    \"TapeBarcode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeBarcode\"\n        },\n        {\n          \"description\": \"The barcode that identifies the archived virtual tape.\"\n        }\n      ]\n    },\n    \"TapeCreatedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \"The date the virtual tape was created.\"\n        }\n      ]\n    },\n    \"TapeSizeInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeSize\"\n        },\n        {\n          \"description\": \"The size, in bytes, of the archived virtual tape.\"\n        }\n      ]\n    },\n    \"CompletionTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \"<p>The time that the archiving of the virtual tape was completed.</p> <p>The default timestamp format is in the ISO8601 extended YYYY-MM-DD'T'HH:MM:SS'Z' format.</p>\"\n        }\n      ]\n    },\n    \"RetrievedTo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayARN\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the tape gateway that the virtual tape\
  \ is being retrieved to.</p> <p>The virtual tape is retrieved from the virtual tape shelf (VTS).</p>\"\n        }\n      ]\n    },\n    \"TapeStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeArchiveStatus\"\n        },\n        {\n          \"description\": \"The current state of the archived virtual tape.\"\n        }\n      ]\n    },\n    \"TapeUsedInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeUsage\"\n        },\n        {\n          \"description\": \"<p>The size, in bytes, of data stored on the virtual tape.</p> <note> <p>This value is not available for tapes created prior to May 13, 2015.</p> </note>\"\n        }\n      ]\n    },\n    \"KMSKey\": {\n      \"$ref\": \"#/components/schemas/KMSKey\"\n    },\n    \"PoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PoolId\"\n        },\n        {\n          \"description\": \"The ID of the pool that was used to\
  \ archive the tape. The tapes in this pool are archived in the S3 storage class that is associated with the pool.\"\n        }\n      ]\n    },\n    \"Worm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/boolean\"\n        },\n        {\n          \"description\": \"Set to <code>true</code> if the archived tape is stored as write-once-read-many (WORM).\"\n        }\n      ]\n    },\n    \"RetentionStartDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \"If the archived tape is subject to tape retention lock, the date that the archived tape started being retained.\"\n        }\n      ]\n    },\n    \"PoolEntryDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \"<p>The time that the tape entered the custom tape pool.</p> <p>The default timestamp format is in the ISO8601 extended\
  \ YYYY-MM-DD'T'HH:MM:SS'Z' format.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-tape-archive-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: TapeArchive
---
