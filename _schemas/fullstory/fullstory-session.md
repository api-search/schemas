---
description: A session in FullStory representing a recorded user interaction. Sessions contain events, page views, and behavioral data that can be replayed. Session replay URLs are scoped to the FullStory account and require authenticated access.
layout: schema
name: FullStory Session
properties_list:
- description: Unique identifier for the session
  name: sessionId
  type: string
- description: URL to view the session replay in the FullStory application. Only accessible by browsers logged into the appropriate FullStory account.
  name: url
  type: string
- description: Timestamp when the session was recorded
  name: created
  type: string
provider_name: FullStory
provider_slug: fullstory
schema_file: json-schema/fullstory-session-schema.json
slug: fullstory-session
source_filename: fullstory-session-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://fullstory.com/schemas/fullstory/session.json\",\n  \"title\": \"FullStory Session\",\n  \"description\": \"A session in FullStory representing a recorded user interaction. Sessions contain events, page views, and behavioral data that can be replayed. Session replay URLs are scoped to the FullStory account and require authenticated access.\",\n  \"type\": \"object\",\n  \"required\": [\"sessionId\"],\n  \"properties\": {\n    \"sessionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the session\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to view the session replay in the FullStory application. Only accessible by browsers logged into the appropriate FullStory account.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"\
  Timestamp when the session was recorded\"\n    }\n  },\n  \"$defs\": {\n    \"SessionEvent\": {\n      \"type\": \"object\",\n      \"description\": \"An individual event captured during a session, such as a page view, click, or custom event\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of event captured\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the event occurred during the session\"\n        },\n        \"data\": {\n          \"type\": \"object\",\n          \"description\": \"Event-specific data and properties\",\n          \"additionalProperties\": true\n        }\n      }\n    },\n    \"SessionSummary\": {\n      \"type\": \"object\",\n      \"description\": \"AI-generated summary of a session using a configured prompt profile\",\n      \"properties\": {\n        \"sessionId\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"The session that was summarized\"\n        },\n        \"summary\": {\n          \"type\": \"string\",\n          \"description\": \"The generated summary text or structured response based on the configured response schema\"\n        },\n        \"configProfileId\": {\n          \"type\": \"string\",\n          \"description\": \"The summary prompt profile ID used for generation\"\n        }\n      }\n    },\n    \"SummaryConfigProfile\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration profile for AI session summaries defining prompting instructions and context\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the summary config profile\"\n        },\n        \"pre_prompt\": {\n          \"type\": \"string\",\n          \"description\": \"Instructional text included before the session data for primary instructions and persona setting\"\n \
  \       },\n        \"post_prompt\": {\n          \"type\": \"string\",\n          \"description\": \"Instructional text included after the session data\"\n        },\n        \"response_schema\": {\n          \"type\": \"object\",\n          \"description\": \"JSON Schema defining the structured output format. Recommended for programmatic use of summary data.\",\n          \"additionalProperties\": true\n        },\n        \"slice\": {\n          \"type\": \"object\",\n          \"description\": \"Configuration to trim session data sent to the AI\",\n          \"properties\": {\n            \"mode\": {\n              \"type\": \"string\",\n              \"description\": \"Which events to include: FIRST (earliest), LAST (latest), or TIMESTAMP (specific range)\",\n              \"enum\": [\"FIRST\", \"LAST\", \"TIMESTAMP\"]\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/json-schema/fullstory-session-schema.json
tags:
- Analytics
- Digital Experience
- Session Replay
- Webhooks
- Data Export
title: FullStory Session
---
