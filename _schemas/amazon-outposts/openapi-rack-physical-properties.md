---
description: Information about the physical and logistical details for racks at sites. For more information about hardware requirements for racks, see <a href="https://docs.aws.amazon.com/outposts/latest/userguide/outposts-requirements.html#checklist">Network readiness checklist</a> in the Amazon Web Services Outposts User Guide.
layout: schema
name: RackPhysicalProperties
properties_list:
- description: ''
  name: PowerDrawKva
  type: object
- description: ''
  name: PowerPhase
  type: object
- description: ''
  name: PowerConnector
  type: object
- description: ''
  name: PowerFeedDrop
  type: object
- description: ''
  name: UplinkGbps
  type: object
- description: ''
  name: UplinkCount
  type: object
- description: ''
  name: FiberOpticCableType
  type: object
- description: ''
  name: OpticalStandard
  type: object
- description: ''
  name: MaximumSupportedWeightLbs
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-rack-physical-properties-schema.json
slug: openapi-rack-physical-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-rack-physical-properties-schema.json\",\n  \"title\": \"RackPhysicalProperties\",\n  \"description\": \" Information about the physical and logistical details for racks at sites. For more information about hardware requirements for racks, see <a href=\\\"https://docs.aws.amazon.com/outposts/latest/userguide/outposts-requirements.html#checklist\\\">Network readiness checklist</a> in the Amazon Web Services Outposts User Guide. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PowerDrawKva\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PowerDrawKva\"\n        },\n        {\n          \"description\": \"The power draw available at the hardware placement position for the rack. \"\n        }\n      ]\n    },\n    \"PowerPhase\": {\n      \"allOf\": [\n       \
  \ {\n          \"$ref\": \"#/components/schemas/PowerPhase\"\n        },\n        {\n          \"description\": \"The power option that you can provide for hardware.\"\n        }\n      ]\n    },\n    \"PowerConnector\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PowerConnector\"\n        },\n        {\n          \"description\": \"The power connector for the hardware. \"\n        }\n      ]\n    },\n    \"PowerFeedDrop\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PowerFeedDrop\"\n        },\n        {\n          \"description\": \"The position of the power feed.\"\n        }\n      ]\n    },\n    \"UplinkGbps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UplinkGbps\"\n        },\n        {\n          \"description\": \"The uplink speed the rack supports for the connection to the Region. \"\n        }\n      ]\n    },\n    \"UplinkCount\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/UplinkCount\"\n        },\n        {\n          \"description\": \"The number of uplinks each Outpost network device.\"\n        }\n      ]\n    },\n    \"FiberOpticCableType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FiberOpticCableType\"\n        },\n        {\n          \"description\": \"The type of fiber used to attach the Outpost to the network. \"\n        }\n      ]\n    },\n    \"OpticalStandard\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OpticalStandard\"\n        },\n        {\n          \"description\": \"The type of optical standard used to attach the Outpost to the network. This field is dependent on uplink speed, fiber type, and distance to the upstream device. For more information about networking requirements for racks, see <a href=\\\"https://docs.aws.amazon.com/outposts/latest/userguide/outposts-requirements.html#facility-networking\\\">Network</a> in the Amazon Web\
  \ Services Outposts User Guide. \"\n        }\n      ]\n    },\n    \"MaximumSupportedWeightLbs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaximumSupportedWeightLbs\"\n        },\n        {\n          \"description\": \"The maximum rack weight that this site can support. <code>NO_LIMIT</code> is over 2000 lbs (907 kg). \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-rack-physical-properties-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: RackPhysicalProperties
---
