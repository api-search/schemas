---
description: A base object for all types of volume attachments. Represents the attachment between a compute instance and a block volume.
layout: schema
name: VolumeAttachment
properties_list:
- description: The OCID of the volume attachment
  name: id
  type: string
- description: The OCID of the instance the volume is attached to
  name: instanceId
  type: string
- description: The OCID of the volume
  name: volumeId
  type: string
- description: The OCID of the compartment
  name: compartmentId
  type: string
- description: The availability domain of an instance
  name: availabilityDomain
  type: string
- description: A user-friendly name for the attachment
  name: displayName
  type: string
- description: The device name (e.g., /dev/oracleoci/oraclevdb)
  name: device
  type: string
- description: The type of volume attachment
  name: attachmentType
  type: string
- description: The lifecycle state of the volume attachment
  name: lifecycleState
  type: string
- description: The date and time the volume was attached
  name: timeCreated
  type: string
- description: Whether the attachment was created in read-only mode
  name: isReadOnly
  type: boolean
- description: Whether the attachment should be created in shareable mode
  name: isShareable
  type: boolean
- description: Whether in-transit encryption is enabled for the attachment
  name: isPvEncryptionInTransitEnabled
  type: boolean
- description: Whether the attachment is multipath
  name: isMultipath
  type: boolean
- description: The iSCSI login state of the volume attachment
  name: iscsiLoginState
  type: string
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-volume-attachment-schema.json
slug: oci-compute-volume-attachment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VolumeAttachment\",\n  \"type\": \"object\",\n  \"description\": \"A base object for all types of volume attachments. Represents the attachment between a compute instance and a block volume.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the volume attachment\"\n    },\n    \"instanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the instance the volume is attached to\"\n    },\n    \"volumeId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the volume\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the compartment\"\n    },\n    \"availabilityDomain\": {\n      \"type\": \"string\",\n      \"description\": \"The availability domain of an instance\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"A user-friendly name for the attachment\"\n    },\n    \"device\": {\n      \"type\": \"string\",\n      \"description\": \"The device name (e.g., /dev/oracleoci/oraclevdb)\"\n    },\n    \"attachmentType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of volume attachment\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"description\": \"The lifecycle state of the volume attachment\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the volume was attached\"\n    },\n    \"isReadOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the attachment was created in read-only mode\"\n    },\n    \"isShareable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the attachment should be created in shareable mode\"\n    },\n    \"isPvEncryptionInTransitEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether in-transit encryption is\
  \ enabled for the attachment\"\n    },\n    \"isMultipath\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the attachment is multipath\"\n    },\n    \"iscsiLoginState\": {\n      \"type\": \"string\",\n      \"description\": \"The iSCSI login state of the volume attachment\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-volume-attachment-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: VolumeAttachment
---
