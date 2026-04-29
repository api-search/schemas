---
description: <p/>
layout: schema
name: GetMissionProfileResponse
properties_list:
- description: ''
  name: contactPostPassDurationSeconds
  type: object
- description: ''
  name: contactPrePassDurationSeconds
  type: object
- description: ''
  name: dataflowEdges
  type: object
- description: ''
  name: minimumViableContactDurationSeconds
  type: object
- description: ''
  name: missionProfileArn
  type: object
- description: ''
  name: missionProfileId
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: region
  type: object
- description: ''
  name: streamsKmsKey
  type: object
- description: ''
  name: streamsKmsRole
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: trackingConfigArn
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-get-mission-profile-response-schema.json
slug: ground-station-get-mission-profile-response
source_filename: ground-station-get-mission-profile-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-get-mission-profile-response-schema.json\",\n  \"title\": \"GetMissionProfileResponse\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contactPostPassDurationSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSeconds\"\n        },\n        {\n          \"description\": \"Amount of time after a contact ends that you\\u2019d like to receive a CloudWatch event indicating the pass has finished.\"\n        }\n      ]\n    },\n    \"contactPrePassDurationSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInSeconds\"\n        },\n        {\n          \"description\": \"Amount of time prior to contact start you\\u2019d like to receive a CloudWatch event indicating\
  \ an upcoming pass.\"\n        }\n      ]\n    },\n    \"dataflowEdges\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataflowEdgeList\"\n        },\n        {\n          \"description\": \"A list of lists of ARNs. Each list of ARNs is an edge, with a <i>from</i> <code>Config</code> and a <i>to</i> <code>Config</code>.\"\n        }\n      ]\n    },\n    \"minimumViableContactDurationSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveDurationInSeconds\"\n        },\n        {\n          \"description\": \"Smallest amount of time in seconds that you\\u2019d like to see for an available contact. AWS Ground Station will not present you with contacts shorter than this duration.\"\n        }\n      ]\n    },\n    \"missionProfileArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MissionProfileArn\"\n        },\n        {\n          \"description\": \"ARN of a mission profile.\"\n  \
  \      }\n      ]\n    },\n    \"missionProfileId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"UUID of a mission profile.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SafeName\"\n        },\n        {\n          \"description\": \"Name of a mission profile.\"\n        }\n      ]\n    },\n    \"region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AWSRegion\"\n        },\n        {\n          \"description\": \"Region of a mission profile.\"\n        }\n      ]\n    },\n    \"streamsKmsKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKey\"\n        },\n        {\n          \"description\": \"KMS key to use for encrypting streams.\"\n        }\n      ]\n    },\n    \"streamsKmsRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\
  \n        },\n        {\n          \"description\": \"Role to use for encrypting streams with KMS key.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"Tags assigned to a mission profile.\"\n        }\n      ]\n    },\n    \"trackingConfigArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigArn\"\n        },\n        {\n          \"description\": \"ARN of a tracking <code>Config</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-get-mission-profile-response-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: GetMissionProfileResponse
---
