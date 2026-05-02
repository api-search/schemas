---
description: A device managed or pre-enrolled through Microsoft Intune, representing the managedDevice resource type from the Microsoft Graph API for Intune device management.
layout: schema
name: Managed Device
properties_list:
- description: Unique identifier for the device. This property is read-only.
  name: id
  type: string
- description: Unique identifier for the user associated with the device.
  name: userId
  type: string
- description: Name of the device.
  name: deviceName
  type: string
- description: Ownership of the device. Can be company or personal.
  name: managedDeviceOwnerType
  type: string
- description: Enrollment time of the device.
  name: enrolledDateTime
  type: string
- description: The date and time that the device last completed a successful sync with Intune.
  name: lastSyncDateTime
  type: string
- description: Operating system of the device (Windows, iOS, Android, macOS, etc.).
  name: operatingSystem
  type: string
- description: Compliance state of the device.
  name: complianceState
  type: string
- description: Whether the device is jail broken or rooted.
  name: jailBroken
  type: string
- description: Management channel of the device.
  name: managementAgent
  type: string
- description: Operating system version of the device.
  name: osVersion
  type: string
- description: Whether the device is Exchange ActiveSync activated.
  name: easActivated
  type: boolean
- description: Exchange ActiveSync Id of the device.
  name: easDeviceId
  type: string
- description: Exchange ActivationSync activation time of the device.
  name: easActivationDateTime
  type: string
- description: Whether the device is Azure Active Directory registered.
  name: azureADRegistered
  type:
  - boolean
  - 'null'
- description: Enrollment type of the device.
  name: deviceEnrollmentType
  type: string
- description: The code that allows the Activation Lock on managed device to be bypassed.
  name: activationLockBypassCode
  type:
  - string
  - 'null'
- description: Email(s) for the user associated with the device.
  name: emailAddress
  type: string
- description: The unique identifier for the Azure Active Directory device.
  name: azureADDeviceId
  type: string
- description: Device registration state.
  name: deviceRegistrationState
  type: string
- description: Device category display name.
  name: deviceCategoryDisplayName
  type: string
- description: Device supervised status.
  name: isSupervised
  type: boolean
- description: Last time the device contacted Exchange.
  name: exchangeLastSuccessfulSyncDateTime
  type: string
- description: The Access State of the device in Exchange.
  name: exchangeAccessState
  type: string
- description: The reason for the device's access state in Exchange.
  name: exchangeAccessStateReason
  type: string
- description: Device encryption status.
  name: isEncrypted
  type: boolean
- description: Device user principal name.
  name: userPrincipalName
  type: string
- description: Model of the device.
  name: model
  type: string
- description: Manufacturer of the device.
  name: manufacturer
  type: string
- description: IMEI.
  name: imei
  type: string
- description: The DateTime when device compliance grace period expires.
  name: complianceGracePeriodExpirationDateTime
  type: string
- description: Serial number of the device.
  name: serialNumber
  type: string
- description: Phone number of the device.
  name: phoneNumber
  type: string
- description: Android security patch level.
  name: androidSecurityPatchLevel
  type: string
- description: User display name.
  name: userDisplayName
  type: string
- description: Configuration Manager client enabled features.
  name: configurationManagerClientEnabledFeatures
  type: object
- description: Wi-Fi MAC address.
  name: wiFiMacAddress
  type: string
- description: Subscriber carrier.
  name: subscriberCarrier
  type: string
- description: MEID.
  name: meid
  type: string
- description: Total storage in bytes.
  name: totalStorageSpaceInBytes
  type: integer
- description: Free storage in bytes.
  name: freeStorageSpaceInBytes
  type: integer
- description: Automatically generated name to identify a device. Can be overwritten to a user-friendly name.
  name: managedDeviceName
  type: string
- description: Threat state of a device when a Mobile Threat Defense partner is in use.
  name: partnerReportedThreatState
  type: string
- description: Reports if the managed iOS device is user approval enrollment.
  name: requireUserEnrollmentApproval
  type:
  - boolean
  - 'null'
- description: Reports device management certificate expiration date.
  name: managementCertificateExpirationDate
  type: string
- description: Integrated Circuit Card Identifier (SIM card unique identification number).
  name: iccid
  type:
  - string
  - 'null'
- description: Unique Device Identifier for iOS and macOS devices.
  name: udid
  type:
  - string
  - 'null'
- description: Notes on the device created by IT Admin.
  name: notes
  type:
  - string
  - 'null'
- description: Ethernet MAC Address of the device.
  name: ethernetMacAddress
  type:
  - string
  - 'null'
- description: Total memory in bytes.
  name: physicalMemoryInBytes
  type: integer
- description: Name of the enrollment profile assigned to the device.
  name: enrollmentProfileName
  type: string
provider_name: Microsoft Endpoint Configuration Management
provider_slug: microsoft-endpoint-configuration-management
schema_file: json-schema/microsoft-endpoint-configuration-management-device-schema.json
slug: microsoft-endpoint-configuration-management-device
source_filename: microsoft-endpoint-configuration-management-device-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/kinlane/microsoft-endpoint-configuration-management/json-schema/microsoft-endpoint-configuration-management-device-schema.json\",\n  \"title\": \"Managed Device\",\n  \"description\": \"A device managed or pre-enrolled through Microsoft Intune, representing the managedDevice resource type from the Microsoft Graph API for Intune device management.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the device. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the user associated with the device.\",\n      \"readOnly\": true\n    },\n    \"deviceName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the device.\",\n      \"readOnly\": true\n    },\n    \"managedDeviceOwnerType\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Ownership of the device. Can be company or personal.\",\n      \"enum\": [\"unknown\", \"company\", \"personal\"]\n    },\n    \"enrolledDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Enrollment time of the device.\",\n      \"readOnly\": true\n    },\n    \"lastSyncDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time that the device last completed a successful sync with Intune.\",\n      \"readOnly\": true\n    },\n    \"operatingSystem\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system of the device (Windows, iOS, Android, macOS, etc.).\",\n      \"readOnly\": true\n    },\n    \"complianceState\": {\n      \"type\": \"string\",\n      \"description\": \"Compliance state of the device.\",\n      \"enum\": [\"unknown\", \"compliant\", \"noncompliant\", \"conflict\", \"error\", \"\
  inGracePeriod\", \"configManager\"]\n    },\n    \"jailBroken\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the device is jail broken or rooted.\",\n      \"readOnly\": true\n    },\n    \"managementAgent\": {\n      \"type\": \"string\",\n      \"description\": \"Management channel of the device.\",\n      \"enum\": [\n        \"eas\", \"mdm\", \"easMdm\", \"intuneClient\", \"easIntuneClient\",\n        \"configurationManagerClient\", \"configurationManagerClientMdm\",\n        \"configurationManagerClientMdmEas\", \"unknown\", \"jamf\",\n        \"googleCloudDevicePolicyController\"\n      ]\n    },\n    \"osVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system version of the device.\",\n      \"readOnly\": true\n    },\n    \"easActivated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the device is Exchange ActiveSync activated.\",\n      \"readOnly\": true\n    },\n    \"easDeviceId\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Exchange ActiveSync Id of the device.\",\n      \"readOnly\": true\n    },\n    \"easActivationDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Exchange ActivationSync activation time of the device.\",\n      \"readOnly\": true\n    },\n    \"azureADRegistered\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Whether the device is Azure Active Directory registered.\",\n      \"readOnly\": true\n    },\n    \"deviceEnrollmentType\": {\n      \"type\": \"string\",\n      \"description\": \"Enrollment type of the device.\",\n      \"enum\": [\n        \"unknown\", \"userEnrollment\", \"deviceEnrollmentManager\",\n        \"appleBulkWithUser\", \"appleBulkWithoutUser\", \"windowsAzureADJoin\",\n        \"windowsBulkUserless\", \"windowsAutoEnrollment\",\n        \"windowsBulkAzureDomainJoin\", \"windowsCoManagement\",\n        \"windowsAzureADJoinUsingDeviceAuth\", \"appleUserEnrollment\"\
  ,\n        \"appleUserEnrollmentWithServiceAccount\"\n      ],\n      \"readOnly\": true\n    },\n    \"activationLockBypassCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The code that allows the Activation Lock on managed device to be bypassed.\",\n      \"readOnly\": true\n    },\n    \"emailAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Email(s) for the user associated with the device.\",\n      \"readOnly\": true\n    },\n    \"azureADDeviceId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the Azure Active Directory device.\",\n      \"readOnly\": true\n    },\n    \"deviceRegistrationState\": {\n      \"type\": \"string\",\n      \"description\": \"Device registration state.\",\n      \"enum\": [\n        \"notRegistered\", \"registered\", \"revoked\", \"keyConflict\",\n        \"approvalPending\", \"certificateReset\",\n        \"notRegisteredPendingEnrollment\", \"unknown\"\n      ],\n    \
  \  \"readOnly\": true\n    },\n    \"deviceCategoryDisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"Device category display name.\",\n      \"readOnly\": true\n    },\n    \"isSupervised\": {\n      \"type\": \"boolean\",\n      \"description\": \"Device supervised status.\",\n      \"readOnly\": true\n    },\n    \"exchangeLastSuccessfulSyncDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last time the device contacted Exchange.\",\n      \"readOnly\": true\n    },\n    \"exchangeAccessState\": {\n      \"type\": \"string\",\n      \"description\": \"The Access State of the device in Exchange.\",\n      \"enum\": [\"none\", \"unknown\", \"allowed\", \"blocked\", \"quarantined\"],\n      \"readOnly\": true\n    },\n    \"exchangeAccessStateReason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason for the device's access state in Exchange.\",\n      \"enum\": [\n        \"none\", \"unknown\"\
  , \"exchangeGlobalRule\", \"exchangeIndividualRule\",\n        \"exchangeDeviceRule\", \"exchangeUpgrade\", \"exchangeMailboxPolicy\",\n        \"other\", \"compliant\", \"notCompliant\", \"notEnrolled\",\n        \"unknownLocation\", \"mfaRequired\", \"azureADBlockDueToAccessPolicy\",\n        \"compromisedPassword\", \"deviceNotKnownWithManagedApp\"\n      ],\n      \"readOnly\": true\n    },\n    \"isEncrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Device encryption status.\",\n      \"readOnly\": true\n    },\n    \"userPrincipalName\": {\n      \"type\": \"string\",\n      \"description\": \"Device user principal name.\",\n      \"readOnly\": true\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Model of the device.\",\n      \"readOnly\": true\n    },\n    \"manufacturer\": {\n      \"type\": \"string\",\n      \"description\": \"Manufacturer of the device.\",\n      \"readOnly\": true\n    },\n    \"imei\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"IMEI.\",\n      \"readOnly\": true\n    },\n    \"complianceGracePeriodExpirationDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The DateTime when device compliance grace period expires.\",\n      \"readOnly\": true\n    },\n    \"serialNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Serial number of the device.\",\n      \"readOnly\": true\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number of the device.\",\n      \"readOnly\": true\n    },\n    \"androidSecurityPatchLevel\": {\n      \"type\": \"string\",\n      \"description\": \"Android security patch level.\",\n      \"readOnly\": true\n    },\n    \"userDisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"User display name.\",\n      \"readOnly\": true\n    },\n    \"configurationManagerClientEnabledFeatures\": {\n      \"type\": \"object\",\n      \"\
  description\": \"Configuration Manager client enabled features.\",\n      \"properties\": {\n        \"inventory\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether inventory is managed by ConfigMgr.\"\n        },\n        \"modernApps\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether modern apps are managed by ConfigMgr.\"\n        },\n        \"resourceAccess\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether resource access is managed by ConfigMgr.\"\n        },\n        \"deviceConfiguration\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether device configuration is managed by ConfigMgr.\"\n        },\n        \"compliancePolicy\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether compliance policy is managed by ConfigMgr.\"\n        },\n        \"windowsUpdateForBusiness\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether Windows Update\
  \ for Business is managed by ConfigMgr.\"\n        }\n      },\n      \"readOnly\": true\n    },\n    \"wiFiMacAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Wi-Fi MAC address.\",\n      \"readOnly\": true\n    },\n    \"subscriberCarrier\": {\n      \"type\": \"string\",\n      \"description\": \"Subscriber carrier.\",\n      \"readOnly\": true\n    },\n    \"meid\": {\n      \"type\": \"string\",\n      \"description\": \"MEID.\",\n      \"readOnly\": true\n    },\n    \"totalStorageSpaceInBytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Total storage in bytes.\",\n      \"readOnly\": true\n    },\n    \"freeStorageSpaceInBytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Free storage in bytes.\",\n      \"readOnly\": true\n    },\n    \"managedDeviceName\": {\n      \"type\": \"string\",\n      \"description\": \"Automatically generated name to identify a device. Can be overwritten to a user-friendly name.\"\n    },\n    \"partnerReportedThreatState\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Threat state of a device when a Mobile Threat Defense partner is in use.\",\n      \"enum\": [\n        \"unknown\", \"activated\", \"deactivated\", \"secured\", \"lowSeverity\",\n        \"mediumSeverity\", \"highSeverity\", \"unresponsive\", \"compromised\",\n        \"misconfigured\"\n      ],\n      \"readOnly\": true\n    },\n    \"requireUserEnrollmentApproval\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Reports if the managed iOS device is user approval enrollment.\",\n      \"readOnly\": true\n    },\n    \"managementCertificateExpirationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Reports device management certificate expiration date.\",\n      \"readOnly\": true\n    },\n    \"iccid\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Integrated Circuit Card Identifier (SIM card unique identification number).\",\n    \
  \  \"readOnly\": true\n    },\n    \"udid\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Unique Device Identifier for iOS and macOS devices.\",\n      \"readOnly\": true\n    },\n    \"notes\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Notes on the device created by IT Admin.\"\n    },\n    \"ethernetMacAddress\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Ethernet MAC Address of the device.\",\n      \"readOnly\": true\n    },\n    \"physicalMemoryInBytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Total memory in bytes.\",\n      \"readOnly\": true\n    },\n    \"enrollmentProfileName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the enrollment profile assigned to the device.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-endpoint-configuration-management/refs/heads/main/json-schema/microsoft-endpoint-configuration-management-device-schema.json
tags:
- Compliance
- Configuration Management
- Device Management
- Endpoint Management
- Mobile Device Management
- Patch Management
- Software Deployment
title: Managed Device
---
