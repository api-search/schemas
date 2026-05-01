---
description: Describes the related WorkSpace. The related WorkSpace could be a standby WorkSpace or primary WorkSpace related to the specified WorkSpace.
layout: schema
name: RelatedWorkspaceProperties
properties_list:
- description: ''
  name: WorkspaceId
  type: object
- description: ''
  name: Region
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-related-workspace-properties-schema.json
slug: workspaces-related-workspace-properties
source_filename: workspaces-related-workspace-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"WorkspaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceId\"\n        },\n        {\n          \"description\": \"The identifier of the related WorkSpace.\"\n        }\n      ]\n    },\n    \"Region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Region\"\n        },\n        {\n          \"description\": \"The Region of the related WorkSpace.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceState\"\n        },\n        {\n          \"description\": \"Indicates the state of the WorkSpace.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StandbyWorkspaceRelationshipType\"\n        },\n        {\n          \"description\": \"Indicates the type of WorkSpace.\"\n        }\n      ]\n    }\n  },\n\
  \  \"description\": \"Describes the related WorkSpace. The related WorkSpace could be a standby WorkSpace or primary WorkSpace related to the specified WorkSpace.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RelatedWorkspaceProperties\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-related-workspace-properties-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-related-workspace-properties-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: RelatedWorkspaceProperties
---
