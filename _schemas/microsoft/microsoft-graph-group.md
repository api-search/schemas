---
description: Represents a Microsoft Entra group, which can be a Microsoft 365 group, security group, or mail-enabled security group. Inherits from directoryObject. This is an open type that allows additional properties beyond those documented.
layout: schema
name: Microsoft Graph Group
properties_list:
- description: Unique identifier for the group (GUID). Inherited from directoryObject.
  name: id
  type: string
- description: The display name for the group. Required when creating and cannot be cleared during updates.
  name: displayName
  type: string
- description: An optional description for the group
  name: description
  type:
  - string
  - 'null'
- description: The SMTP address for the group
  name: mail
  type:
  - string
  - 'null'
- description: Specifies whether the group is mail-enabled
  name: mailEnabled
  type: boolean
- description: The mail alias for the group, unique for Microsoft 365 groups in the organization
  name: mailNickname
  type: string
- description: Specifies whether the group is a security group
  name: securityEnabled
  type: boolean
- description: Specifies the group type and its membership. If the collection contains 'Unified', the group is a Microsoft 365 group; if it includes 'DynamicMembership', the group has dynamic membership.
  name: groupTypes
  type: array
- description: Specifies the group join policy and group content visibility
  name: visibility
  type:
  - string
  - 'null'
- description: Describes a classification for the group (such as low, medium, or high business impact)
  name: classification
  type:
  - string
  - 'null'
- description: Specifies a Microsoft 365 group's color theme
  name: theme
  type:
  - string
  - 'null'
- description: Timestamp of when the group was created in ISO 8601 format and UTC
  name: createdDateTime
  type:
  - string
  - 'null'
- description: The date and time the group was deleted
  name: deletedDateTime
  type:
  - string
  - 'null'
- description: Timestamp of when the group was last renewed
  name: renewedDateTime
  type:
  - string
  - 'null'
- description: Timestamp of when the group is set to expire
  name: expirationDateTime
  type:
  - string
  - 'null'
- description: The rule that determines members for this group if the group is a dynamic group
  name: membershipRule
  type:
  - string
  - 'null'
- description: Indicates whether dynamic membership processing is on or paused
  name: membershipRuleProcessingState
  type:
  - string
  - 'null'
- description: Indicates whether this group can be assigned to a Microsoft Entra role
  name: isAssignableToRole
  type:
  - boolean
  - 'null'
- description: When a group is associated with a team, this determines whether the team is in read-only mode
  name: isArchived
  type:
  - boolean
  - 'null'
- description: Indicates whether the group is a member of a restricted management administrative unit
  name: isManagementRestricted
  type:
  - boolean
  - 'null'
- description: The preferred data location for the Microsoft 365 group
  name: preferredDataLocation
  type:
  - string
  - 'null'
- description: The preferred language for a Microsoft 365 group in ISO 639-1 format
  name: preferredLanguage
  type:
  - string
  - 'null'
- description: Email addresses for the group that direct to the same group mailbox
  name: proxyAddresses
  type: array
- description: Security identifier of the group, used in Windows scenarios
  name: securityIdentifier
  type:
  - string
  - 'null'
- description: The unique identifier that can be assigned to a group and used as an alternate key
  name: uniqueName
  type:
  - string
  - 'null'
- description: Contains the on-premises domain FQDN
  name: onPremisesDomainName
  type:
  - string
  - 'null'
- description: Indicates the last time at which the group was synced with the on-premises directory
  name: onPremisesLastSyncDateTime
  type:
  - string
  - 'null'
- description: Contains the on-premises netBios name
  name: onPremisesNetBiosName
  type:
  - string
  - 'null'
- description: Contains the on-premises SAM account name
  name: onPremisesSamAccountName
  type:
  - string
  - 'null'
- description: Contains the on-premises security identifier (SID) for the group
  name: onPremisesSecurityIdentifier
  type:
  - string
  - 'null'
- description: True if this group is synced from an on-premises directory
  name: onPremisesSyncEnabled
  type:
  - boolean
  - 'null'
- description: Errors when using Microsoft synchronization product during provisioning
  name: onPremisesProvisioningErrors
  type: array
- description: Indicates if people external to the organization can send messages to the group
  name: allowExternalSenders
  type:
  - boolean
  - 'null'
- description: Indicates if new members added to the group are auto-subscribed to receive email notifications
  name: autoSubscribeNewMembers
  type:
  - boolean
  - 'null'
- description: True if the group is not displayed in certain parts of the Outlook UI
  name: hideFromAddressLists
  type:
  - boolean
  - 'null'
- description: True if the group is not displayed in Outlook clients
  name: hideFromOutlookClients
  type:
  - boolean
  - 'null'
- description: Indicates whether the signed-in user is subscribed to receive email conversations
  name: isSubscribedByMail
  type:
  - boolean
  - 'null'
- description: Indicates whether there are members in this group that have license errors
  name: hasMembersWithLicenseErrors
  type:
  - boolean
  - 'null'
- description: Count of conversations that received new posts since the signed-in user last visited the group
  name: unseenCount
  type:
  - integer
  - 'null'
- description: Specifies the group behaviors that can be set during creation
  name: resourceBehaviorOptions
  type: array
- description: Specifies the group resources associated with the Microsoft 365 group
  name: resourceProvisioningOptions
  type: array
- description: The licenses that are assigned to the group
  name: assignedLicenses
  type: array
- description: The list of sensitivity label pairs associated with a Microsoft 365 group
  name: assignedLabels
  type: array
provider_name: Microsoft
provider_slug: microsoft
schema_file: json-schema/microsoft-graph-group-schema.json
slug: microsoft-graph-group
source_filename: microsoft-graph-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://learn.microsoft.com/en-us/graph/schemas/microsoft/group.json\",\n  \"title\": \"Microsoft Graph Group\",\n  \"description\": \"Represents a Microsoft Entra group, which can be a Microsoft 365 group, security group, or mail-enabled security group. Inherits from directoryObject. This is an open type that allows additional properties beyond those documented.\",\n  \"type\": \"object\",\n  \"required\": [\"displayName\", \"mailEnabled\", \"mailNickname\", \"securityEnabled\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the group (GUID). Inherited from directoryObject.\",\n      \"readOnly\": true\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name for the group. Required when creating and cannot be cleared during updates.\",\n      \"maxLength\": 256\n    },\n    \"description\"\
  : {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"An optional description for the group\"\n    },\n    \"mail\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"email\",\n      \"description\": \"The SMTP address for the group\",\n      \"readOnly\": true\n    },\n    \"mailEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether the group is mail-enabled\"\n    },\n    \"mailNickname\": {\n      \"type\": \"string\",\n      \"description\": \"The mail alias for the group, unique for Microsoft 365 groups in the organization\",\n      \"maxLength\": 64\n    },\n    \"securityEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether the group is a security group\"\n    },\n    \"groupTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Specifies the group type and its membership. If the collection contains 'Unified', the group\
  \ is a Microsoft 365 group; if it includes 'DynamicMembership', the group has dynamic membership.\"\n    },\n    \"visibility\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [null, \"Public\", \"Private\", \"HiddenMembership\"],\n      \"description\": \"Specifies the group join policy and group content visibility\"\n    },\n    \"classification\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Describes a classification for the group (such as low, medium, or high business impact)\"\n    },\n    \"theme\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [null, \"Teal\", \"Purple\", \"Green\", \"Blue\", \"Pink\", \"Orange\", \"Red\"],\n      \"description\": \"Specifies a Microsoft 365 group's color theme\"\n    },\n    \"createdDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of when the group was created in ISO 8601 format and UTC\",\n      \"readOnly\": true\n\
  \    },\n    \"deletedDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the group was deleted\",\n      \"readOnly\": true\n    },\n    \"renewedDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of when the group was last renewed\",\n      \"readOnly\": true\n    },\n    \"expirationDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of when the group is set to expire\",\n      \"readOnly\": true\n    },\n    \"membershipRule\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The rule that determines members for this group if the group is a dynamic group\"\n    },\n    \"membershipRuleProcessingState\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [null, \"On\", \"Paused\"],\n      \"description\": \"Indicates whether dynamic\
  \ membership processing is on or paused\"\n    },\n    \"isAssignableToRole\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Indicates whether this group can be assigned to a Microsoft Entra role\"\n    },\n    \"isArchived\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"When a group is associated with a team, this determines whether the team is in read-only mode\"\n    },\n    \"isManagementRestricted\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Indicates whether the group is a member of a restricted management administrative unit\",\n      \"readOnly\": true\n    },\n    \"preferredDataLocation\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The preferred data location for the Microsoft 365 group\"\n    },\n    \"preferredLanguage\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The preferred language for a Microsoft 365 group in ISO 639-1 format\"\n    },\n   \
  \ \"proxyAddresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Email addresses for the group that direct to the same group mailbox\",\n      \"readOnly\": true\n    },\n    \"securityIdentifier\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Security identifier of the group, used in Windows scenarios\",\n      \"readOnly\": true\n    },\n    \"uniqueName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The unique identifier that can be assigned to a group and used as an alternate key\",\n      \"readOnly\": true\n    },\n    \"onPremisesDomainName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Contains the on-premises domain FQDN\",\n      \"readOnly\": true\n    },\n    \"onPremisesLastSyncDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Indicates the last time at which the group\
  \ was synced with the on-premises directory\",\n      \"readOnly\": true\n    },\n    \"onPremisesNetBiosName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Contains the on-premises netBios name\",\n      \"readOnly\": true\n    },\n    \"onPremisesSamAccountName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Contains the on-premises SAM account name\",\n      \"readOnly\": true\n    },\n    \"onPremisesSecurityIdentifier\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Contains the on-premises security identifier (SID) for the group\",\n      \"readOnly\": true\n    },\n    \"onPremisesSyncEnabled\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"True if this group is synced from an on-premises directory\",\n      \"readOnly\": true\n    },\n    \"onPremisesProvisioningErrors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/OnPremisesProvisioningError\"\n  \
  \    },\n      \"description\": \"Errors when using Microsoft synchronization product during provisioning\"\n    },\n    \"allowExternalSenders\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Indicates if people external to the organization can send messages to the group\"\n    },\n    \"autoSubscribeNewMembers\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Indicates if new members added to the group are auto-subscribed to receive email notifications\"\n    },\n    \"hideFromAddressLists\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"True if the group is not displayed in certain parts of the Outlook UI\"\n    },\n    \"hideFromOutlookClients\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"True if the group is not displayed in Outlook clients\"\n    },\n    \"isSubscribedByMail\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Indicates whether the signed-in user\
  \ is subscribed to receive email conversations\"\n    },\n    \"hasMembersWithLicenseErrors\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Indicates whether there are members in this group that have license errors\",\n      \"readOnly\": true\n    },\n    \"unseenCount\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Count of conversations that received new posts since the signed-in user last visited the group\"\n    },\n    \"resourceBehaviorOptions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Specifies the group behaviors that can be set during creation\"\n    },\n    \"resourceProvisioningOptions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Specifies the group resources associated with the Microsoft 365 group\"\n    },\n    \"assignedLicenses\": {\n      \"type\": \"array\",\n      \"items\"\
  : {\n        \"$ref\": \"#/$defs/AssignedLicense\"\n      },\n      \"description\": \"The licenses that are assigned to the group\",\n      \"readOnly\": true\n    },\n    \"assignedLabels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AssignedLabel\"\n      },\n      \"description\": \"The list of sensitivity label pairs associated with a Microsoft 365 group\"\n    }\n  },\n  \"$defs\": {\n    \"OnPremisesProvisioningError\": {\n      \"type\": \"object\",\n      \"description\": \"Represents errors during synchronization from on-premises directory\",\n      \"properties\": {\n        \"category\": {\n          \"type\": \"string\",\n          \"description\": \"Category of the provisioning error\"\n        },\n        \"occurredDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time at which the error occurred\"\n        },\n        \"propertyCausingError\": {\n          \"\
  type\": \"string\",\n          \"description\": \"Name of the directory property causing the error\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"Value of the property causing the error\"\n        }\n      }\n    },\n    \"AssignedLicense\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a license assigned to a group\",\n      \"properties\": {\n        \"skuId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the SKU\"\n        },\n        \"disabledPlans\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"A collection of the unique identifiers for disabled plans\"\n        }\n      }\n    },\n    \"AssignedLabel\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a sensitivity label assigned to a Microsoft 365 group\",\n      \"properties\": {\n        \"labelId\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the label\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the label\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/json-schema/microsoft-graph-group-schema.json
tags: []
title: Microsoft Graph Group
---
