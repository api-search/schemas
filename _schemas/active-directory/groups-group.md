---
description: A Microsoft Entra security group or Microsoft 365 group managed via Microsoft Graph
layout: schema
name: Group
properties_list:
- description: Unique identifier for the group object (read-only)
  name: id
  type: string
- description: Display name for the group
  name: displayName
  type: string
- description: Optional description for the group
  name: description
  type:
  - string
  - 'null'
- description: SMTP address for the group
  name: mail
  type:
  - string
  - 'null'
- description: Mail alias for the group (without domain suffix)
  name: mailNickname
  type: string
- description: Specifies whether the group is mail-enabled
  name: mailEnabled
  type: boolean
- description: Specifies whether the group is a security group
  name: securityEnabled
  type: boolean
- description: Collection specifying the group type and dynamic membership. Unified = Microsoft 365 group.
  name: groupTypes
  type: array
- description: Visibility of a Microsoft 365 group content and members list
  name: visibility
  type:
  - string
  - 'null'
- description: Rule defining dynamic group membership (requires DynamicMembership in groupTypes)
  name: membershipRule
  type:
  - string
  - 'null'
- description: Indicates whether dynamic membership processing is on or paused
  name: membershipRuleProcessingState
  type:
  - string
  - 'null'
- description: True if the group is synced from on-premises Active Directory
  name: onPremisesSyncEnabled
  type:
  - boolean
  - 'null'
- description: Distinguished name from on-premises AD
  name: onPremisesDistinguishedName
  type:
  - string
  - 'null'
- description: Timestamp when the group was created
  name: createdDateTime
  type:
  - string
  - 'null'
- description: Timestamp when the Microsoft 365 group was last renewed
  name: renewedDateTime
  type:
  - string
  - 'null'
- description: Timestamp when the group expires (requires an expiration policy)
  name: expirationDateTime
  type:
  - string
  - 'null'
- description: Preferred data location for multi-geo tenant (e.g. CAN, EUR)
  name: preferredDataLocation
  type:
  - string
  - 'null'
- description: Resources provisioned (e.g. Team for Microsoft Teams-enabled groups)
  name: resourceProvisioningOptions
  type: array
provider_name: Microsoft Active Directory
provider_slug: active-directory
schema_file: json-schema/groups-group-schema.json
slug: groups-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/active-directory/main/json-schema/groups-group-schema.json\",\n  \"title\": \"Group\",\n  \"description\": \"A Microsoft Entra security group or Microsoft 365 group managed via Microsoft Graph\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the group object (read-only)\",\n      \"readOnly\": true\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the group\",\n      \"maxLength\": 256\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Optional description for the group\",\n      \"maxLength\": 1024\n    },\n    \"mail\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"email\",\n      \"description\": \"SMTP address\
  \ for the group\",\n      \"readOnly\": true\n    },\n    \"mailNickname\": {\n      \"type\": \"string\",\n      \"description\": \"Mail alias for the group (without domain suffix)\",\n      \"maxLength\": 64\n    },\n    \"mailEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether the group is mail-enabled\"\n    },\n    \"securityEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether the group is a security group\"\n    },\n    \"groupTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"Unified\", \"DynamicMembership\"]\n      },\n      \"description\": \"Collection specifying the group type and dynamic membership. Unified = Microsoft 365 group.\"\n    },\n    \"visibility\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Visibility of a Microsoft 365 group content and members list\",\n      \"enum\": [\"Public\", \"Private\", \"HiddenMembership\"\
  , null]\n    },\n    \"membershipRule\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Rule defining dynamic group membership (requires DynamicMembership in groupTypes)\"\n    },\n    \"membershipRuleProcessingState\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Indicates whether dynamic membership processing is on or paused\",\n      \"enum\": [\"On\", \"Paused\", null]\n    },\n    \"onPremisesSyncEnabled\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"True if the group is synced from on-premises Active Directory\",\n      \"readOnly\": true\n    },\n    \"onPremisesDistinguishedName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Distinguished name from on-premises AD\",\n      \"readOnly\": true\n    },\n    \"createdDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the group was created\",\n      \"readOnly\"\
  : true\n    },\n    \"renewedDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the Microsoft 365 group was last renewed\",\n      \"readOnly\": true\n    },\n    \"expirationDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the group expires (requires an expiration policy)\",\n      \"readOnly\": true\n    },\n    \"preferredDataLocation\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Preferred data location for multi-geo tenant (e.g. CAN, EUR)\"\n    },\n    \"resourceProvisioningOptions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Resources provisioned (e.g. Team for Microsoft Teams-enabled groups)\"\n    }\n  },\n  \"required\": [\"displayName\", \"mailEnabled\", \"mailNickname\", \"securityEnabled\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/active-directory/refs/heads/main/json-schema/groups-group-schema.json
tags:
- Active Directory
- Authentication
- Authorization
- Directory Services
- Identity Management
- Microsoft Entra
- Zero Trust
title: Group
---
