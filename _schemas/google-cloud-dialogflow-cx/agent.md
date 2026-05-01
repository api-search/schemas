---
description: A Dialogflow CX agent resource representing a conversational virtual agent.
layout: schema
name: Agent
properties_list:
- description: Resource name of the agent.
  name: name
  type: string
- description: Human-readable name of the agent.
  name: displayName
  type: string
- description: Default language of the agent as a BCP-47 language tag.
  name: defaultLanguageCode
  type: string
- description: List of additional supported language codes.
  name: supportedLanguageCodes
  type: array
- description: Time zone of the agent from the IANA time zone database.
  name: timeZone
  type: string
- description: Description of the agent.
  name: description
  type: string
- description: URI of the agent avatar.
  name: avatarUri
  type: string
- description: Name of the start flow in the agent.
  name: startFlow
  type: string
- description: Name of the security settings resource.
  name: securitySettings
  type: string
- description: Whether to enable Stackdriver logging for the agent.
  name: enableStackdriverLogging
  type: boolean
- description: Whether to enable spell correction for the agent.
  name: enableSpellCorrection
  type: boolean
- description: Whether the agent is locked for changes.
  name: locked
  type: boolean
- description: Speech-to-text settings.
  name: speechToTextSettings
  type: object
provider_name: Google Cloud Dialogflow CX
provider_slug: google-cloud-dialogflow-cx
schema_file: json-schema/agent.json
slug: agent
source_filename: agent.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-dialogflow-cx/refs/heads/main/json-schema/agent.json\",\n  \"title\": \"Agent\",\n  \"description\": \"A Dialogflow CX agent resource representing a conversational virtual agent.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name of the agent.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the agent.\"\n    },\n    \"defaultLanguageCode\": {\n      \"type\": \"string\",\n      \"description\": \"Default language of the agent as a BCP-47 language tag.\"\n    },\n    \"supportedLanguageCodes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of additional supported language codes.\"\n    },\n    \"timeZone\": {\n   \
  \   \"type\": \"string\",\n      \"description\": \"Time zone of the agent from the IANA time zone database.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the agent.\"\n    },\n    \"avatarUri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URI of the agent avatar.\"\n    },\n    \"startFlow\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the start flow in the agent.\"\n    },\n    \"securitySettings\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the security settings resource.\"\n    },\n    \"enableStackdriverLogging\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable Stackdriver logging for the agent.\"\n    },\n    \"enableSpellCorrection\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable spell correction for the agent.\"\n    },\n    \"locked\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether the agent is locked for changes.\"\n    },\n    \"speechToTextSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Speech-to-text settings.\",\n      \"properties\": {\n        \"enableSpeechAdaptation\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to use speech adaptation.\"\n        }\n      }\n    }\n  },\n  \"required\": [\"displayName\", \"defaultLanguageCode\", \"timeZone\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dialogflow-cx/refs/heads/main/json-schema/agent.json
tags:
- Chatbots
- Conversational AI
- Dialogflow
- Google Cloud
- NLU
- Virtual Agents
title: Agent
---
