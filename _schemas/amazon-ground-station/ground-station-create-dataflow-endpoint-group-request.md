---
description: <p/>
layout: schema
name: CreateDataflowEndpointGroupRequest
properties_list:
- description: ''
  name: contactPostPassDurationSeconds
  type: object
- description: ''
  name: contactPrePassDurationSeconds
  type: object
- description: ''
  name: endpointDetails
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-create-dataflow-endpoint-group-request-schema.json
slug: ground-station-create-dataflow-endpoint-group-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-create-dataflow-endpoint-group-request-schema.json\",\n  \"title\": \"CreateDataflowEndpointGroupRequest\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contactPostPassDurationSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataflowEndpointGroupDurationInSeconds\"\n        },\n        {\n          \"description\": \"Amount of time, in seconds, after a contact ends that the Ground Station Dataflow Endpoint Group will be in a <code>POSTPASS</code> state. A Ground Station Dataflow Endpoint Group State Change event will be emitted when the Dataflow Endpoint Group enters and exits the <code>POSTPASS</code> state.\"\n        }\n      ]\n    },\n    \"contactPrePassDurationSeconds\": {\n      \"allOf\": [\n    \
  \    {\n          \"$ref\": \"#/components/schemas/DataflowEndpointGroupDurationInSeconds\"\n        },\n        {\n          \"description\": \"Amount of time, in seconds, before a contact starts that the Ground Station Dataflow Endpoint Group will be in a <code>PREPASS</code> state. A Ground Station Dataflow Endpoint Group State Change event will be emitted when the Dataflow Endpoint Group enters and exits the <code>PREPASS</code> state.\"\n        }\n      ]\n    },\n    \"endpointDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointDetailsList\"\n        },\n        {\n          \"description\": \"Endpoint details of each endpoint in the dataflow endpoint group.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"Tags of a dataflow endpoint group.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"\
  endpointDetails\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-create-dataflow-endpoint-group-request-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: CreateDataflowEndpointGroupRequest
---
