---
description: Describes a virtual tape object.
layout: schema
name: Tape
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
  name: TapeStatus
  type: object
- description: ''
  name: VTLDevice
  type: object
- description: ''
  name: Progress
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
schema_file: json-schema/amazon-storage-gateway-tape-schema.json
slug: amazon-storage-gateway-tape
source_filename: amazon-storage-gateway-tape-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-tape-schema.json\",\n  \"title\": \"Tape\",\n  \"description\": \"Describes a virtual tape object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TapeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the virtual tape.\"\n        }\n      ]\n    },\n    \"TapeBarcode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeBarcode\"\n        },\n        {\n          \"description\": \"The barcode that identifies a specific virtual tape.\"\n        }\n      ]\n    },\n    \"TapeCreatedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"\
  description\": \"The date the virtual tape was created.\"\n        }\n      ]\n    },\n    \"TapeSizeInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeSize\"\n        },\n        {\n          \"description\": \"The size, in bytes, of the virtual tape capacity.\"\n        }\n      ]\n    },\n    \"TapeStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeStatus\"\n        },\n        {\n          \"description\": \"The current state of the virtual tape.\"\n        }\n      ]\n    },\n    \"VTLDevice\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VTLDeviceARN\"\n        },\n        {\n          \"description\": \"The virtual tape library (VTL) device that the virtual tape is associated with.\"\n        }\n      ]\n    },\n    \"Progress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DoubleObject\"\n        },\n        {\n          \"description\"\
  : \"<p>For archiving virtual tapes, indicates how much data remains to be uploaded before archiving is complete.</p> <p>Range: 0 (not started) to 100 (complete).</p>\"\n        }\n      ]\n    },\n    \"TapeUsedInBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeUsage\"\n        },\n        {\n          \"description\": \"<p>The size, in bytes, of data stored on the virtual tape.</p> <note> <p>This value is not available for tapes created prior to May 13, 2015.</p> </note>\"\n        }\n      ]\n    },\n    \"KMSKey\": {\n      \"$ref\": \"#/components/schemas/KMSKey\"\n    },\n    \"PoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PoolId\"\n        },\n        {\n          \"description\": \"The ID of the pool that contains tapes that will be archived. The tapes in this pool are archived in the S3 storage class that is associated with the pool. When you use your backup application to eject the tape, the tape\
  \ is archived directly into the storage class (S3 Glacier or S3 Glacier Deep Archive) that corresponds to the pool.\"\n        }\n      ]\n    },\n    \"Worm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/boolean\"\n        },\n        {\n          \"description\": \"If the tape is archived as write-once-read-many (WORM), this value is <code>true</code>.\"\n        }\n      ]\n    },\n    \"RetentionStartDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \"The date that the tape is first archived with tape retention lock enabled.\"\n        }\n      ]\n    },\n    \"PoolEntryDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \"The date that the tape enters a custom tape pool.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-tape-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: Tape
---
