---
description: Represents an Azure Active Directory group. Can be a Microsoft 365 group, a security group, a mail-enabled security group, or a distribution group.
layout: schema
name: Group
properties_list:
- description: The unique identifier for the group.
  name: id
  type: string
- description: The display name for the group.
  name: displayName
  type: string
- description: An optional description for the group.
  name: description
  type: string
- description: The SMTP address for the group.
  name: mail
  type: string
- description: Specifies whether the group is mail-enabled.
  name: mailEnabled
  type: boolean
- description: The mail alias for the group, unique for Microsoft 365 groups in the organization.
  name: mailNickname
  type: string
- description: Specifies whether the group is a security group.
  name: securityEnabled
  type: boolean
- description: Specifies the group type and its membership. If the collection includes "Unified", the group is a Microsoft 365 group.
  name: groupTypes
  type: array
- description: Specifies the visibility of a Microsoft 365 group. Default value is Public.
  name: visibility
  type: string
- description: Timestamp of when the group was created.
  name: createdDateTime
  type: string
- description: Timestamp of when the group was last renewed.
  name: renewedDateTime
  type: string
- description: Describes a classification for the group (such as low, medium, or high business impact).
  name: classification
  type: string
- description: The rule that determines members for this group if the group is a dynamic group.
  name: membershipRule
  type: string
- description: Whether dynamic membership processing is on or paused.
  name: membershipRuleProcessingState
  type: string
- description: Specifies the group resources provisioned as part of Microsoft 365 group creation (e.g., Team).
  name: resourceProvisioningOptions
  type: array
- description: Direct members of this group.
  name: members
  type: array
- description: The owners of the group.
  name: owners
  type: array
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-group-schema.json
slug: microsoft-graph-group
source_filename: microsoft-graph-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Group\",\n  \"type\": \"object\",\n  \"description\": \"Represents an Azure Active Directory group. Can be a Microsoft 365 group, a security group, a mail-enabled security group, or a distribution group.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the group.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name for the group.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"An optional description for the group.\"\n    },\n    \"mail\": {\n      \"type\": \"string\",\n      \"description\": \"The SMTP address for the group.\"\n    },\n    \"mailEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether the group is mail-enabled.\"\n    },\n    \"mailNickname\": {\n      \"type\": \"string\",\n     \
  \ \"description\": \"The mail alias for the group, unique for Microsoft 365 groups in the organization.\"\n    },\n    \"securityEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether the group is a security group.\"\n    },\n    \"groupTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Specifies the group type and its membership. If the collection includes \\\"Unified\\\", the group is a Microsoft 365 group.\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the visibility of a Microsoft 365 group. Default value is Public.\"\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of when the group was created.\"\n    },\n    \"renewedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of when the group was last renewed.\"\n    },\n    \"classification\": {\n      \"type\": \"string\",\n      \"description\": \"Describes a\
  \ classification for the group (such as low, medium, or high business impact).\"\n    },\n    \"membershipRule\": {\n      \"type\": \"string\",\n      \"description\": \"The rule that determines members for this group if the group is a dynamic group.\"\n    },\n    \"membershipRuleProcessingState\": {\n      \"type\": \"string\",\n      \"description\": \"Whether dynamic membership processing is on or paused.\"\n    },\n    \"resourceProvisioningOptions\": {\n      \"type\": \"array\",\n      \"description\": \"Specifies the group resources provisioned as part of Microsoft 365 group creation (e.g., Team).\"\n    },\n    \"members\": {\n      \"type\": \"array\",\n      \"description\": \"Direct members of this group.\"\n    },\n    \"owners\": {\n      \"type\": \"array\",\n      \"description\": \"The owners of the group.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-group-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: Group
---
