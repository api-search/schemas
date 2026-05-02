---
description: Device configuration profile in Microsoft Intune. Represents the deviceConfiguration resource type from the Microsoft Graph API. Platform-specific configuration profiles inherit from this base type to define specific settings for Windows, iOS, Android, and macOS devices.
layout: schema
name: Device Configuration Profile
properties_list:
- description: Key of the entity.
  name: id
  type: string
- description: DateTime the object was last modified.
  name: lastModifiedDateTime
  type: string
- description: DateTime the object was created.
  name: createdDateTime
  type: string
- description: Admin provided description of the device configuration.
  name: description
  type:
  - string
  - 'null'
- description: Admin provided name of the device configuration.
  name: displayName
  type: string
- description: Version of the device configuration.
  name: version
  type: integer
- description: The list of assignments for the device configuration profile.
  name: assignments
  type: array
- description: Device configuration installation status by device.
  name: deviceStatuses
  type: array
- description: Device configuration installation status by user.
  name: userStatuses
  type: array
- description: Device configuration devices status overview.
  name: deviceStatusOverview
  type: object
- description: Device configuration users status overview.
  name: userStatusOverview
  type: object
- description: Device configuration setting state device summary.
  name: deviceSettingStateSummaries
  type: array
provider_name: Microsoft Endpoint Configuration Management
provider_slug: microsoft-endpoint-configuration-management
schema_file: json-schema/microsoft-endpoint-configuration-management-configuration-profile-schema.json
slug: microsoft-endpoint-configuration-management-configuration-profile
source_filename: microsoft-endpoint-configuration-management-configuration-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/kinlane/microsoft-endpoint-configuration-management/json-schema/microsoft-endpoint-configuration-management-configuration-profile-schema.json\",\n  \"title\": \"Device Configuration Profile\",\n  \"description\": \"Device configuration profile in Microsoft Intune. Represents the deviceConfiguration resource type from the Microsoft Graph API. Platform-specific configuration profiles inherit from this base type to define specific settings for Windows, iOS, Android, and macOS devices.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Key of the entity.\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"DateTime the object was last modified.\",\n      \"readOnly\": true\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"DateTime the object was created.\",\n      \"readOnly\": true\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Admin provided description of the device configuration.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Admin provided name of the device configuration.\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"Version of the device configuration.\",\n      \"readOnly\": true\n    },\n    \"assignments\": {\n      \"type\": \"array\",\n      \"description\": \"The list of assignments for the device configuration profile.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DeviceConfigurationAssignment\"\n      }\n    },\n    \"deviceStatuses\": {\n      \"type\": \"array\",\n      \"description\": \"Device configuration installation status by device.\",\n      \"readOnly\": true,\n      \"items\": {\n\
  \        \"$ref\": \"#/$defs/DeviceConfigurationDeviceStatus\"\n      }\n    },\n    \"userStatuses\": {\n      \"type\": \"array\",\n      \"description\": \"Device configuration installation status by user.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"$ref\": \"#/$defs/DeviceConfigurationUserStatus\"\n      }\n    },\n    \"deviceStatusOverview\": {\n      \"$ref\": \"#/$defs/DeviceConfigurationDeviceOverview\",\n      \"description\": \"Device configuration devices status overview.\",\n      \"readOnly\": true\n    },\n    \"userStatusOverview\": {\n      \"$ref\": \"#/$defs/DeviceConfigurationUserOverview\",\n      \"description\": \"Device configuration users status overview.\",\n      \"readOnly\": true\n    },\n    \"deviceSettingStateSummaries\": {\n      \"type\": \"array\",\n      \"description\": \"Device configuration setting state device summary.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"$ref\": \"#/$defs/SettingStateDeviceSummary\"\n   \
  \   }\n    }\n  },\n  \"required\": [\"displayName\"],\n  \"$defs\": {\n    \"DeviceConfigurationAssignment\": {\n      \"type\": \"object\",\n      \"description\": \"Assignment of a device configuration profile to a group.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Key of the assignment.\"\n        },\n        \"target\": {\n          \"type\": \"object\",\n          \"description\": \"The assignment target for the device configuration.\",\n          \"properties\": {\n            \"@odata.type\": {\n              \"type\": \"string\",\n              \"description\": \"Type discriminator for the target (e.g., #microsoft.graph.groupAssignmentTarget).\"\n            },\n            \"groupId\": {\n              \"type\": \"string\",\n              \"description\": \"The group ID for the assignment target.\"\n            }\n          }\n        }\n      }\n    },\n    \"DeviceConfigurationDeviceStatus\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"Per-device configuration installation status.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"deviceDisplayName\": {\n          \"type\": \"string\",\n          \"description\": \"Device display name.\"\n        },\n        \"userName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"User name associated with the report.\"\n        },\n        \"deviceModel\": {\n          \"type\": \"string\",\n          \"description\": \"The device model.\"\n        },\n        \"complianceGracePeriodExpirationDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The DateTime when device compliance grace period expires.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Compliance status of the policy report.\",\n          \"enum\": [\"unknown\", \"notApplicable\", \"compliant\"\
  , \"remediated\", \"nonCompliant\", \"error\", \"conflict\", \"notAssigned\"]\n        },\n        \"lastReportedDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Last modified date time of the policy report.\"\n        },\n        \"userPrincipalName\": {\n          \"type\": \"string\",\n          \"description\": \"User principal name.\"\n        }\n      }\n    },\n    \"DeviceConfigurationUserStatus\": {\n      \"type\": \"object\",\n      \"description\": \"Per-user configuration installation status.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"userDisplayName\": {\n          \"type\": \"string\",\n          \"description\": \"User display name.\"\n        },\n        \"devicesCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Devices count for the user.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"\
  description\": \"Compliance status of the policy report.\",\n          \"enum\": [\"unknown\", \"notApplicable\", \"compliant\", \"remediated\", \"nonCompliant\", \"error\", \"conflict\", \"notAssigned\"]\n        },\n        \"lastReportedDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"userPrincipalName\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"DeviceConfigurationDeviceOverview\": {\n      \"type\": \"object\",\n      \"description\": \"Overview of device configuration status counts.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"pendingCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of pending devices.\"\n        },\n        \"notApplicableCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of not applicable devices.\"\n        },\n        \"successCount\": {\n          \"type\"\
  : \"integer\",\n          \"description\": \"Number of succeeded devices.\"\n        },\n        \"errorCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of error devices.\"\n        },\n        \"failedCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of failed devices.\"\n        },\n        \"lastUpdateDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Last update time.\"\n        },\n        \"configurationVersion\": {\n          \"type\": \"integer\",\n          \"description\": \"Version of the policy for the overview.\"\n        }\n      }\n    },\n    \"DeviceConfigurationUserOverview\": {\n      \"type\": \"object\",\n      \"description\": \"Overview of user configuration status counts.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"pendingCount\": {\n          \"type\": \"integer\"\n        },\n\
  \        \"notApplicableCount\": {\n          \"type\": \"integer\"\n        },\n        \"successCount\": {\n          \"type\": \"integer\"\n        },\n        \"errorCount\": {\n          \"type\": \"integer\"\n        },\n        \"failedCount\": {\n          \"type\": \"integer\"\n        },\n        \"lastUpdateDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"configurationVersion\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"SettingStateDeviceSummary\": {\n      \"type\": \"object\",\n      \"description\": \"Device configuration setting state summary.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"settingName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the setting.\"\n        },\n        \"instancePath\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the InstancePath for the setting.\"\
  \n        },\n        \"compliantDeviceCount\": {\n          \"type\": \"integer\"\n        },\n        \"errorDeviceCount\": {\n          \"type\": \"integer\"\n        },\n        \"conflictDeviceCount\": {\n          \"type\": \"integer\"\n        },\n        \"nonCompliantDeviceCount\": {\n          \"type\": \"integer\"\n        },\n        \"notApplicableDeviceCount\": {\n          \"type\": \"integer\"\n        },\n        \"remediatedDeviceCount\": {\n          \"type\": \"integer\"\n        },\n        \"unknownDeviceCount\": {\n          \"type\": \"integer\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-endpoint-configuration-management/refs/heads/main/json-schema/microsoft-endpoint-configuration-management-configuration-profile-schema.json
tags:
- Compliance
- Configuration Management
- Device Management
- Endpoint Management
- Mobile Device Management
- Patch Management
- Software Deployment
title: Device Configuration Profile
---
