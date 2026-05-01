---
description: <p>A JSON object containing one or more of the following fields:</p> <ul> <li> <p> <a>UpdateSnapshotScheduleInput$Description</a> </p> </li> <li> <p> <a>UpdateSnapshotScheduleInput$RecurrenceInHours</a> </p> </li> <li> <p> <a>UpdateSnapshotScheduleInput$StartAt</a> </p> </li> <li> <p> <a>UpdateSnapshotScheduleInput$VolumeARN</a> </p> </li> </ul>
layout: schema
name: UpdateSnapshotScheduleInput
properties_list:
- description: ''
  name: VolumeARN
  type: object
- description: ''
  name: StartAt
  type: object
- description: ''
  name: RecurrenceInHours
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-update-snapshot-schedule-input-schema.json
slug: amazon-storage-gateway-update-snapshot-schedule-input
source_filename: amazon-storage-gateway-update-snapshot-schedule-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-snapshot-schedule-input-schema.json\",\n  \"title\": \"UpdateSnapshotScheduleInput\",\n  \"description\": \"<p>A JSON object containing one or more of the following fields:</p> <ul> <li> <p> <a>UpdateSnapshotScheduleInput$Description</a> </p> </li> <li> <p> <a>UpdateSnapshotScheduleInput$RecurrenceInHours</a> </p> </li> <li> <p> <a>UpdateSnapshotScheduleInput$StartAt</a> </p> </li> <li> <p> <a>UpdateSnapshotScheduleInput$VolumeARN</a> </p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VolumeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the volume. Use the <a>ListVolumes</a> operation to return a list of gateway\
  \ volumes.\"\n        }\n      ]\n    },\n    \"StartAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HourOfDay\"\n        },\n        {\n          \"description\": \"The hour of the day at which the snapshot schedule begins represented as <i>hh</i>, where <i>hh</i> is the hour (0 to 23). The hour of the day is in the time zone of the gateway.\"\n        }\n      ]\n    },\n    \"RecurrenceInHours\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecurrenceInHours\"\n        },\n        {\n          \"description\": \"Frequency of snapshots. Specify the number of hours between snapshots.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"Optional description of the snapshot that overwrites the existing description.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"<p>A list of up to 50 tags that can be assigned to a snapshot. Each tag is a key-value pair.</p> <note> <p>Valid characters for key and value are letters, spaces, and numbers representable in UTF-8 format, and the following special characters: + - = . _ : / @. The maximum length of a tag's key is 128 characters, and the maximum length for a tag's value is 256.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VolumeARN\",\n    \"StartAt\",\n    \"RecurrenceInHours\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-snapshot-schedule-input-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: UpdateSnapshotScheduleInput
---
