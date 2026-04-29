---
description: DescribeSnapshotScheduleOutput schema from Amazon Storage Gateway API
layout: schema
name: DescribeSnapshotScheduleOutput
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
  name: Timezone
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-snapshot-schedule-output-schema.json
slug: amazon-storage-gateway-describe-snapshot-schedule-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-snapshot-schedule-output-schema.json\",\n  \"title\": \"DescribeSnapshotScheduleOutput\",\n  \"description\": \"DescribeSnapshotScheduleOutput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VolumeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the volume that was specified in the request.\"\n        }\n      ]\n    },\n    \"StartAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HourOfDay\"\n        },\n        {\n          \"description\": \"The hour of the day at which the snapshot schedule begins represented as <i>hh</i>, where <i>hh</i> is the hour\
  \ (0 to 23). The hour of the day is in the time zone of the gateway.\"\n        }\n      ]\n    },\n    \"RecurrenceInHours\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecurrenceInHours\"\n        },\n        {\n          \"description\": \"The number of hours between snapshots.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The snapshot description.\"\n        }\n      ]\n    },\n    \"Timezone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayTimezone\"\n        },\n        {\n          \"description\": \"A value that indicates the time zone of the gateway.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"A list of up to 50 tags assigned\
  \ to the snapshot schedule, sorted alphabetically by key name. Each tag is a key-value pair. For a gateway with more than 10 tags assigned, you can view all tags using the <code>ListTagsForResource</code> API operation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-snapshot-schedule-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeSnapshotScheduleOutput
---
