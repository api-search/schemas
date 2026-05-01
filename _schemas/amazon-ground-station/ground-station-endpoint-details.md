---
description: Information about the endpoint details.
layout: schema
name: EndpointDetails
properties_list:
- description: ''
  name: awsGroundStationAgentEndpoint
  type: object
- description: ''
  name: endpoint
  type: object
- description: ''
  name: healthReasons
  type: object
- description: ''
  name: healthStatus
  type: object
- description: ''
  name: securityDetails
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-endpoint-details-schema.json
slug: ground-station-endpoint-details
source_filename: ground-station-endpoint-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-endpoint-details-schema.json\",\n  \"title\": \"EndpointDetails\",\n  \"description\": \"Information about the endpoint details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"awsGroundStationAgentEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsGroundStationAgentEndpoint\"\n        },\n        {\n          \"description\": \"An agent endpoint.\"\n        }\n      ]\n    },\n    \"endpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataflowEndpoint\"\n        },\n        {\n          \"description\": \"A dataflow endpoint.\"\n        }\n      ]\n    },\n    \"healthReasons\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CapabilityHealthReasonList\"\n        },\n\
  \        {\n          \"description\": \"Health reasons for a dataflow endpoint. This field is ignored when calling <code>CreateDataflowEndpointGroup</code>.\"\n        }\n      ]\n    },\n    \"healthStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CapabilityHealth\"\n        },\n        {\n          \"description\": \"A dataflow endpoint health status. This field is ignored when calling <code>CreateDataflowEndpointGroup</code>.\"\n        }\n      ]\n    },\n    \"securityDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityDetails\"\n        },\n        {\n          \"description\": \"Endpoint security details including a list of subnets, a list of security groups and a role to connect streams to instances.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-endpoint-details-schema.json
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: EndpointDetails
---
