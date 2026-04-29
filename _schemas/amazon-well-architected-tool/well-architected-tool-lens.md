---
description: A lens return object.
layout: schema
name: Lens
properties_list:
- description: ''
  name: LensArn
  type: object
- description: ''
  name: LensVersion
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Owner
  type: object
- description: ''
  name: ShareInvitationId
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-lens-schema.json
slug: well-architected-tool-lens
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"LensArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensArn\"\n        },\n        {\n          \"description\": \"The ARN of a lens.\"\n        }\n      ]\n    },\n    \"LensVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensVersion\"\n        },\n        {\n          \"description\": \"The version of a lens.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"$ref\": \"#/components/schemas/LensName\"\n    },\n    \"Description\": {\n      \"$ref\": \"#/components/schemas/LensDescription\"\n    },\n    \"Owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LensOwner\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID that owns the lens.\"\n        }\n      ]\n    },\n    \"ShareInvitationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShareInvitationId\"\
  \n        },\n        {\n          \"description\": \"The ID assigned to the share invitation.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags assigned to the lens.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A lens return object.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Lens\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-lens-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-lens-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: Lens
---
