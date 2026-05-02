---
description: Represents a retention label for records management in Microsoft Purview. Retention labels define how long data should be retained and what happens after the retention period.
layout: schema
name: Microsoft Purview Retention Label
properties_list:
- description: The unique identifier of the retention label
  name: id
  type: string
- description: The display name of the retention label
  name: displayName
  type: string
- description: Description visible to administrators
  name: descriptionForAdmins
  type: string
- description: Description visible to end users
  name: descriptionForUsers
  type: string
- description: Whether the label is currently in use
  name: isInUse
  type: boolean
- description: What triggers the start of the retention period
  name: retentionTrigger
  type: string
- description: The behavior during the retention period
  name: behaviorDuringRetentionPeriod
  type: string
- description: What happens after the retention period ends
  name: actionAfterRetentionPeriod
  type: string
- description: The duration of the retention period
  name: retentionDuration
  type: object
- description: The default record behavior
  name: defaultRecordBehavior
  type: string
- description: ''
  name: createdDateTime
  type: string
- description: ''
  name: lastModifiedDateTime
  type: string
provider_name: Microsoft Purview
provider_slug: microsoft-purview
schema_file: json-schema/microsoft-purview-retention-label-schema.json
slug: microsoft-purview-retention-label
source_filename: microsoft-purview-retention-label-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/microsoft-purview/json-schema/microsoft-purview-retention-label-schema.json\",\n  \"title\": \"Microsoft Purview Retention Label\",\n  \"description\": \"Represents a retention label for records management in Microsoft Purview. Retention labels define how long data should be retained and what happens after the retention period.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the retention label\",\n      \"readOnly\": true\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the retention label\"\n    },\n    \"descriptionForAdmins\": {\n      \"type\": \"string\",\n      \"description\": \"Description visible to administrators\"\n    },\n    \"descriptionForUsers\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Description visible to end users\"\n    },\n    \"isInUse\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the label is currently in use\",\n      \"readOnly\": true\n    },\n    \"retentionTrigger\": {\n      \"type\": \"string\",\n      \"description\": \"What triggers the start of the retention period\",\n      \"enum\": [\"dateLabeled\", \"dateCreated\", \"dateModified\", \"dateOfEvent\"]\n    },\n    \"behaviorDuringRetentionPeriod\": {\n      \"type\": \"string\",\n      \"description\": \"The behavior during the retention period\",\n      \"enum\": [\"doNotRetain\", \"retain\", \"retainAsRecord\", \"retainAsRegulatoryRecord\"]\n    },\n    \"actionAfterRetentionPeriod\": {\n      \"type\": \"string\",\n      \"description\": \"What happens after the retention period ends\",\n      \"enum\": [\"none\", \"delete\", \"startDispositionReview\"]\n    },\n    \"retentionDuration\": {\n      \"type\": \"object\",\n      \"description\": \"The duration of the retention\
  \ period\",\n      \"properties\": {\n        \"@odata.type\": {\n          \"type\": \"string\"\n        },\n        \"days\": {\n          \"type\": \"integer\",\n          \"description\": \"The retention duration in days\"\n        }\n      }\n    },\n    \"defaultRecordBehavior\": {\n      \"type\": \"string\",\n      \"description\": \"The default record behavior\",\n      \"enum\": [\"startLocked\", \"startUnlocked\"]\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"displayName\", \"behaviorDuringRetentionPeriod\", \"actionAfterRetentionPeriod\", \"retentionDuration\", \"retentionTrigger\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/json-schema/microsoft-purview-retention-label-schema.json
tags:
- Compliance
- Data Catalog
- Data Classification
- Data Governance
- Data Loss Prevention
- Information Protection
title: Microsoft Purview Retention Label
---
