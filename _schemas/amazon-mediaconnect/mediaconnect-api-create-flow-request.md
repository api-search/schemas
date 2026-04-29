---
description: Creates a new flow. The request must include one source. The request optionally can include outputs (up to 50) and entitlements (up to 50).
layout: schema
name: CreateFlowRequest
properties_list:
- description: ''
  name: AvailabilityZone
  type: object
- description: ''
  name: Entitlements
  type: object
- description: ''
  name: MediaStreams
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Outputs
  type: object
- description: ''
  name: Source
  type: object
- description: ''
  name: SourceFailoverConfig
  type: object
- description: ''
  name: Sources
  type: object
- description: ''
  name: VpcInterfaces
  type: object
- description: ''
  name: Maintenance
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-create-flow-request-schema.json
slug: mediaconnect-api-create-flow-request
source_filename: mediaconnect-api-create-flow-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-create-flow-request-schema.json\",\n  \"title\": \"CreateFlowRequest\",\n  \"description\": \"Creates a new flow. The request must include one source. The request optionally can include outputs (up to 50) and entitlements (up to 50).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AvailabilityZone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"availabilityZone\"\n          },\n          \"description\": \"The Availability Zone that you want to create the flow in. These options are limited to the Availability Zones within the current AWS Region.\"\n        }\n      ]\n    },\n    \"Entitlements\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfGrantEntitlementRequest\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"entitlements\"\n          },\n          \"description\": \"The entitlements that you want to grant on a flow.\"\n        }\n      ]\n    },\n    \"MediaStreams\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfAddMediaStreamRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaStreams\"\n          },\n          \"description\": \"The media streams that you want to add to the flow. You can associate these media streams with sources and outputs on the flow.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the flow.\"\n        }\n      ]\n    },\n    \"Outputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfAddOutputRequest\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"outputs\"\n          },\n          \"description\": \"The outputs that you want to add to this flow.\"\n        }\n      ]\n    },\n    \"Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SetSourceRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"source\"\n          }\n        }\n      ]\n    },\n    \"SourceFailoverConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailoverConfig\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceFailoverConfig\"\n          }\n        }\n      ]\n    },\n    \"Sources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfSetSourceRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sources\"\n          }\n        }\n      ]\n    },\n    \"VpcInterfaces\": {\n      \"allOf\": [\n        {\n    \
  \      \"$ref\": \"#/components/schemas/__listOfVpcInterfaceRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vpcInterfaces\"\n          },\n          \"description\": \"The VPC interfaces you want on the flow.\"\n        }\n      ]\n    },\n    \"Maintenance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddMaintenance\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenance\"\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-create-flow-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: CreateFlowRequest
---
