---
description: The settings for a flow, including its source, outputs, and entitlements.
layout: schema
name: Flow
properties_list:
- description: ''
  name: AvailabilityZone
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: EgressIp
  type: object
- description: ''
  name: Entitlements
  type: object
- description: ''
  name: FlowArn
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
  name: Status
  type: object
- description: ''
  name: VpcInterfaces
  type: object
- description: ''
  name: Maintenance
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-flow-schema.json
slug: mediaconnect-api-flow
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-flow-schema.json\",\n  \"title\": \"Flow\",\n  \"description\": \"The settings for a flow, including its source, outputs, and entitlements.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AvailabilityZone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"availabilityZone\"\n          },\n          \"description\": \"The Availability Zone that you want to create the flow in. These options are limited to the Availability Zones within the current AWS.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\
  \n          },\n          \"description\": \"A description of the flow. This value is not used or seen outside of the current AWS Elemental MediaConnect account.\"\n        }\n      ]\n    },\n    \"EgressIp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"egressIp\"\n          },\n          \"description\": \"The IP address from which video will be sent to output destinations.\"\n        }\n      ]\n    },\n    \"Entitlements\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfEntitlement\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"entitlements\"\n          },\n          \"description\": \"The entitlements in this flow.\"\n        }\n      ]\n    },\n    \"FlowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"\
  name\": \"flowArn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) of the flow.\"\n        }\n      ]\n    },\n    \"MediaStreams\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfMediaStream\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mediaStreams\"\n          },\n          \"description\": \"The media streams that are associated with the flow. After you associate a media stream with a source, you can also associate it with outputs on the flow.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the flow.\"\n        }\n      ]\n    },\n    \"Outputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfOutput\"\n        },\n        {\n          \"xml\"\
  : {\n            \"name\": \"outputs\"\n          },\n          \"description\": \"The outputs in this flow.\"\n        }\n      ]\n    },\n    \"Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Source\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"source\"\n          }\n        }\n      ]\n    },\n    \"SourceFailoverConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailoverConfig\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceFailoverConfig\"\n          }\n        }\n      ]\n    },\n    \"Sources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfSource\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sources\"\n          }\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Status\"\n        },\n        {\n          \"xml\":\
  \ {\n            \"name\": \"status\"\n          },\n          \"description\": \"The current status of the flow.\"\n        }\n      ]\n    },\n    \"VpcInterfaces\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfVpcInterface\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vpcInterfaces\"\n          },\n          \"description\": \"The VPC Interfaces for this flow.\"\n        }\n      ]\n    },\n    \"Maintenance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Maintenance\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenance\"\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Status\",\n    \"AvailabilityZone\",\n    \"Source\",\n    \"Name\",\n    \"Entitlements\",\n    \"Outputs\",\n    \"FlowArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-flow-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: Flow
---
