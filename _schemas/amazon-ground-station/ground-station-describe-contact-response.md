---
description: <p/>
layout: schema
name: DescribeContactResponse
properties_list:
- description: ''
  name: contactId
  type: object
- description: ''
  name: contactStatus
  type: object
- description: ''
  name: dataflowList
  type: object
- description: ''
  name: endTime
  type: object
- description: ''
  name: errorMessage
  type: object
- description: ''
  name: groundStation
  type: object
- description: ''
  name: maximumElevation
  type: object
- description: ''
  name: missionProfileArn
  type: object
- description: ''
  name: postPassEndTime
  type: object
- description: ''
  name: prePassStartTime
  type: object
- description: ''
  name: region
  type: object
- description: ''
  name: satelliteArn
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-describe-contact-response-schema.json
slug: ground-station-describe-contact-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-describe-contact-response-schema.json\",\n  \"title\": \"DescribeContactResponse\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contactId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"UUID of a contact.\"\n        }\n      ]\n    },\n    \"contactStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContactStatus\"\n        },\n        {\n          \"description\": \"Status of a contact.\"\n        }\n      ]\n    },\n    \"dataflowList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataflowList\"\n        },\n        {\n          \"description\": \"List describing source and destination\
  \ details for each dataflow edge.\"\n        }\n      ]\n    },\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"End time of a contact in UTC.\"\n        }\n      ]\n    },\n    \"errorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Error message for a contact.\"\n        }\n      ]\n    },\n    \"groundStation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Ground station for a contact.\"\n        }\n      ]\n    },\n    \"maximumElevation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Elevation\"\n        },\n        {\n          \"description\": \"Maximum elevation angle of a contact.\"\n        }\n      ]\n    },\n    \"missionProfileArn\": {\n   \
  \   \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MissionProfileArn\"\n        },\n        {\n          \"description\": \"ARN of a mission profile.\"\n        }\n      ]\n    },\n    \"postPassEndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Amount of time after a contact ends that you\\u2019d like to receive a CloudWatch event indicating the pass has finished.\"\n        }\n      ]\n    },\n    \"prePassStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Amount of time prior to contact start you\\u2019d like to receive a CloudWatch event indicating an upcoming pass.\"\n        }\n      ]\n    },\n    \"region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Region of\
  \ a contact.\"\n        }\n      ]\n    },\n    \"satelliteArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/satelliteArn\"\n        },\n        {\n          \"description\": \"ARN of a satellite.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Start time of a contact in UTC.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"Tags assigned to a contact.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-describe-contact-response-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: DescribeContactResponse
---
