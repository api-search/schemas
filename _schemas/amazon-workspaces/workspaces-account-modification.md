---
description: Describes a modification to the configuration of Bring Your Own License (BYOL) for the specified account.
layout: schema
name: AccountModification
properties_list:
- description: ''
  name: ModificationState
  type: object
- description: ''
  name: DedicatedTenancySupport
  type: object
- description: ''
  name: DedicatedTenancyManagementCidrRange
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: ErrorCode
  type: object
- description: ''
  name: ErrorMessage
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-account-modification-schema.json
slug: workspaces-account-modification
source_filename: workspaces-account-modification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ModificationState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DedicatedTenancyModificationStateEnum\"\n        },\n        {\n          \"description\": \"The state of the modification to the configuration of BYOL.\"\n        }\n      ]\n    },\n    \"DedicatedTenancySupport\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DedicatedTenancySupportResultEnum\"\n        },\n        {\n          \"description\": \"The status of BYOL (whether BYOL is being enabled or disabled).\"\n        }\n      ]\n    },\n    \"DedicatedTenancyManagementCidrRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DedicatedTenancyManagementCidrRange\"\n        },\n        {\n          \"description\": \"The IP address range, specified as an IPv4 CIDR block, for the management network interface used for the account.\"\n        }\n      ]\n    },\n\
  \    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp when the modification of the BYOL configuration was started.\"\n        }\n      ]\n    },\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceErrorCode\"\n        },\n        {\n          \"description\": \"The error code that is returned if the configuration of BYOL cannot be modified.\"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The text of the error message that is returned if the configuration of BYOL cannot be modified.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes a modification to the configuration of Bring Your Own License (BYOL) for the specified account. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"AccountModification\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-account-modification-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-account-modification-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: AccountModification
---
