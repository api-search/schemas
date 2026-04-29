---
description: Information about compute hardware assets.
layout: schema
name: ComputeAttributes
properties_list:
- description: ''
  name: HostId
  type: object
- description: ''
  name: State
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-compute-attributes-schema.json
slug: openapi-compute-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-compute-attributes-schema.json\",\n  \"title\": \"ComputeAttributes\",\n  \"description\": \" Information about compute hardware assets. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HostId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HostId\"\n        },\n        {\n          \"description\": \" The host ID of the Dedicated Host on the asset. \"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeAssetState\"\n        },\n        {\n          \"description\": \"<p>The state.</p> <ul> <li> <p>ACTIVE - The asset is available and can provide capacity for new compute resources.</p> </li> <li> <p>ISOLATED - The asset is undergoing maintenance and can't provide capacity for new compute\
  \ resources. Existing compute resources on the asset are not affected.</p> </li> <li> <p>RETIRING - The underlying hardware for the asset is degraded. Capacity for new compute resources is reduced. Amazon Web Services sends notifications for resources that must be stopped before the asset can be replaced.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-compute-attributes-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: ComputeAttributes
---
