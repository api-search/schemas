---
description: UpdateSiteRackPhysicalPropertiesInput schema from Amazon Outposts
layout: schema
name: UpdateSiteRackPhysicalPropertiesInput
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
schema_file: json-schema/openapi-update-site-rack-physical-properties-input-schema.json
slug: openapi-update-site-rack-physical-properties-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-update-site-rack-physical-properties-input-schema.json\",\n  \"title\": \"UpdateSiteRackPhysicalPropertiesInput\",\n  \"description\": \"UpdateSiteRackPhysicalPropertiesInput schema from Amazon Outposts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PowerDrawKva\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PowerDrawKva\"\n        },\n        {\n          \"description\": \"The power draw, in kVA, available at the hardware placement position for the rack.\"\n        }\n      ]\n    },\n    \"PowerPhase\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PowerPhase\"\n        },\n        {\n          \"description\": \"<p>The power option that you can provide for hardware. </p> <ul> <li> <p>Single-phase AC feed: 200 V to 277\
  \ V, 50 Hz or 60 Hz</p> </li> <li> <p>Three-phase AC feed: 346 V to 480 V, 50 Hz or 60 Hz</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"PowerConnector\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PowerConnector\"\n        },\n        {\n          \"description\": \"<p>The power connector that Amazon Web Services should plan to provide for connections to the hardware. Note the correlation between <code>PowerPhase</code> and <code>PowerConnector</code>. </p> <ul> <li> <p>Single-phase AC feed</p> <ul> <li> <p> <b>L6-30P</b> \\u2013 (common in US); 30A; single phase</p> </li> <li> <p> <b>IEC309 (blue)</b> \\u2013 P+N+E, 6hr; 32 A; single phase</p> </li> </ul> </li> <li> <p>Three-phase AC feed</p> <ul> <li> <p> <b>AH530P7W (red)</b> \\u2013 3P+N+E, 7hr; 30A; three phase</p> </li> <li> <p> <b>AH532P6W (red)</b> \\u2013 3P+N+E, 6hr; 32A; three phase</p> </li> </ul> </li> </ul>\"\n        }\n      ]\n    },\n    \"PowerFeedDrop\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/PowerFeedDrop\"\n        },\n        {\n          \"description\": \"Indicates whether the power feed comes above or below the rack. \"\n        }\n      ]\n    },\n    \"UplinkGbps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UplinkGbps\"\n        },\n        {\n          \"description\": \"The uplink speed the rack should support for the connection to the Region. \"\n        }\n      ]\n    },\n    \"UplinkCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UplinkCount\"\n        },\n        {\n          \"description\": \"<p>Racks come with two Outpost network devices. Depending on the supported uplink speed at the site, the Outpost network devices provide a variable number of uplinks. Specify the number of uplinks for each Outpost network device that you intend to use to connect the rack to your network. Note the correlation between <code>UplinkGbps</code> and\
  \ <code>UplinkCount</code>. </p> <ul> <li> <p>1Gbps - Uplinks available: 1, 2, 4, 6, 8</p> </li> <li> <p>10Gbps - Uplinks available: 1, 2, 4, 8, 12, 16</p> </li> <li> <p>40 and 100 Gbps- Uplinks available: 1, 2, 4</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"FiberOpticCableType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FiberOpticCableType\"\n        },\n        {\n          \"description\": \"The type of fiber that you will use to attach the Outpost to your network. \"\n        }\n      ]\n    },\n    \"OpticalStandard\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OpticalStandard\"\n        },\n        {\n          \"description\": \"<p>The type of optical standard that you will use to attach the Outpost to your network. This field is dependent on uplink speed, fiber type, and distance to the upstream device. For more information about networking requirements for racks, see <a href=\\\"https://docs.aws.amazon.com/outposts/latest/userguide/outposts-requirements.html#facility-networking\\\
  \">Network</a> in the Amazon Web Services Outposts User Guide. </p> <ul> <li> <p> <code>OPTIC_10GBASE_SR</code>: 10GBASE-SR</p> </li> <li> <p> <code>OPTIC_10GBASE_IR</code>: 10GBASE-IR</p> </li> <li> <p> <code>OPTIC_10GBASE_LR</code>: 10GBASE-LR</p> </li> <li> <p> <code>OPTIC_40GBASE_SR</code>: 40GBASE-SR</p> </li> <li> <p> <code>OPTIC_40GBASE_ESR</code>: 40GBASE-ESR</p> </li> <li> <p> <code>OPTIC_40GBASE_IR4_LR4L</code>: 40GBASE-IR (LR4L)</p> </li> <li> <p> <code>OPTIC_40GBASE_LR4</code>: 40GBASE-LR4</p> </li> <li> <p> <code>OPTIC_100GBASE_SR4</code>: 100GBASE-SR4</p> </li> <li> <p> <code>OPTIC_100GBASE_CWDM4</code>: 100GBASE-CWDM4</p> </li> <li> <p> <code>OPTIC_100GBASE_LR4</code>: 100GBASE-LR4</p> </li> <li> <p> <code>OPTIC_100G_PSM4_MSA</code>: 100G PSM4 MSA</p> </li> <li> <p> <code>OPTIC_1000BASE_LX</code>: 1000Base-LX</p> </li> <li> <p> <code>OPTIC_1000BASE_SX</code> : 1000Base-SX</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"MaximumSupportedWeightLbs\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/MaximumSupportedWeightLbs\"\n        },\n        {\n          \"description\": \"The maximum rack weight that this site can support. <code>NO_LIMIT</code> is over 2000lbs. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-update-site-rack-physical-properties-input-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: UpdateSiteRackPhysicalPropertiesInput
---
