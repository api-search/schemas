---
description: Represents a device that is managed through Intune. Contains information about the hardware inventory, installed applications, and compliance state of the device.
layout: schema
name: Microsoft Intune Managed Device
properties_list:
- description: Unique identifier for the device
  name: id
  type: string
- description: Name of the device
  name: deviceName
  type:
  - string
  - 'null'
- description: Ownership of the device (company or personal)
  name: managedDeviceOwnerType
  type: string
- description: Enrollment time of the device
  name: enrolledDateTime
  type: string
- description: The date and time that the device last completed a sync with Intune
  name: lastSyncDateTime
  type: string
- description: Operating system of the device (Windows, iOS, Android, macOS)
  name: operatingSystem
  type:
  - string
  - 'null'
- description: Operating system version of the device
  name: osVersion
  type:
  - string
  - 'null'
- description: Compliance state of the device
  name: complianceState
  type: string
- description: Model of the device
  name: model
  type:
  - string
  - 'null'
- description: Manufacturer of the device
  name: manufacturer
  type:
  - string
  - 'null'
- description: Serial number of the device
  name: serialNumber
  type:
  - string
  - 'null'
- description: IMEI number of the device
  name: imei
  type:
  - string
  - 'null'
- description: Device user principal name
  name: userPrincipalName
  type:
  - string
  - 'null'
- description: User display name
  name: userDisplayName
  type:
  - string
  - 'null'
- description: Email address of the user associated with the device
  name: emailAddress
  type:
  - string
  - 'null'
- description: Phone number of the device
  name: phoneNumber
  type:
  - string
  - 'null'
- description: Management channel of the device
  name: managementAgent
  type: string
- description: Device registration state
  name: deviceRegistrationState
  type: string
- description: Device category display name
  name: deviceCategoryDisplayName
  type:
  - string
  - 'null'
- description: Device encryption status
  name: isEncrypted
  type:
  - boolean
  - 'null'
- description: Device supervised status
  name: isSupervised
  type:
  - boolean
  - 'null'
- description: Whether the device is jail broken or rooted
  name: jailBroken
  type:
  - string
  - 'null'
- description: Total storage in bytes
  name: totalStorageSpaceInBytes
  type:
  - integer
  - 'null'
- description: Free storage in bytes
  name: freeStorageSpaceInBytes
  type:
  - integer
  - 'null'
- description: Wi-Fi MAC address of the device
  name: wiFiMacAddress
  type:
  - string
  - 'null'
- description: Whether the device is Azure Active Directory registered
  name: azureADRegistered
  type:
  - boolean
  - 'null'
- description: The unique identifier of the Azure Active Directory device
  name: azureADDeviceId
  type:
  - string
  - 'null'
- description: Enrollment type of the device
  name: deviceEnrollmentType
  type: string
provider_name: Microsoft
provider_slug: microsoft
schema_file: json-schema/microsoft-managed-device-schema.json
slug: microsoft-managed-device
source_filename: microsoft-managed-device-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://learn.microsoft.com/en-us/graph/schemas/microsoft/managed-device.json\",\n  \"title\": \"Microsoft Intune Managed Device\",\n  \"description\": \"Represents a device that is managed through Intune. Contains information about the hardware inventory, installed applications, and compliance state of the device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the device\",\n      \"readOnly\": true\n    },\n    \"deviceName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Name of the device\"\n    },\n    \"managedDeviceOwnerType\": {\n      \"type\": \"string\",\n      \"enum\": [\"unknown\", \"company\", \"personal\"],\n      \"description\": \"Ownership of the device (company or personal)\"\n    },\n    \"enrolledDateTime\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\",\n      \"description\": \"Enrollment time of the device\",\n      \"readOnly\": true\n    },\n    \"lastSyncDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time that the device last completed a sync with Intune\",\n      \"readOnly\": true\n    },\n    \"operatingSystem\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Operating system of the device (Windows, iOS, Android, macOS)\"\n    },\n    \"osVersion\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Operating system version of the device\"\n    },\n    \"complianceState\": {\n      \"type\": \"string\",\n      \"enum\": [\"unknown\", \"compliant\", \"noncompliant\", \"conflict\", \"error\", \"inGracePeriod\", \"configManager\"],\n      \"description\": \"Compliance state of the device\"\n    },\n    \"model\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Model of the device\"\n \
  \   },\n    \"manufacturer\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Manufacturer of the device\"\n    },\n    \"serialNumber\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Serial number of the device\"\n    },\n    \"imei\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"IMEI number of the device\"\n    },\n    \"userPrincipalName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Device user principal name\"\n    },\n    \"userDisplayName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"User display name\"\n    },\n    \"emailAddress\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"email\",\n      \"description\": \"Email address of the user associated with the device\"\n    },\n    \"phoneNumber\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Phone number of the device\"\n    },\n    \"managementAgent\": {\n      \"type\"\
  : \"string\",\n      \"enum\": [\"eas\", \"mdm\", \"easMdm\", \"intuneClient\", \"easIntuneClient\", \"configurationManagerClient\", \"configurationManagerClientMdm\", \"unknown\"],\n      \"description\": \"Management channel of the device\"\n    },\n    \"deviceRegistrationState\": {\n      \"type\": \"string\",\n      \"enum\": [\"notRegistered\", \"registered\", \"revoked\", \"keyConflict\", \"approvalPending\", \"certificateReset\", \"notRegisteredPendingEnrollment\", \"unknown\"],\n      \"description\": \"Device registration state\"\n    },\n    \"deviceCategoryDisplayName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Device category display name\"\n    },\n    \"isEncrypted\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Device encryption status\"\n    },\n    \"isSupervised\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Device supervised status\"\n    },\n    \"jailBroken\": {\n      \"type\": [\"string\"\
  , \"null\"],\n      \"description\": \"Whether the device is jail broken or rooted\"\n    },\n    \"totalStorageSpaceInBytes\": {\n      \"type\": [\"integer\", \"null\"],\n      \"format\": \"int64\",\n      \"description\": \"Total storage in bytes\"\n    },\n    \"freeStorageSpaceInBytes\": {\n      \"type\": [\"integer\", \"null\"],\n      \"format\": \"int64\",\n      \"description\": \"Free storage in bytes\"\n    },\n    \"wiFiMacAddress\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Wi-Fi MAC address of the device\"\n    },\n    \"azureADRegistered\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Whether the device is Azure Active Directory registered\"\n    },\n    \"azureADDeviceId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The unique identifier of the Azure Active Directory device\"\n    },\n    \"deviceEnrollmentType\": {\n      \"type\": \"string\",\n      \"enum\": [\"unknown\", \"userEnrollment\"\
  , \"deviceEnrollmentManager\", \"appleBulkWithUser\", \"appleBulkWithoutUser\", \"windowsAzureADJoin\", \"windowsBulkUserless\", \"windowsAutoEnrollment\", \"windowsBulkAzureDomainJoin\", \"windowsCoManagement\"],\n      \"description\": \"Enrollment type of the device\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/json-schema/microsoft-managed-device-schema.json
tags: []
title: Microsoft Intune Managed Device
---
