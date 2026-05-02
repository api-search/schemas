---
description: The payload delivered by LaunchDarkly webhooks when changes occur to resources. The format is identical to audit log entries.
layout: schema
name: LaunchDarkly Webhook Event
properties_list:
- description: The unique identifier of this audit log event.
  name: _id
  type: string
- description: Unix epoch timestamp in milliseconds when the change occurred. Use this to reorder events since webhooks may arrive out of order.
  name: date
  type: integer
- description: The kind of resource that was changed.
  name: kind
  type: string
- description: The name of the resource that was changed.
  name: name
  type: string
- description: A markdown-formatted description of the changes made.
  name: description
  type: string
- description: A brief plain-text summary of the change.
  name: shortDescription
  type: string
- description: An optional comment provided by the member who made the change.
  name: comment
  type: string
- description: The access details describing what action was taken on which resource.
  name: accesses
  type: array
- description: ''
  name: member
  type: object
- description: The verb describing the action taken, such as created, updated, or deleted.
  name: titleVerb
  type: string
- description: A human-readable title for the event.
  name: title
  type: string
- description: Details about the target resource.
  name: target
  type: object
- description: HATEOAS links to related resources.
  name: _links
  type: object
provider_name: launchdarkly
provider_slug: launchdarkly
schema_file: json-schema/launchdarkly-webhook-event-schema.json
slug: launchdarkly-webhook-event
source_filename: launchdarkly-webhook-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://launchdarkly.com/schemas/launchdarkly/webhook-event.json\",\n  \"title\": \"LaunchDarkly Webhook Event\",\n  \"description\": \"The payload delivered by LaunchDarkly webhooks when changes occur to resources. The format is identical to audit log entries.\",\n  \"type\": \"object\",\n  \"required\": [\"_id\", \"date\", \"kind\", \"name\"],\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of this audit log event.\"\n    },\n    \"date\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Unix epoch timestamp in milliseconds when the change occurred. Use this to reorder events since webhooks may arrive out of order.\",\n      \"minimum\": 0\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The kind of resource that was changed.\",\n      \"enum\": [\n        \"\
  flag\",\n        \"project\",\n        \"environment\",\n        \"segment\",\n        \"metric\",\n        \"member\",\n        \"role\",\n        \"webhook\",\n        \"integration\",\n        \"token\",\n        \"destination\",\n        \"relay-proxy-config\",\n        \"experiment\",\n        \"team\",\n        \"release-pipeline\"\n      ]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the resource that was changed.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A markdown-formatted description of the changes made.\"\n    },\n    \"shortDescription\": {\n      \"type\": \"string\",\n      \"description\": \"A brief plain-text summary of the change.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"An optional comment provided by the member who made the change.\"\n    },\n    \"accesses\": {\n      \"type\": \"array\",\n      \"description\": \"The access details\
  \ describing what action was taken on which resource.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Access\"\n      }\n    },\n    \"member\": {\n      \"$ref\": \"#/$defs/MemberRef\"\n    },\n    \"titleVerb\": {\n      \"type\": \"string\",\n      \"description\": \"The verb describing the action taken, such as created, updated, or deleted.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable title for the event.\"\n    },\n    \"target\": {\n      \"type\": \"object\",\n      \"description\": \"Details about the target resource.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the target resource.\"\n        },\n        \"resources\": {\n          \"type\": \"array\",\n          \"description\": \"The resource specifiers for the target.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"_links\": {\n          \"\
  type\": \"object\",\n          \"description\": \"Links to the target resource.\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/Link\"\n          }\n        }\n      }\n    },\n    \"_links\": {\n      \"type\": \"object\",\n      \"description\": \"HATEOAS links to related resources.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/Link\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Access\": {\n      \"type\": \"object\",\n      \"description\": \"An access record describing what action was performed on which resource.\",\n      \"properties\": {\n        \"action\": {\n          \"type\": \"string\",\n          \"description\": \"The action that was performed, such as createFlag, updateOn, deleteFlag, or updateTargets.\"\n        },\n        \"resource\": {\n          \"type\": \"string\",\n          \"description\": \"A resource specifier in the format proj/{projKey}:env/{envKey}:flag/{flagKey}.\"\n        }\n      }\n    },\n    \"MemberRef\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"A reference to the account member who made the change.\",\n      \"properties\": {\n        \"_id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the member.\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The email address of the member.\"\n        },\n        \"firstName\": {\n          \"type\": \"string\",\n          \"description\": \"The first name of the member.\"\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n          \"description\": \"The last name of the member.\"\n        },\n        \"_links\": {\n          \"type\": \"object\",\n          \"description\": \"Links related to the member.\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/Link\"\n          }\n        }\n      }\n    },\n    \"Link\": {\n      \"type\": \"object\",\n      \"\
  description\": \"A HATEOAS link.\",\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"description\": \"The URL of the linked resource.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The media type of the linked resource.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/launchdarkly/refs/heads/main/json-schema/launchdarkly-webhook-event-schema.json
tags: []
title: LaunchDarkly Webhook Event
---
