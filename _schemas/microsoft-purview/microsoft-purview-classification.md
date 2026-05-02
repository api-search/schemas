---
description: Represents a classification (tag) applied to data entities in Microsoft Purview. Classifications are used for data sensitivity labeling and categorization.
layout: schema
name: Microsoft Purview Classification
properties_list:
- description: The attributes of the classification instance
  name: attributes
  type: object
- description: The name of the classification type (e.g., MICROSOFT.PERSONAL.NAME, MICROSOFT.FINANCIAL.CREDIT_CARD_NUMBER)
  name: typeName
  type: string
- description: ETag for concurrency control
  name: lastModifiedTS
  type: string
- description: The GUID of the entity this classification is applied to
  name: entityGuid
  type: string
- description: The status of the associated entity
  name: entityStatus
  type: string
- description: Whether the classification propagates to child entities
  name: propagate
  type: boolean
- description: Whether propagated classifications are removed when the source entity is deleted
  name: removePropagationsOnEntityDelete
  type: boolean
- description: Time-bounded validity periods for the classification
  name: validityPeriods
  type: array
provider_name: Microsoft Purview
provider_slug: microsoft-purview
schema_file: json-schema/microsoft-purview-classification-schema.json
slug: microsoft-purview-classification
source_filename: microsoft-purview-classification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/microsoft-purview/json-schema/microsoft-purview-classification-schema.json\",\n  \"title\": \"Microsoft Purview Classification\",\n  \"description\": \"Represents a classification (tag) applied to data entities in Microsoft Purview. Classifications are used for data sensitivity labeling and categorization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"The attributes of the classification instance\",\n      \"additionalProperties\": true\n    },\n    \"typeName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the classification type (e.g., MICROSOFT.PERSONAL.NAME, MICROSOFT.FINANCIAL.CREDIT_CARD_NUMBER)\"\n    },\n    \"lastModifiedTS\": {\n      \"type\": \"string\",\n      \"description\": \"ETag for concurrency control\"\n    },\n    \"entityGuid\": {\n      \"\
  type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The GUID of the entity this classification is applied to\"\n    },\n    \"entityStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the associated entity\",\n      \"enum\": [\"ACTIVE\", \"DELETED\"]\n    },\n    \"propagate\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the classification propagates to child entities\",\n      \"default\": true\n    },\n    \"removePropagationsOnEntityDelete\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether propagated classifications are removed when the source entity is deleted\",\n      \"default\": false\n    },\n    \"validityPeriods\": {\n      \"type\": \"array\",\n      \"description\": \"Time-bounded validity periods for the classification\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"endTime\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"The end time of the validity period\"\n          },\n          \"startTime\": {\n            \"type\": \"string\",\n            \"description\": \"The start time of the validity period\"\n          },\n          \"timeZone\": {\n            \"type\": \"string\",\n            \"description\": \"The time zone\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"typeName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/json-schema/microsoft-purview-classification-schema.json
tags:
- Compliance
- Data Catalog
- Data Classification
- Data Governance
- Data Loss Prevention
- Information Protection
title: Microsoft Purview Classification
---
