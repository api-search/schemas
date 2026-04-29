---
description: <p/>
layout: schema
name: GetDataflowEndpointGroupResponse
properties_list:
- description: ''
  name: contactPostPassDurationSeconds
  type: object
- description: ''
  name: contactPrePassDurationSeconds
  type: object
- description: ''
  name: dataflowEndpointGroupArn
  type: object
- description: ''
  name: dataflowEndpointGroupId
  type: object
- description: ''
  name: endpointsDetails
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-get-dataflow-endpoint-group-response-schema.json
slug: ground-station-get-dataflow-endpoint-group-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-get-dataflow-endpoint-group-response-schema.json\",\n  \"title\": \"GetDataflowEndpointGroupResponse\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contactPostPassDurationSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataflowEndpointGroupDurationInSeconds\"\n        },\n        {\n          \"description\": \"Amount of time, in seconds, after a contact ends that the Ground Station Dataflow Endpoint Group will be in a <code>POSTPASS</code> state. A Ground Station Dataflow Endpoint Group State Change event will be emitted when the Dataflow Endpoint Group enters and exits the <code>POSTPASS</code> state.\"\n        }\n      ]\n    },\n    \"contactPrePassDurationSeconds\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/DataflowEndpointGroupDurationInSeconds\"\n        },\n        {\n          \"description\": \"Amount of time, in seconds, before a contact starts that the Ground Station Dataflow Endpoint Group will be in a <code>PREPASS</code> state. A Ground Station Dataflow Endpoint Group State Change event will be emitted when the Dataflow Endpoint Group enters and exits the <code>PREPASS</code> state.\"\n        }\n      ]\n    },\n    \"dataflowEndpointGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataflowEndpointGroupArn\"\n        },\n        {\n          \"description\": \"ARN of a dataflow endpoint group.\"\n        }\n      ]\n    },\n    \"dataflowEndpointGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"UUID of a dataflow endpoint group.\"\n        }\n      ]\n    },\n    \"endpointsDetails\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/EndpointDetailsList\"\n        },\n        {\n          \"description\": \"Details of a dataflow endpoint.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"Tags assigned to a dataflow endpoint group.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-get-dataflow-endpoint-group-response-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: GetDataflowEndpointGroupResponse
---
