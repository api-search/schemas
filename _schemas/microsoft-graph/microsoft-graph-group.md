---
description: Represents a Microsoft Entra ID group, which can be a Microsoft 365 group, a security group, a mail-enabled security group, or a distribution group. Groups are used to manage collections of users and other directory objects for access control, collaboration, and resource sharing across Microsoft 365 services including Teams, SharePoint, Outlook, Planner, and OneDrive.
layout: schema
name: Microsoft Graph Group
properties_list:
- description: The unique identifier for the group. Inherited from directoryObject. Read-only.
  name: id
  type: string
- description: The name to display in the address book for the group. Required during creation and cannot be cleared during updates.
  name: displayName
  type: string
- description: An optional description for the group.
  name: description
  type:
  - string
  - 'null'
- description: The SMTP address for the group, for example 'serviceadmins@contoso.com'. Read-only.
  name: mail
  type:
  - string
  - 'null'
- description: Specifies whether the group is mail-enabled. Required during creation.
  name: mailEnabled
  type: boolean
- description: The mail alias for the group, unique for Microsoft 365 groups in the organization. Required during creation.
  name: mailNickname
  type: string
- description: Specifies whether the group is a security group. Required during creation.
  name: securityEnabled
  type: boolean
- description: Specifies the group type and its membership. If the collection contains 'Unified', the group is a Microsoft 365 group. If it contains 'DynamicMembership', the group has dynamic membership.
  name: groupTypes
  type: array
- description: Specifies the visibility of a Microsoft 365 group. If visibility is not specified during group creation, the group is created as Public by default.
  name: visibility
  type:
  - string
  - 'null'
- description: Describes a classification for the group (such as low, medium, or high business impact).
  name: classification
  type:
  - string
  - 'null'
- description: Timestamp of when the group was created. Read-only.
  name: createdDateTime
  type: string
- description: Timestamp of when the group was last renewed. This cannot be modified directly and is only updated via the renew service action. Read-only.
  name: renewedDateTime
  type: string
- description: Timestamp of when the group is set to expire. Read-only.
  name: expirationDateTime
  type:
  - string
  - 'null'
- description: Indicates whether this group can be assigned to a Microsoft Entra role. This property can only be set when creating the group and is immutable.
  name: isAssignableToRole
  type:
  - boolean
  - 'null'
- description: The rule that determines members for this group if the group is a dynamic group.
  name: membershipRule
  type:
  - string
  - 'null'
- description: Indicates whether the dynamic membership processing is on or paused.
  name: membershipRuleProcessingState
  type:
  - string
  - 'null'
- description: The preferred data location for the Microsoft 365 group.
  name: preferredDataLocation
  type:
  - string
  - 'null'
- description: The preferred language for a Microsoft 365 group.
  name: preferredLanguage
  type:
  - string
  - 'null'
- description: 'Email addresses for the group that direct to the same group mailbox. For example: [''SMTP:bob@contoso.com'', ''smtp:bob@sales.contoso.com'']. Read-only.'
  name: proxyAddresses
  type: array
- description: Specifies a Microsoft 365 group's color theme.
  name: theme
  type:
  - string
  - 'null'
- description: Specifies the group resources that are provisioned as part of Microsoft 365 group creation.
  name: resourceProvisioningOptions
  type: array
- description: True if this group is synced from an on-premises directory; false if this group was originally synced from an on-premises directory but is no longer synced. Read-only.
  name: onPremisesSyncEnabled
  type:
  - boolean
  - 'null'
- description: The last time at which the group was synced with the on-premises directory. Read-only.
  name: onPremisesLastSyncDateTime
  type:
  - string
  - 'null'
- description: The date and time the group was soft-deleted. Read-only.
  name: deletedDateTime
  type:
  - string
  - 'null'
provider_name: Microsoft Graph
provider_slug: microsoft-graph
schema_file: json-schema/microsoft-graph-group-schema.json
slug: microsoft-graph-group
source_filename: microsoft-graph-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.api.gov/microsoft-graph/group\",\n  \"title\": \"Microsoft Graph Group\",\n  \"description\": \"Represents a Microsoft Entra ID group, which can be a Microsoft 365 group, a security group, a mail-enabled security group, or a distribution group. Groups are used to manage collections of users and other directory objects for access control, collaboration, and resource sharing across Microsoft 365 services including Teams, SharePoint, Outlook, Planner, and OneDrive.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"displayName\",\n    \"mailEnabled\",\n    \"mailNickname\",\n    \"securityEnabled\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the group. Inherited from directoryObject. Read-only.\",\n      \"readOnly\": true,\n      \"examples\": [\n        \"45b7d2e7-b882-4a80-ba97-10b7a63b8fa4\"\n   \
  \   ]\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The name to display in the address book for the group. Required during creation and cannot be cleared during updates.\",\n      \"maxLength\": 256,\n      \"examples\": [\n        \"All Company\"\n      ]\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"An optional description for the group.\",\n      \"maxLength\": 1024\n    },\n    \"mail\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The SMTP address for the group, for example 'serviceadmins@contoso.com'. Read-only.\",\n      \"format\": \"email\",\n      \"readOnly\": true\n    },\n    \"mailEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether the group is mail-enabled. Required during creation.\"\n    },\n    \"mailNickname\": {\n      \"type\": \"string\",\n      \"description\": \"The mail alias for the group, unique for Microsoft\
  \ 365 groups in the organization. Required during creation.\",\n      \"maxLength\": 64,\n      \"pattern\": \"^[^@\\\\s]+$\",\n      \"examples\": [\n        \"allcompany\"\n      ]\n    },\n    \"securityEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether the group is a security group. Required during creation.\"\n    },\n    \"groupTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Specifies the group type and its membership. If the collection contains 'Unified', the group is a Microsoft 365 group. If it contains 'DynamicMembership', the group has dynamic membership.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"Unified\",\n          \"DynamicMembership\"\n        ]\n      },\n      \"examples\": [\n        [\"Unified\"]\n      ]\n    },\n    \"visibility\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Specifies the visibility of a Microsoft 365 group. If visibility is\
  \ not specified during group creation, the group is created as Public by default.\",\n      \"enum\": [\"Public\", \"Private\", \"HiddenMembership\", null]\n    },\n    \"classification\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Describes a classification for the group (such as low, medium, or high business impact).\"\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of when the group was created. Read-only.\",\n      \"readOnly\": true\n    },\n    \"renewedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of when the group was last renewed. This cannot be modified directly and is only updated via the renew service action. Read-only.\",\n      \"readOnly\": true\n    },\n    \"expirationDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of\
  \ when the group is set to expire. Read-only.\",\n      \"readOnly\": true\n    },\n    \"isAssignableToRole\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Indicates whether this group can be assigned to a Microsoft Entra role. This property can only be set when creating the group and is immutable.\"\n    },\n    \"membershipRule\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The rule that determines members for this group if the group is a dynamic group.\"\n    },\n    \"membershipRuleProcessingState\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Indicates whether the dynamic membership processing is on or paused.\",\n      \"enum\": [\"On\", \"Paused\", null]\n    },\n    \"preferredDataLocation\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The preferred data location for the Microsoft 365 group.\"\n    },\n    \"preferredLanguage\": {\n      \"type\": [\"string\", \"null\"],\n     \
  \ \"description\": \"The preferred language for a Microsoft 365 group.\"\n    },\n    \"proxyAddresses\": {\n      \"type\": \"array\",\n      \"description\": \"Email addresses for the group that direct to the same group mailbox. For example: ['SMTP:bob@contoso.com', 'smtp:bob@sales.contoso.com']. Read-only.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"theme\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Specifies a Microsoft 365 group's color theme.\",\n      \"enum\": [\n        \"Teal\", \"Purple\", \"Green\", \"Blue\", \"Pink\",\n        \"Orange\", \"Red\", null\n      ]\n    },\n    \"resourceProvisioningOptions\": {\n      \"type\": \"array\",\n      \"description\": \"Specifies the group resources that are provisioned as part of Microsoft 365 group creation.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [\n        [\"Team\"]\n      ]\n    },\n    \"onPremisesSyncEnabled\"\
  : {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"True if this group is synced from an on-premises directory; false if this group was originally synced from an on-premises directory but is no longer synced. Read-only.\",\n      \"readOnly\": true\n    },\n    \"onPremisesLastSyncDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The last time at which the group was synced with the on-premises directory. Read-only.\",\n      \"readOnly\": true\n    },\n    \"deletedDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the group was soft-deleted. Read-only.\",\n      \"readOnly\": true\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-graph/refs/heads/main/json-schema/microsoft-graph-group-schema.json
tags:
- Azure AD
- Collaboration
- Contacts
- Documents
- Email
- Graph
- Identity
- Microsoft
- Office 365
- Presentations
- Productivity
- Spreadsheets
- T1
- Tasks
title: Microsoft Graph Group
---
