---
description: Abstract base class containing the base properties for Intune mobile apps. Represents the mobileApp resource type from the Microsoft Graph API. Platform-specific app types (iOS, Android, Windows, web) inherit from this base type.
layout: schema
name: Mobile Application
properties_list:
- description: Key of the entity. This property is read-only.
  name: id
  type: string
- description: The admin provided or imported title of the app.
  name: displayName
  type: string
- description: The description of the app.
  name: description
  type:
  - string
  - 'null'
- description: The publisher of the app.
  name: publisher
  type:
  - string
  - 'null'
- description: The large icon, to be displayed in the app details and used for upload of the icon.
  name: largeIcon
  type: object
- description: The date and time the app was created.
  name: createdDateTime
  type: string
- description: The date and time the app was last modified.
  name: lastModifiedDateTime
  type: string
- description: The value indicating whether the app is marked as featured by the admin.
  name: isFeatured
  type: boolean
- description: The privacy statement URL.
  name: privacyInformationUrl
  type:
  - string
  - 'null'
- description: The more information URL.
  name: informationUrl
  type:
  - string
  - 'null'
- description: The owner of the app.
  name: owner
  type:
  - string
  - 'null'
- description: The developer of the app.
  name: developer
  type:
  - string
  - 'null'
- description: Notes for the app.
  name: notes
  type:
  - string
  - 'null'
- description: The publishing state for the app. The app cannot be assigned unless published.
  name: publishingState
  type: string
- description: The list of categories for this app.
  name: categories
  type: array
- description: The list of group assignments for this mobile app.
  name: assignments
  type: array
provider_name: Microsoft Endpoint Configuration Management
provider_slug: microsoft-endpoint-configuration-management
schema_file: json-schema/microsoft-endpoint-configuration-management-application-schema.json
slug: microsoft-endpoint-configuration-management-application
source_filename: microsoft-endpoint-configuration-management-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/kinlane/microsoft-endpoint-configuration-management/json-schema/microsoft-endpoint-configuration-management-application-schema.json\",\n  \"title\": \"Mobile Application\",\n  \"description\": \"Abstract base class containing the base properties for Intune mobile apps. Represents the mobileApp resource type from the Microsoft Graph API. Platform-specific app types (iOS, Android, Windows, web) inherit from this base type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Key of the entity. This property is read-only.\",\n      \"readOnly\": true\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The admin provided or imported title of the app.\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The description of the app.\"\n\
  \    },\n    \"publisher\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The publisher of the app.\"\n    },\n    \"largeIcon\": {\n      \"$ref\": \"#/$defs/MimeContent\",\n      \"description\": \"The large icon, to be displayed in the app details and used for upload of the icon.\"\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the app was created.\",\n      \"readOnly\": true\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the app was last modified.\",\n      \"readOnly\": true\n    },\n    \"isFeatured\": {\n      \"type\": \"boolean\",\n      \"description\": \"The value indicating whether the app is marked as featured by the admin.\"\n    },\n    \"privacyInformationUrl\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\"\
  : \"The privacy statement URL.\"\n    },\n    \"informationUrl\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"The more information URL.\"\n    },\n    \"owner\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The owner of the app.\"\n    },\n    \"developer\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The developer of the app.\"\n    },\n    \"notes\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Notes for the app.\"\n    },\n    \"publishingState\": {\n      \"type\": \"string\",\n      \"description\": \"The publishing state for the app. The app cannot be assigned unless published.\",\n      \"enum\": [\"notPublished\", \"processing\", \"published\"],\n      \"readOnly\": true\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"description\": \"The list of categories for this app.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/MobileAppCategory\"\
  \n      }\n    },\n    \"assignments\": {\n      \"type\": \"array\",\n      \"description\": \"The list of group assignments for this mobile app.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/MobileAppAssignment\"\n      }\n    }\n  },\n  \"required\": [\"displayName\"],\n  \"$defs\": {\n    \"MimeContent\": {\n      \"type\": \"object\",\n      \"description\": \"Contains properties for a generic MIME content.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The MIME type.\"\n        },\n        \"value\": {\n          \"type\": [\"string\", \"null\"],\n          \"contentEncoding\": \"base64\",\n          \"description\": \"The byte array content (base64 encoded).\"\n        }\n      }\n    },\n    \"MobileAppCategory\": {\n      \"type\": \"object\",\n      \"description\": \"Contains properties for an Intune app category.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n\
  \          \"description\": \"Key of the entity.\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the app category.\"\n        },\n        \"lastModifiedDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time the category was last modified.\"\n        }\n      }\n    },\n    \"MobileAppAssignment\": {\n      \"type\": \"object\",\n      \"description\": \"A class containing the properties used for Group Assignment of a Mobile App.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Key of the entity.\"\n        },\n        \"intent\": {\n          \"type\": \"string\",\n          \"description\": \"The install intent defined by the admin.\",\n          \"enum\": [\"available\", \"required\", \"uninstall\", \"availableWithoutEnrollment\"]\n        },\n        \"target\": {\n          \"\
  $ref\": \"#/$defs/DeviceAndAppManagementAssignmentTarget\",\n          \"description\": \"The target group assignment.\"\n        },\n        \"settings\": {\n          \"$ref\": \"#/$defs/MobileAppAssignmentSettings\",\n          \"description\": \"The settings for target assignment.\"\n        }\n      }\n    },\n    \"DeviceAndAppManagementAssignmentTarget\": {\n      \"type\": \"object\",\n      \"description\": \"Base type for assignment targets.\",\n      \"properties\": {\n        \"@odata.type\": {\n          \"type\": \"string\",\n          \"description\": \"Type discriminator for the target type.\"\n        },\n        \"groupId\": {\n          \"type\": \"string\",\n          \"description\": \"The group ID that is the target of the assignment.\"\n        }\n      }\n    },\n    \"MobileAppAssignmentSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Abstract class containing properties used to assign a mobile app to a group.\",\n      \"properties\": {\n \
  \       \"@odata.type\": {\n          \"type\": \"string\",\n          \"description\": \"Type discriminator for platform-specific settings.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-endpoint-configuration-management/refs/heads/main/json-schema/microsoft-endpoint-configuration-management-application-schema.json
tags:
- Compliance
- Configuration Management
- Device Management
- Endpoint Management
- Mobile Device Management
- Patch Management
- Software Deployment
title: Mobile Application
---
