---
description: Attributes of a NetBackup backup image
layout: schema
name: ImageAttributes
properties_list:
- description: Unique identifier for the backup image
  name: backupId
  type: string
- description: Name of the policy that created this image
  name: policyName
  type: string
- description: Type of the policy
  name: policyType
  type: string
- description: Client hostname that was backed up
  name: clientName
  type: string
- description: Schedule name that triggered the backup
  name: scheduleName
  type: string
- description: Type of the schedule
  name: scheduleType
  type: string
- description: Timestamp when the backup was performed
  name: backupTime
  type: string
- description: Timestamp when the image will expire
  name: expirationTime
  type: string
- description: Total size of the backup image in kilobytes
  name: kilobytes
  type: integer
- description: Total number of files in the backup image
  name: numberOfFiles
  type: integer
- description: Primary copy number for the image
  name: primaryCopy
  type: integer
- description: Total number of copies of this image
  name: copyCount
  type: integer
- description: Media server that performed the backup
  name: mediaServer
  type: string
- description: Storage unit where the image is stored
  name: storageUnit
  type: string
- description: Media ID where the image resides
  name: mediaId
  type: string
- description: Whether the image data is compressed
  name: compressed
  type: boolean
- description: Whether the image data is encrypted
  name: encrypted
  type: boolean
- description: Whether the image is multiplexed
  name: multiplexed
  type: boolean
- description: Retention level assigned to the image
  name: retentionLevel
  type: integer
provider_name: Veritas NetBackup
provider_slug: veritas-netbackup
schema_file: json-schema/veritas-netbackup-rest-image-attributes-schema.json
slug: veritas-netbackup-rest-image-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImageAttributes\",\n  \"type\": \"object\",\n  \"description\": \"Attributes of a NetBackup backup image\",\n  \"properties\": {\n    \"backupId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the backup image\"\n    },\n    \"policyName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the policy that created this image\"\n    },\n    \"policyType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the policy\"\n    },\n    \"clientName\": {\n      \"type\": \"string\",\n      \"description\": \"Client hostname that was backed up\"\n    },\n    \"scheduleName\": {\n      \"type\": \"string\",\n      \"description\": \"Schedule name that triggered the backup\"\n    },\n    \"scheduleType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the schedule\"\n    },\n    \"backupTime\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Timestamp when the backup was performed\"\n    },\n    \"expirationTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the image will expire\"\n    },\n    \"kilobytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Total size of the backup image in kilobytes\"\n    },\n    \"numberOfFiles\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of files in the backup image\"\n    },\n    \"primaryCopy\": {\n      \"type\": \"integer\",\n      \"description\": \"Primary copy number for the image\"\n    },\n    \"copyCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of copies of this image\"\n    },\n    \"mediaServer\": {\n      \"type\": \"string\",\n      \"description\": \"Media server that performed the backup\"\n    },\n    \"storageUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Storage unit where the image is stored\"\n    },\n    \"mediaId\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Media ID where the image resides\"\n    },\n    \"compressed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the image data is compressed\"\n    },\n    \"encrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the image data is encrypted\"\n    },\n    \"multiplexed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the image is multiplexed\"\n    },\n    \"retentionLevel\": {\n      \"type\": \"integer\",\n      \"description\": \"Retention level assigned to the image\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/veritas-netbackup/refs/heads/main/json-schema/veritas-netbackup-rest-image-attributes-schema.json
tags:
- Backup
- Data Protection
- Disaster Recovery
- Enterprise
- Recovery
- Storage
title: ImageAttributes
---
