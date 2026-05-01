---
description: Input for List Share Invitations
layout: schema
name: ListShareInvitationsOutput
properties_list:
- description: ''
  name: ShareInvitationSummaries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-list-share-invitations-output-schema.json
slug: well-architected-tool-list-share-invitations-output
source_filename: well-architected-tool-list-share-invitations-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ShareInvitationSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShareInvitationSummaries\"\n        },\n        {\n          \"description\": \"List of share invitation summaries in a workload.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/NextToken\"\n    }\n  },\n  \"description\": \"Input for List Share Invitations\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListShareInvitationsOutput\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-share-invitations-output-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-list-share-invitations-output-schema.json
tags:
- Architecture
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ListShareInvitationsOutput
---
