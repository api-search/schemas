---
description: Base class for Compliance policy in Microsoft Intune. Compliance policies are platform-specific and individual per-platform compliance policies inherit from this base type. Represents the deviceCompliancePolicy resource from the Microsoft Graph API.
layout: schema
name: Device Compliance Policy
properties_list:
- description: Key of the entity.
  name: id
  type: string
- description: DateTime the object was created.
  name: createdDateTime
  type: string
- description: Admin provided description of the device configuration.
  name: description
  type:
  - string
  - 'null'
- description: DateTime the object was last modified.
  name: lastModifiedDateTime
  type: string
- description: Admin provided name of the device configuration.
  name: displayName
  type: string
- description: Version of the device configuration.
  name: version
  type: integer
- description: The list of scheduled action per rule for this compliance policy. Required when creating per-platform compliance policies.
  name: scheduledActionsForRule
  type: array
- description: List of per-device compliance statuses.
  name: deviceStatuses
  type: array
- description: List of per-user compliance statuses.
  name: userStatuses
  type: array
- description: Device compliance devices status overview.
  name: deviceStatusOverview
  type: object
- description: Device compliance users status overview.
  name: userStatusOverview
  type: object
- description: Compliance setting state device summary.
  name: deviceSettingStateSummaries
  type: array
- description: The collection of assignments for this compliance policy.
  name: assignments
  type: array
provider_name: Microsoft Endpoint Configuration Management
provider_slug: microsoft-endpoint-configuration-management
schema_file: json-schema/microsoft-endpoint-configuration-management-compliance-policy-schema.json
slug: microsoft-endpoint-configuration-management-compliance-policy
source_filename: microsoft-endpoint-configuration-management-compliance-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/kinlane/microsoft-endpoint-configuration-management/json-schema/microsoft-endpoint-configuration-management-compliance-policy-schema.json\",\n  \"title\": \"Device Compliance Policy\",\n  \"description\": \"Base class for Compliance policy in Microsoft Intune. Compliance policies are platform-specific and individual per-platform compliance policies inherit from this base type. Represents the deviceCompliancePolicy resource from the Microsoft Graph API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Key of the entity.\"\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"DateTime the object was created.\",\n      \"readOnly\": true\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Admin\
  \ provided description of the device configuration.\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"DateTime the object was last modified.\",\n      \"readOnly\": true\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Admin provided name of the device configuration.\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"Version of the device configuration.\",\n      \"readOnly\": true\n    },\n    \"scheduledActionsForRule\": {\n      \"type\": \"array\",\n      \"description\": \"The list of scheduled action per rule for this compliance policy. Required when creating per-platform compliance policies.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DeviceComplianceScheduledActionForRule\"\n      }\n    },\n    \"deviceStatuses\": {\n      \"type\": \"array\",\n      \"description\": \"List of per-device compliance statuses.\",\n   \
  \   \"readOnly\": true,\n      \"items\": {\n        \"$ref\": \"#/$defs/DeviceComplianceDeviceStatus\"\n      }\n    },\n    \"userStatuses\": {\n      \"type\": \"array\",\n      \"description\": \"List of per-user compliance statuses.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"$ref\": \"#/$defs/DeviceComplianceUserStatus\"\n      }\n    },\n    \"deviceStatusOverview\": {\n      \"$ref\": \"#/$defs/DeviceComplianceDeviceOverview\",\n      \"description\": \"Device compliance devices status overview.\",\n      \"readOnly\": true\n    },\n    \"userStatusOverview\": {\n      \"$ref\": \"#/$defs/DeviceComplianceUserOverview\",\n      \"description\": \"Device compliance users status overview.\",\n      \"readOnly\": true\n    },\n    \"deviceSettingStateSummaries\": {\n      \"type\": \"array\",\n      \"description\": \"Compliance setting state device summary.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"$ref\": \"#/$defs/SettingStateDeviceSummary\"\n\
  \      }\n    },\n    \"assignments\": {\n      \"type\": \"array\",\n      \"description\": \"The collection of assignments for this compliance policy.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DeviceCompliancePolicyAssignment\"\n      }\n    }\n  },\n  \"required\": [\"displayName\"],\n  \"$defs\": {\n    \"DeviceComplianceScheduledActionForRule\": {\n      \"type\": \"object\",\n      \"description\": \"Scheduled action for a compliance policy rule.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Key of the entity.\"\n        },\n        \"ruleName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Name of the rule this scheduled action applies to.\"\n        },\n        \"scheduledActionConfigurations\": {\n          \"type\": \"array\",\n          \"description\": \"The list of scheduled action configurations for this compliance policy.\",\n          \"items\": {\n            \"type\"\
  : \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\"\n              },\n              \"gracePeriodHours\": {\n                \"type\": \"integer\",\n                \"description\": \"Number of hours to wait before enforcing the action.\"\n              },\n              \"actionType\": {\n                \"type\": \"string\",\n                \"description\": \"Type of action to take.\",\n                \"enum\": [\"noAction\", \"notification\", \"block\", \"retire\", \"wipe\", \"removeResourceAccessProfiles\", \"pushNotification\"]\n              },\n              \"notificationTemplateId\": {\n                \"type\": \"string\",\n                \"description\": \"Notification template ID to use.\"\n              },\n              \"notificationMessageCCList\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"string\"\n                },\n                \"description\": \"\
  List of group IDs to CC the notification message to.\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"DeviceComplianceDeviceStatus\": {\n      \"type\": \"object\",\n      \"description\": \"Per-device compliance status.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"deviceDisplayName\": {\n          \"type\": \"string\",\n          \"description\": \"Device display name.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Compliance status of the policy report.\",\n          \"enum\": [\"unknown\", \"notApplicable\", \"compliant\", \"remediated\", \"nonCompliant\", \"error\", \"conflict\", \"notAssigned\"]\n        },\n        \"lastReportedDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Last modified date time of the policy report.\"\n        },\n        \"userPrincipalName\": {\n   \
  \       \"type\": \"string\",\n          \"description\": \"User principal name.\"\n        }\n      }\n    },\n    \"DeviceComplianceUserStatus\": {\n      \"type\": \"object\",\n      \"description\": \"Per-user compliance status.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"userDisplayName\": {\n          \"type\": \"string\",\n          \"description\": \"User display name.\"\n        },\n        \"devicesCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Devices count for the user.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Compliance status of the policy report.\",\n          \"enum\": [\"unknown\", \"notApplicable\", \"compliant\", \"remediated\", \"nonCompliant\", \"error\", \"conflict\", \"notAssigned\"]\n        },\n        \"lastReportedDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n      \
  \  \"userPrincipalName\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"DeviceComplianceDeviceOverview\": {\n      \"type\": \"object\",\n      \"description\": \"Overview of device compliance status counts.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"pendingCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of pending devices.\"\n        },\n        \"notApplicableCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of not applicable devices.\"\n        },\n        \"successCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of succeeded devices.\"\n        },\n        \"errorCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of error devices.\"\n        },\n        \"failedCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of failed devices.\"\n        },\n\
  \        \"lastUpdateDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Last update time.\"\n        },\n        \"configurationVersion\": {\n          \"type\": \"integer\",\n          \"description\": \"Version of the policy for that overview.\"\n        }\n      }\n    },\n    \"DeviceComplianceUserOverview\": {\n      \"type\": \"object\",\n      \"description\": \"Overview of user compliance status counts.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"pendingCount\": {\n          \"type\": \"integer\"\n        },\n        \"notApplicableCount\": {\n          \"type\": \"integer\"\n        },\n        \"successCount\": {\n          \"type\": \"integer\"\n        },\n        \"errorCount\": {\n          \"type\": \"integer\"\n        },\n        \"failedCount\": {\n          \"type\": \"integer\"\n        },\n        \"lastUpdateDateTime\": {\n          \"type\": \"\
  string\",\n          \"format\": \"date-time\"\n        },\n        \"configurationVersion\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"SettingStateDeviceSummary\": {\n      \"type\": \"object\",\n      \"description\": \"Device compliance setting state summary.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"settingName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the setting.\"\n        },\n        \"instancePath\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the InstancePath for the setting.\"\n        },\n        \"compliantDeviceCount\": {\n          \"type\": \"integer\"\n        },\n        \"errorDeviceCount\": {\n          \"type\": \"integer\"\n        },\n        \"conflictDeviceCount\": {\n          \"type\": \"integer\"\n        },\n        \"nonCompliantDeviceCount\": {\n          \"type\": \"integer\"\n        },\n        \"notApplicableDeviceCount\"\
  : {\n          \"type\": \"integer\"\n        },\n        \"remediatedDeviceCount\": {\n          \"type\": \"integer\"\n        },\n        \"unknownDeviceCount\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"DeviceCompliancePolicyAssignment\": {\n      \"type\": \"object\",\n      \"description\": \"Assignment of a device compliance policy to a group.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"target\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"@odata.type\": {\n              \"type\": \"string\",\n              \"description\": \"Type of target (e.g., #microsoft.graph.groupAssignmentTarget).\"\n            },\n            \"groupId\": {\n              \"type\": \"string\",\n              \"description\": \"The group ID for the assignment target.\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-endpoint-configuration-management/refs/heads/main/json-schema/microsoft-endpoint-configuration-management-compliance-policy-schema.json
tags:
- Compliance
- Configuration Management
- Device Management
- Endpoint Management
- Mobile Device Management
- Patch Management
- Software Deployment
title: Device Compliance Policy
---
