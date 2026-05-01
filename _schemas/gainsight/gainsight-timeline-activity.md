---
description: Represents a timeline activity record in Gainsight CS, capturing customer interactions such as calls, meetings, emails, and notes for a chronological view of the customer relationship.
layout: schema
name: Gainsight Timeline Activity
properties_list:
- description: Activity unique identifier
  name: Gsid
  type: string
- description: Activity subject line
  name: Subject
  type: string
- description: Activity notes or body content
  name: Notes
  type: string
- description: Activity type identifier
  name: ActivityTypeId
  type: string
- description: Activity type display name (e.g., Call, Meeting, Email)
  name: ActivityTypeName
  type: string
- description: Associated company Gsid
  name: CompanyId
  type: string
- description: Associated company name
  name: CompanyName
  type: string
- description: Date and time of the activity
  name: ActivityDate
  type: string
- description: Activity owner user ID
  name: OwnerId
  type: string
- description: Activity owner display name
  name: OwnerName
  type: string
- description: External system identifier for deduplication
  name: ExternalId
  type: string
- description: List of attendees for the activity
  name: Attendees
  type: array
- description: Sentiment captured during the activity
  name: Sentiment
  type: string
- description: Record creation timestamp
  name: CreatedDate
  type: string
- description: Record last modification timestamp
  name: ModifiedDate
  type: string
provider_name: Gainsight
provider_slug: gainsight
schema_file: json-schema/gainsight-timeline-activity-schema.json
slug: gainsight-timeline-activity
source_filename: gainsight-timeline-activity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.gainsight.com/schemas/gainsight/timeline-activity.json\",\n  \"title\": \"Gainsight Timeline Activity\",\n  \"description\": \"Represents a timeline activity record in Gainsight CS, capturing customer interactions such as calls, meetings, emails, and notes for a chronological view of the customer relationship.\",\n  \"type\": \"object\",\n  \"required\": [\"Subject\", \"ActivityTypeId\", \"CompanyId\", \"ActivityDate\"],\n  \"properties\": {\n    \"Gsid\": {\n      \"type\": \"string\",\n      \"description\": \"Activity unique identifier\"\n    },\n    \"Subject\": {\n      \"type\": \"string\",\n      \"description\": \"Activity subject line\"\n    },\n    \"Notes\": {\n      \"type\": \"string\",\n      \"description\": \"Activity notes or body content\"\n    },\n    \"ActivityTypeId\": {\n      \"type\": \"string\",\n      \"description\": \"Activity type identifier\"\n    },\n\
  \    \"ActivityTypeName\": {\n      \"type\": \"string\",\n      \"description\": \"Activity type display name (e.g., Call, Meeting, Email)\"\n    },\n    \"CompanyId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated company Gsid\"\n    },\n    \"CompanyName\": {\n      \"type\": \"string\",\n      \"description\": \"Associated company name\"\n    },\n    \"ActivityDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time of the activity\"\n    },\n    \"OwnerId\": {\n      \"type\": \"string\",\n      \"description\": \"Activity owner user ID\"\n    },\n    \"OwnerName\": {\n      \"type\": \"string\",\n      \"description\": \"Activity owner display name\"\n    },\n    \"ExternalId\": {\n      \"type\": \"string\",\n      \"description\": \"External system identifier for deduplication\"\n    },\n    \"Attendees\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\"\
  : {\n          \"personId\": {\n            \"type\": \"string\",\n            \"description\": \"Gainsight person Gsid\"\n          },\n          \"email\": {\n            \"type\": \"string\",\n            \"format\": \"email\",\n            \"description\": \"Attendee email address\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Attendee name\"\n          }\n        }\n      },\n      \"description\": \"List of attendees for the activity\"\n    },\n    \"Sentiment\": {\n      \"type\": \"string\",\n      \"enum\": [\"Positive\", \"Neutral\", \"Negative\"],\n      \"description\": \"Sentiment captured during the activity\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record creation timestamp\"\n    },\n    \"ModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record last modification timestamp\"\n\
  \    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/json-schema/gainsight-timeline-activity-schema.json
tags: []
title: Gainsight Timeline Activity
---
