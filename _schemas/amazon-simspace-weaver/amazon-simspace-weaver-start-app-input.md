---
description: StartAppInput schema from Amazon SimSpace Weaver API
layout: schema
name: StartAppInput
properties_list:
- description: ''
  name: ClientToken
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Domain
  type: object
- description: ''
  name: LaunchOverrides
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Simulation
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-start-app-input-schema.json
slug: amazon-simspace-weaver-start-app-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-start-app-input-schema.json\",\n  \"title\": \"StartAppInput\",\n  \"description\": \"StartAppInput schema from Amazon SimSpace Weaver API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A value that you provide to ensure that repeated calls to this API operation using the same parameters complete only once. A <code>ClientToken</code> is also known as an <i>idempotency token</i>. A <code>ClientToken</code> expires after 24 hours.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\"\
  : \"The description of the app.\"\n        }\n      ]\n    },\n    \"Domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimSpaceWeaverResourceName\"\n        },\n        {\n          \"description\": \"The name of the domain of the app.\"\n        }\n      ]\n    },\n    \"LaunchOverrides\": {\n      \"$ref\": \"#/components/schemas/LaunchOverrides\"\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimSpaceWeaverResourceName\"\n        },\n        {\n          \"description\": \"The name of the app.\"\n        }\n      ]\n    },\n    \"Simulation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimSpaceWeaverResourceName\"\n        },\n        {\n          \"description\": \"The name of the simulation of the app.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Domain\",\n    \"Name\",\n    \"Simulation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-start-app-input-schema.json
tags:
- AWS
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: StartAppInput
---
