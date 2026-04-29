---
description: Resource capacity settings. Fleet capacity is measured in Amazon EC2 instances. Pending and terminating counts are non-zero when the fleet capacity is adjusting to a scaling event or if access to resources is temporarily affected.
layout: schema
name: EC2InstanceCounts
properties_list:
- description: ''
  name: DESIRED
  type: object
- description: ''
  name: MINIMUM
  type: object
- description: ''
  name: MAXIMUM
  type: object
- description: ''
  name: PENDING
  type: object
- description: ''
  name: ACTIVE
  type: object
- description: ''
  name: IDLE
  type: object
- description: ''
  name: TERMINATING
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-ec2-instance-counts-schema.json
slug: gamelift-ec2-instance-counts
source_filename: gamelift-ec2-instance-counts-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-ec2-instance-counts-schema.json\",\n  \"title\": \"EC2InstanceCounts\",\n  \"description\": \"Resource capacity settings. Fleet capacity is measured in Amazon EC2 instances. Pending and terminating counts are non-zero when the fleet capacity is adjusting to a scaling event or if access to resources is temporarily affected.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DESIRED\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"Ideal number of active instances. GameLift will always try to maintain the desired number of instances. Capacity is scaled up or down by changing the desired instances. \"\n        }\n      ]\n    },\n    \"MINIMUM\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"The minimum instance count value allowed.\"\n        }\n      ]\n    },\n    \"MAXIMUM\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"The maximum instance count value allowed.\"\n        }\n      ]\n    },\n    \"PENDING\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"Number of instances that are starting but not yet active.\"\n        }\n      ]\n    },\n    \"ACTIVE\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"Actual number of instances that are ready to host game sessions.\"\n        }\n      ]\n    },\n    \"IDLE\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\
  \n        },\n        {\n          \"description\": \"Number of active instances that are not currently hosting a game session.\"\n        }\n      ]\n    },\n    \"TERMINATING\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"Number of instances that are no longer active but haven't yet been terminated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-ec2-instance-counts-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: EC2InstanceCounts
---
