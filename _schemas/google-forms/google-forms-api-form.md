---
description: A Google Form with items, settings, and metadata.
layout: schema
name: Form
properties_list:
- description: Output only. The form ID.
  name: formId
  type: string
- description: General information about the form.
  name: info
  type: object
- description: Form-level settings including quiz configuration.
  name: settings
  type: object
- description: A list of the form's items including section headers, questions, and media.
  name: items
  type: array
- description: Output only. The revision ID of the form.
  name: revisionId
  type: string
- description: Output only. The form URI to share with responders.
  name: responderUri
  type: string
- description: Output only. The ID of the linked Google Sheet.
  name: linkedSheetId
  type: string
- description: ''
  name: publishSettings
  type: object
provider_name: Google Forms
provider_slug: google-forms
schema_file: json-schema/google-forms-api-form-schema.json
slug: google-forms-api-form
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-forms/refs/heads/main/json-schema/google-forms-api-form-schema.json\",\n  \"title\": \"Form\",\n  \"description\": \"A Google Form with items, settings, and metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"formId\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The form ID.\",\n      \"readOnly\": true\n    },\n    \"info\": {\n      \"type\": \"object\",\n      \"description\": \"General information about the form.\",\n      \"properties\": {\n        \"title\": { \"type\": \"string\", \"description\": \"Required. The title of the form visible to responders.\" },\n        \"documentTitle\": { \"type\": \"string\", \"description\": \"Output only. The title of the document visible in Google Drive.\", \"readOnly\": true },\n        \"description\": { \"type\": \"string\", \"description\": \"The description\
  \ of the form.\" }\n      },\n      \"required\": [\"title\"]\n    },\n    \"settings\": {\n      \"type\": \"object\",\n      \"description\": \"Form-level settings including quiz configuration.\",\n      \"properties\": {\n        \"quizSettings\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"isQuiz\": { \"type\": \"boolean\", \"description\": \"Whether this form is a quiz.\" }\n          }\n        },\n        \"emailCollectionType\": {\n          \"type\": \"string\",\n          \"enum\": [\"EMAIL_COLLECTION_TYPE_UNSPECIFIED\", \"DO_NOT_COLLECT\", \"VERIFIED\", \"RESPONDER_INPUT\"]\n        }\n      }\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"A list of the form's items including section headers, questions, and media.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"itemId\": { \"type\": \"string\" },\n          \"title\": { \"type\": \"string\" },\n          \"description\"\
  : { \"type\": \"string\" }\n        }\n      }\n    },\n    \"revisionId\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The revision ID of the form.\",\n      \"readOnly\": true\n    },\n    \"responderUri\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The form URI to share with responders.\",\n      \"readOnly\": true\n    },\n    \"linkedSheetId\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The ID of the linked Google Sheet.\",\n      \"readOnly\": true\n    },\n    \"publishSettings\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"isPublished\": { \"type\": \"boolean\" },\n        \"isAcceptingResponses\": { \"type\": \"boolean\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-forms/refs/heads/main/json-schema/google-forms-api-form-schema.json
tags:
- Data Collection
- Forms
- Google
- Google Workspace
- Questionnaires
- Responses
- Surveys
title: Form
---
