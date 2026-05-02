---
description: Devices that are managed or pre-enrolled through Intune. Represents a physical or virtual device managed by the Microsoft Intune service via the Microsoft Graph API. Based on the microsoft.graph.managedDevice resource type.
layout: schema
name: Microsoft Intune Managed Device
properties_list:
- description: The OData type annotation for the managed device resource.
  name: '@odata.type'
  type: string
- description: Unique identifier for the device. This property is read-only.
  name: id
  type: string
- description: Unique identifier for the user associated with the device. This property is read-only.
  name: userId
  type: string
- description: Name of the device. This property is read-only.
  name: deviceName
  type: string
- description: Ownership of the device. Can be 'company' or 'personal'.
  name: managedDeviceOwnerType
  type: string
- description: List of ComplexType deviceActionResult objects. This property is read-only.
  name: deviceActionResults
  type: array
- description: Enrollment time of the device. Supports $filter operator 'lt' and 'gt'. This property is read-only.
  name: enrolledDateTime
  type: string
- description: The date and time that the device last completed a successful sync with Intune. Supports $filter operator 'lt' and 'gt'. This property is read-only.
  name: lastSyncDateTime
  type: string
- description: Operating system of the device. Windows, iOS, etc. This property is read-only.
  name: operatingSystem
  type: string
- description: 'Compliance state of the device. Examples: Compliant, Conflict, Error, etc. Default is unknown. Supports $filter operator ''eq'' and ''or''. This property is read-only.'
  name: complianceState
  type: string
- description: Whether the device is jail broken or rooted. Default is an empty string. This property is read-only.
  name: jailBroken
  type: string
- description: 'Management channel of the device. Examples: Intune, EAS, etc. Default is unknown. This property is read-only.'
  name: managementAgent
  type: string
- description: Operating system version of the device. This property is read-only.
  name: osVersion
  type: string
- description: Whether the device is Exchange ActiveSync activated. This property is read-only.
  name: easActivated
  type: boolean
- description: Exchange ActiveSync Id of the device. This property is read-only.
  name: easDeviceId
  type: string
- description: Exchange ActivationSync activation time of the device. This property is read-only.
  name: easActivationDateTime
  type: string
- description: Whether the device is Azure Active Directory registered. This property is read-only.
  name: azureADRegistered
  type:
  - boolean
  - 'null'
- description: Enrollment type of the device. This property is read-only.
  name: deviceEnrollmentType
  type: string
- description: The code that allows the Activation Lock on managed device to be bypassed. This property is read-only.
  name: activationLockBypassCode
  type:
  - string
  - 'null'
- description: Email(s) for the user associated with the device. This property is read-only.
  name: emailAddress
  type: string
- description: The unique identifier for the Azure Active Directory device. Read only. This property is read-only.
  name: azureADDeviceId
  type: string
- description: Device registration state. This property is read-only.
  name: deviceRegistrationState
  type: string
- description: Device category display name. Default is an empty string. This property is read-only.
  name: deviceCategoryDisplayName
  type: string
- description: Device supervised status. This property is read-only.
  name: isSupervised
  type: boolean
- description: Last time the device contacted Exchange. This property is read-only.
  name: exchangeLastSuccessfulSyncDateTime
  type: string
- description: The Access State of the device in Exchange. This property is read-only.
  name: exchangeAccessState
  type: string
- description: The reason for the device's access state in Exchange. This property is read-only.
  name: exchangeAccessStateReason
  type: string
- description: URL that allows a Remote Assistance session to be established with the device. This property is read-only.
  name: remoteAssistanceSessionUrl
  type:
  - string
  - 'null'
- description: An error string that identifies issues when creating Remote Assistance session objects. This property is read-only.
  name: remoteAssistanceSessionErrorDetails
  type:
  - string
  - 'null'
- description: Device encryption status. This property is read-only.
  name: isEncrypted
  type: boolean
- description: Device user principal name. This property is read-only.
  name: userPrincipalName
  type: string
- description: Model of the device. This property is read-only.
  name: model
  type: string
- description: Manufacturer of the device. This property is read-only.
  name: manufacturer
  type: string
- description: IMEI (International Mobile Equipment Identity). This property is read-only.
  name: imei
  type: string
- description: The DateTime when device compliance grace period expires. This property is read-only.
  name: complianceGracePeriodExpirationDateTime
  type: string
- description: Serial number of the device. This property is read-only.
  name: serialNumber
  type: string
- description: Phone number of the device. This property is read-only.
  name: phoneNumber
  type: string
- description: Android security patch level. This property is read-only.
  name: androidSecurityPatchLevel
  type: string
- description: User display name. This property is read-only.
  name: userDisplayName
  type: string
- description: ConfigrMgr client enabled features. This property is read-only.
  name: configurationManagerClientEnabledFeatures
  type: object
- description: Wi-Fi MAC address. This property is read-only.
  name: wiFiMacAddress
  type: string
- description: The device health attestation state. This property is read-only.
  name: deviceHealthAttestationState
  type: object
- description: Subscriber carrier. This property is read-only.
  name: subscriberCarrier
  type: string
- description: MEID (Mobile Equipment Identifier). This property is read-only.
  name: meid
  type: string
- description: Total storage in bytes. This property is read-only.
  name: totalStorageSpaceInBytes
  type: integer
- description: Free storage in bytes. Default value is 0. This property is read-only.
  name: freeStorageSpaceInBytes
  type: integer
- description: Automatically generated name to identify a device. Can be overwritten to a user friendly name.
  name: managedDeviceName
  type: string
- description: Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device. Read only. This property is read-only.
  name: partnerReportedThreatState
  type: string
- description: Reports if the managed iOS device is user approval enrollment. This property is read-only.
  name: requireUserEnrollmentApproval
  type:
  - boolean
  - 'null'
- description: Reports device management certificate expiration date. This property is read-only.
  name: managementCertificateExpirationDate
  type: string
- description: Integrated Circuit Card Identifier, the SIM card's unique identification number. This property is read-only.
  name: iccid
  type:
  - string
  - 'null'
- description: Unique Device Identifier for iOS and macOS devices. This property is read-only.
  name: udid
  type:
  - string
  - 'null'
- description: Notes on the device created by IT Admin. Default is null.
  name: notes
  type:
  - string
  - 'null'
- description: Indicates Ethernet MAC Address of the device. This property is read-only.
  name: ethernetMacAddress
  type:
  - string
  - 'null'
- description: Total memory in bytes. Default is 0. This property is read-only.
  name: physicalMemoryInBytes
  type: integer
- description: Name of the enrollment profile assigned to the device. Default value is empty string. This property is read-only.
  name: enrollmentProfileName
  type:
  - string
  - 'null'
provider_name: Microsoft Intune
provider_slug: microsoft-intune
schema_file: json-schema/microsoft-intune-managed-device-schema.json
slug: microsoft-intune-managed-device
source_filename: microsoft-intune-managed-device-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/microsoft-intune/json-schema/microsoft-intune-managed-device-schema.json\",\n  \"title\": \"Microsoft Intune Managed Device\",\n  \"description\": \"Devices that are managed or pre-enrolled through Intune. Represents a physical or virtual device managed by the Microsoft Intune service via the Microsoft Graph API. Based on the microsoft.graph.managedDevice resource type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@odata.type\": {\n      \"type\": \"string\",\n      \"const\": \"#microsoft.graph.managedDevice\",\n      \"description\": \"The OData type annotation for the managed device resource.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the device. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique\
  \ identifier for the user associated with the device. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"deviceName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the device. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"managedDeviceOwnerType\": {\n      \"type\": \"string\",\n      \"description\": \"Ownership of the device. Can be 'company' or 'personal'.\",\n      \"enum\": [\n        \"unknown\",\n        \"company\",\n        \"personal\"\n      ]\n    },\n    \"deviceActionResults\": {\n      \"type\": \"array\",\n      \"description\": \"List of ComplexType deviceActionResult objects. This property is read-only.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"$ref\": \"#/$defs/deviceActionResult\"\n      }\n    },\n    \"enrolledDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Enrollment time of the device. Supports $filter operator 'lt' and 'gt'.\
  \ This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"lastSyncDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time that the device last completed a successful sync with Intune. Supports $filter operator 'lt' and 'gt'. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"operatingSystem\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system of the device. Windows, iOS, etc. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"complianceState\": {\n      \"type\": \"string\",\n      \"description\": \"Compliance state of the device. Examples: Compliant, Conflict, Error, etc. Default is unknown. Supports $filter operator 'eq' and 'or'. This property is read-only.\",\n      \"readOnly\": true,\n      \"enum\": [\n        \"unknown\",\n        \"compliant\",\n        \"noncompliant\",\n        \"conflict\",\n        \"error\",\n        \"inGracePeriod\"\
  ,\n        \"configManager\"\n      ]\n    },\n    \"jailBroken\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the device is jail broken or rooted. Default is an empty string. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"managementAgent\": {\n      \"type\": \"string\",\n      \"description\": \"Management channel of the device. Examples: Intune, EAS, etc. Default is unknown. This property is read-only.\",\n      \"readOnly\": true,\n      \"enum\": [\n        \"eas\",\n        \"mdm\",\n        \"easMdm\",\n        \"intuneClient\",\n        \"easIntuneClient\",\n        \"configurationManagerClient\",\n        \"configurationManagerClientMdm\",\n        \"configurationManagerClientMdmEas\",\n        \"unknown\",\n        \"jamf\",\n        \"googleCloudDevicePolicyController\"\n      ]\n    },\n    \"osVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system version of the device. This property is read-only.\"\
  ,\n      \"readOnly\": true\n    },\n    \"easActivated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the device is Exchange ActiveSync activated. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"easDeviceId\": {\n      \"type\": \"string\",\n      \"description\": \"Exchange ActiveSync Id of the device. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"easActivationDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Exchange ActivationSync activation time of the device. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"azureADRegistered\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Whether the device is Azure Active Directory registered. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"deviceEnrollmentType\": {\n      \"type\": \"string\",\n      \"description\": \"Enrollment type of the device. This\
  \ property is read-only.\",\n      \"readOnly\": true,\n      \"enum\": [\n        \"unknown\",\n        \"userEnrollment\",\n        \"deviceEnrollmentManager\",\n        \"appleBulkWithUser\",\n        \"appleBulkWithoutUser\",\n        \"windowsAzureADJoin\",\n        \"windowsBulkUserless\",\n        \"windowsAutoEnrollment\",\n        \"windowsBulkAzureDomainJoin\",\n        \"windowsCoManagement\",\n        \"windowsAzureADJoinUsingDeviceAuth\",\n        \"appleUserEnrollment\",\n        \"appleUserEnrollmentWithServiceAccount\"\n      ]\n    },\n    \"activationLockBypassCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The code that allows the Activation Lock on managed device to be bypassed. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"emailAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Email(s) for the user associated with the device. This property is read-only.\",\n      \"readOnly\": true\n    },\n \
  \   \"azureADDeviceId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the Azure Active Directory device. Read only. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"deviceRegistrationState\": {\n      \"type\": \"string\",\n      \"description\": \"Device registration state. This property is read-only.\",\n      \"readOnly\": true,\n      \"enum\": [\n        \"notRegistered\",\n        \"registered\",\n        \"revoked\",\n        \"keyConflict\",\n        \"approvalPending\",\n        \"certificateReset\",\n        \"notRegisteredPendingEnrollment\",\n        \"unknown\"\n      ]\n    },\n    \"deviceCategoryDisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"Device category display name. Default is an empty string. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"isSupervised\": {\n      \"type\": \"boolean\",\n      \"description\": \"Device supervised status. This property is read-only.\"\
  ,\n      \"readOnly\": true\n    },\n    \"exchangeLastSuccessfulSyncDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last time the device contacted Exchange. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"exchangeAccessState\": {\n      \"type\": \"string\",\n      \"description\": \"The Access State of the device in Exchange. This property is read-only.\",\n      \"readOnly\": true,\n      \"enum\": [\n        \"none\",\n        \"unknown\",\n        \"allowed\",\n        \"blocked\",\n        \"quarantined\"\n      ]\n    },\n    \"exchangeAccessStateReason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason for the device's access state in Exchange. This property is read-only.\",\n      \"readOnly\": true,\n      \"enum\": [\n        \"none\",\n        \"unknown\",\n        \"exchangeGlobalRule\",\n        \"exchangeIndividualRule\",\n        \"exchangeDeviceRule\",\n        \"exchangeUpgrade\"\
  ,\n        \"exchangeMailboxPolicy\",\n        \"other\",\n        \"compliant\",\n        \"notCompliant\",\n        \"notEnrolled\",\n        \"unknownLocation\",\n        \"mfaRequired\",\n        \"azureADBlockDueToAccessPolicy\",\n        \"compromisedPassword\",\n        \"deviceNotKnownWithManagedApp\"\n      ]\n    },\n    \"remoteAssistanceSessionUrl\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"URL that allows a Remote Assistance session to be established with the device. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"remoteAssistanceSessionErrorDetails\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"An error string that identifies issues when creating Remote Assistance session objects. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"isEncrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Device encryption status. This property is read-only.\"\
  ,\n      \"readOnly\": true\n    },\n    \"userPrincipalName\": {\n      \"type\": \"string\",\n      \"description\": \"Device user principal name. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Model of the device. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"manufacturer\": {\n      \"type\": \"string\",\n      \"description\": \"Manufacturer of the device. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"imei\": {\n      \"type\": \"string\",\n      \"description\": \"IMEI (International Mobile Equipment Identity). This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"complianceGracePeriodExpirationDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The DateTime when device compliance grace period expires. This property is read-only.\",\n      \"readOnly\": true\n    },\n   \
  \ \"serialNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Serial number of the device. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number of the device. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"androidSecurityPatchLevel\": {\n      \"type\": \"string\",\n      \"description\": \"Android security patch level. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"userDisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"User display name. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"configurationManagerClientEnabledFeatures\": {\n      \"$ref\": \"#/$defs/configurationManagerClientEnabledFeatures\",\n      \"description\": \"ConfigrMgr client enabled features. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"wiFiMacAddress\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Wi-Fi MAC address. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"deviceHealthAttestationState\": {\n      \"$ref\": \"#/$defs/deviceHealthAttestationState\",\n      \"description\": \"The device health attestation state. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"subscriberCarrier\": {\n      \"type\": \"string\",\n      \"description\": \"Subscriber carrier. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"meid\": {\n      \"type\": \"string\",\n      \"description\": \"MEID (Mobile Equipment Identifier). This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"totalStorageSpaceInBytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Total storage in bytes. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"freeStorageSpaceInBytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Free storage in bytes. Default value is 0.\
  \ This property is read-only.\",\n      \"readOnly\": true,\n      \"default\": 0\n    },\n    \"managedDeviceName\": {\n      \"type\": \"string\",\n      \"description\": \"Automatically generated name to identify a device. Can be overwritten to a user friendly name.\"\n    },\n    \"partnerReportedThreatState\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device. Read only. This property is read-only.\",\n      \"readOnly\": true,\n      \"enum\": [\n        \"unknown\",\n        \"activated\",\n        \"deactivated\",\n        \"secured\",\n        \"lowSeverity\",\n        \"mediumSeverity\",\n        \"highSeverity\",\n        \"unresponsive\",\n        \"compromised\",\n        \"misconfigured\"\n      ]\n    },\n    \"requireUserEnrollmentApproval\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Reports if the managed iOS device is user\
  \ approval enrollment. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"managementCertificateExpirationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Reports device management certificate expiration date. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"iccid\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Integrated Circuit Card Identifier, the SIM card's unique identification number. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"udid\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Unique Device Identifier for iOS and macOS devices. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"notes\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Notes on the device created by IT Admin. Default is null.\"\n    },\n    \"ethernetMacAddress\": {\n      \"type\": [\"string\", \"null\"\
  ],\n      \"description\": \"Indicates Ethernet MAC Address of the device. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"physicalMemoryInBytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Total memory in bytes. Default is 0. This property is read-only.\",\n      \"readOnly\": true,\n      \"default\": 0\n    },\n    \"enrollmentProfileName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Name of the enrollment profile assigned to the device. Default value is empty string. This property is read-only.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\n    \"id\"\n  ],\n  \"$defs\": {\n    \"deviceActionResult\": {\n      \"type\": \"object\",\n      \"title\": \"Device Action Result\",\n      \"description\": \"Device action result returned from performing an action on a managed device.\",\n      \"properties\": {\n        \"@odata.type\": {\n          \"type\": \"string\",\n          \"const\": \"microsoft.graph.deviceActionResult\"\
  \n        },\n        \"actionName\": {\n          \"type\": \"string\",\n          \"description\": \"Action name.\"\n        },\n        \"actionState\": {\n          \"type\": \"string\",\n          \"description\": \"State of the action.\",\n          \"enum\": [\n            \"none\",\n            \"pending\",\n            \"canceled\",\n            \"active\",\n            \"done\",\n            \"failed\",\n            \"notSupported\"\n          ]\n        },\n        \"startDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Time the action was initiated.\"\n        },\n        \"lastUpdatedDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Time the action state was last updated.\"\n        }\n      }\n    },\n    \"configurationManagerClientEnabledFeatures\": {\n      \"type\": \"object\",\n      \"title\": \"Configuration Manager Client Enabled Features\"\
  ,\n      \"description\": \"Represents the enabled features of the Configuration Manager client co-managed with Intune.\",\n      \"properties\": {\n        \"@odata.type\": {\n          \"type\": \"string\",\n          \"const\": \"microsoft.graph.configurationManagerClientEnabledFeatures\"\n        },\n        \"inventory\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether inventory is managed by Intune.\"\n        },\n        \"modernApps\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether modern application is managed by Intune.\"\n        },\n        \"resourceAccess\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether resource access is managed by Intune.\"\n        },\n        \"deviceConfiguration\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether device configuration is managed by Intune.\"\n        },\n        \"compliancePolicy\": {\n          \"type\": \"boolean\",\n        \
  \  \"description\": \"Whether compliance policy is managed by Intune.\"\n        },\n        \"windowsUpdateForBusiness\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether Windows Update for Business is managed by Intune.\"\n        }\n      }\n    },\n    \"deviceHealthAttestationState\": {\n      \"type\": \"object\",\n      \"title\": \"Device Health Attestation State\",\n      \"description\": \"The device health attestation state, providing hardware-based security and health status information.\",\n      \"properties\": {\n        \"@odata.type\": {\n          \"type\": \"string\",\n          \"const\": \"microsoft.graph.deviceHealthAttestationState\"\n        },\n        \"lastUpdateDateTime\": {\n          \"type\": \"string\",\n          \"description\": \"The timestamp of the last update.\"\n        },\n        \"contentNamespaceUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The DHA report version\
  \ (namespace version).\"\n        },\n        \"deviceHealthAttestationStatus\": {\n          \"type\": \"string\",\n          \"description\": \"The device health attestation status.\"\n        },\n        \"contentVersion\": {\n          \"type\": \"string\",\n          \"description\": \"The HealthAttestation state schema version.\"\n        },\n        \"issuedDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The DateTime when device was evaluated or issued to MDM.\"\n        },\n        \"attestationIdentityKey\": {\n          \"type\": \"string\",\n          \"description\": \"TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.\"\n        },\n        \"resetCount\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of times a PC device has hibernated or resumed.\"\n        },\n        \"restartCount\": {\n  \
  \        \"type\": \"integer\",\n          \"description\": \"The number of times a PC device has rebooted.\"\n        },\n        \"dataExcutionPolicy\": {\n          \"type\": \"string\",\n          \"description\": \"DEP policy defines a set of hardware and software technologies that perform additional checks on memory.\"\n        },\n        \"bitLockerStatus\": {\n          \"type\": \"string\",\n          \"description\": \"On or Off of BitLocker Drive Encryption.\"\n        },\n        \"bootManagerVersion\": {\n          \"type\": \"string\",\n          \"description\": \"The version of the Boot Manager.\"\n        },\n        \"codeIntegrityCheckVersion\": {\n          \"type\": \"string\",\n          \"description\": \"The version of the code integrity check.\"\n        },\n        \"secureBoot\": {\n          \"type\": \"string\",\n          \"description\": \"When Secure Boot is enabled, the core components must have correct cryptographic signatures.\"\n        },\n       \
  \ \"bootDebugging\": {\n          \"type\": \"string\",\n          \"description\": \"When bootDebugging is enabled, it is used to provide diagnostic information during development.\"\n        },\n        \"operatingSystemKernelDebugging\": {\n          \"type\": \"string\",\n          \"description\": \"When operatingSystemKernelDebugging is enabled, it allows kernel debugging.\"\n        },\n        \"codeIntegrity\": {\n          \"type\": \"string\",\n          \"description\": \"When code integrity is enabled, code execution is restricted to integrity verified code.\"\n        },\n        \"testSigning\": {\n          \"type\": \"string\",\n          \"description\": \"When test signing is allowed, the device does not enforce signature validation during boot.\"\n        },\n        \"safeMode\": {\n          \"type\": \"string\",\n          \"description\": \"Safe mode is a troubleshooting option for Windows that starts the computer in a limited state.\"\n        },\n        \"windowsPE\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Operating system running with limited services that is used to prepare a computer for Windows.\"\n        },\n        \"earlyLaunchAntiMalwareDriverProtection\": {\n          \"type\": \"string\",\n          \"description\": \"ELAM provides protection for the computers in your network when they start up.\"\n        },\n        \"virtualSecureMode\": {\n          \"type\": \"string\",\n          \"description\": \"VSM is a container that protects high value assets from a compromised kernel.\"\n        },\n        \"pcrHashAlgorithm\": {\n          \"type\": \"string\",\n          \"description\": \"Informational attribute that identifies the HASH algorithm that was used by TPM.\"\n        },\n        \"bootAppSecurityVersion\": {\n          \"type\": \"string\",\n          \"description\": \"The security version number of the Boot Application.\"\n        },\n        \"bootManagerSecurityVersion\": {\n          \"type\":\
  \ \"string\",\n          \"description\": \"The security version number of the Boot Manager.\"\n        },\n        \"tpmVersion\": {\n          \"type\": \"string\",\n          \"description\": \"The security version number of the Boot Application.\"\n        },\n        \"pcr0\": {\n          \"type\": \"string\",\n          \"description\": \"A fingerprint of the legacy BIOS configuration measured in PCR[0].\"\n        },\n        \"secureBootConfigurationPolicyFingerPrint\": {\n          \"type\": \"string\",\n          \"description\": \"Fingerprint of the Custom Secure Boot Configuration Policy.\"\n        },\n        \"codeIntegrityPolicy\": {\n          \"type\": \"string\",\n          \"description\": \"The Code Integrity policy that is controlling the security of the boot environment.\"\n        },\n        \"bootRevisionListInfo\": {\n          \"type\": \"string\",\n          \"description\": \"The Boot Revision List that was loaded during initial boot on the attested device.\"\
  \n        },\n        \"operatingSystemRevListInfo\": {\n          \"type\": \"string\",\n          \"description\": \"The Operating System Revision List that was loaded during initial boot on the attested device.\"\n        },\n        \"healthStatusMismatchInfo\": {\n          \"type\": \"string\",\n          \"description\": \"This attribute appears if DHA-Service detects an integrity issue.\"\n        },\n        \"healthAttestationSupportedStatus\": {\n          \"type\": \"string\",\n          \"description\": \"This attribute indicates if DHA is supported for the device.\"\n        }\n      }\n    }\n  },\n  \"examples\": [\n    {\n      \"@odata.type\": \"#microsoft.graph.managedDevice\",\n      \"id\": \"705c034c-034c-705c-4c03-5c704c035c70\",\n      \"userId\": \"a1b2c3d4-e5f6-7890-abcd-ef1234567890\",\n      \"deviceName\": \"DESKTOP-ABC123\",\n      \"managedDeviceOwnerType\": \"company\",\n      \"enrolledDateTime\": \"2024-01-15T10:30:00Z\",\n      \"lastSyncDateTime\": \"\
  2026-03-01T14:22:00Z\",\n      \"operatingSystem\": \"Windows\",\n      \"complianceState\": \"compliant\",\n      \"jailBroken\": \"False\",\n      \"managementAgent\": \"mdm\",\n      \"osVersion\": \"10.0.22631.3007\",\n      \"easActivated\": false,\n      \"azureADRegistered\": true,\n      \"deviceEnrollmentType\": \"windowsAzureADJoin\",\n      \"isSupervised\": false,\n      \"isEncrypted\": true,\n      \"userPrincipalName\": \"user@contoso.com\",\n      \"model\": \"Surface Pro 9\",\n      \"manufacturer\": \"Microsoft Corporation\",\n      \"serialNumber\": \"012345678901\",\n      \"userDisplayName\": \"Jane Doe\",\n      \"wiFiMacAddress\": \"AA:BB:CC:DD:EE:FF\",\n      \"totalStorageSpaceInBytes\": 512110190592,\n      \"freeStorageSpaceInBytes\": 256055095296,\n      \"managedDeviceName\": \"user_Windows_3/1/2026_2:22 PM\",\n      \"partnerReportedThreatState\": \"secured\",\n      \"physicalMemoryInBytes\": 17179869184,\n      \"notes\": null\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-intune/refs/heads/main/json-schema/microsoft-intune-managed-device-schema.json
tags:
- App Protection
- Azure
- Compliance
- Device Configuration
- Endpoint Management
- Enrollment
- MAM
- MDM
- Microsoft Graph
- Mobile Application Management
- Mobile Device Management
- Security
title: Microsoft Intune Managed Device
---
