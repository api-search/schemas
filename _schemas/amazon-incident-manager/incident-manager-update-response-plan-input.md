---
description: UpdateResponsePlanInput schema
layout: schema
name: UpdateResponsePlanInput
properties_list:
- description: ''
  name: actions
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: chatChannel
  type: object
- description: ''
  name: clientToken
  type: object
- description: ''
  name: displayName
  type: object
- description: ''
  name: engagements
  type: object
- description: ''
  name: incidentTemplateDedupeString
  type: object
- description: ''
  name: incidentTemplateImpact
  type: object
- description: ''
  name: incidentTemplateNotificationTargets
  type: object
- description: ''
  name: incidentTemplateSummary
  type: object
- description: ''
  name: incidentTemplateTags
  type: object
- description: ''
  name: incidentTemplateTitle
  type: object
- description: ''
  name: integrations
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-update-response-plan-input-schema.json
slug: incident-manager-update-response-plan-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-update-response-plan-input-schema.json\",\n  \"title\": \"UpdateResponsePlanInput\",\n  \"description\": \"UpdateResponsePlanInput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionsList\"\n        },\n        {\n          \"description\": \"The actions that this response plan takes at the beginning of an incident.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the response plan.\"\n        }\n      ]\n    },\n    \"chatChannel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChatChannel\"\
  \n        },\n        {\n          \"description\": \"<p>The Chatbot chat channel used for collaboration during an incident.</p> <p>Use the empty structure to remove the chat channel from the response plan.</p>\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A token ensuring that the operation is called only once with the specified details.\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResponsePlanDisplayName\"\n        },\n        {\n          \"description\": \"The long format name of the response plan. The display name can't contain spaces.\"\n        }\n      ]\n    },\n    \"engagements\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngagementSet\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name\
  \ (ARN) for the contacts and escalation plans that the response plan engages during an incident.\"\n        }\n      ]\n    },\n    \"incidentTemplateDedupeString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DedupeString\"\n        },\n        {\n          \"description\": \"The string Incident Manager uses to prevent duplicate incidents from being created by the same incident in the same account.\"\n        }\n      ]\n    },\n    \"incidentTemplateImpact\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Impact\"\n        },\n        {\n          \"description\": \"<p>Defines the impact to the customers. Providing an impact overwrites the impact provided by a response plan.</p> <p class=\\\"title\\\"> <b>Possible impacts:</b> </p> <ul> <li> <p> <code>5</code> - Severe impact</p> </li> <li> <p> <code>4</code> - High impact</p> </li> <li> <p> <code>3</code> - Medium impact</p> </li> <li> <p> <code>2</code> - Low impact</p>\
  \ </li> <li> <p> <code>1</code> - No impact</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"incidentTemplateNotificationTargets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationTargetSet\"\n        },\n        {\n          \"description\": \"The Amazon SNS targets that are notified when updates are made to an incident.\"\n        }\n      ]\n    },\n    \"incidentTemplateSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncidentSummary\"\n        },\n        {\n          \"description\": \"A brief summary of the incident. This typically contains what has happened, what's currently happening, and next steps.\"\n        }\n      ]\n    },\n    \"incidentTemplateTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMapUpdate\"\n        },\n        {\n          \"description\": \"Tags to assign to the template. When the <code>StartIncident</code> API action is called, Incident\
  \ Manager assigns the tags specified in the template to the incident. To call this action, you must also have permission to call the <code>TagResource</code> API action for the incident record resource.\"\n        }\n      ]\n    },\n    \"incidentTemplateTitle\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncidentTitle\"\n        },\n        {\n          \"description\": \"The short format name of the incident. The title can't contain spaces.\"\n        }\n      ]\n    },\n    \"integrations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integrations\"\n        },\n        {\n          \"description\": \"Information about third-party services integrated into the response plan.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-update-response-plan-input-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: UpdateResponsePlanInput
---
