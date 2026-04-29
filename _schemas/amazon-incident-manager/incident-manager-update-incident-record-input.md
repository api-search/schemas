---
description: UpdateIncidentRecordInput schema
layout: schema
name: UpdateIncidentRecordInput
properties_list:
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
  name: impact
  type: object
- description: ''
  name: notificationTargets
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: summary
  type: object
- description: ''
  name: title
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-update-incident-record-input-schema.json
slug: incident-manager-update-incident-record-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-update-incident-record-input-schema.json\",\n  \"title\": \"UpdateIncidentRecordInput\",\n  \"description\": \"UpdateIncidentRecordInput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the incident record you are updating.\"\n        }\n      ]\n    },\n    \"chatChannel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChatChannel\"\n        },\n        {\n          \"description\": \"The Chatbot chat channel where responders can collaborate.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\
  \n        },\n        {\n          \"description\": \"A token that ensures that a client calls the operation only once with the specified details.\"\n        }\n      ]\n    },\n    \"impact\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Impact\"\n        },\n        {\n          \"description\": \"<p>Defines the impact of the incident to customers and applications. If you provide an impact for an incident, it overwrites the impact provided by the response plan.</p> <p class=\\\"title\\\"> <b>Possible impacts:</b> </p> <ul> <li> <p> <code>1</code> - Critical impact, full application failure that impacts many to all customers. </p> </li> <li> <p> <code>2</code> - High impact, partial application failure with impact to many customers.</p> </li> <li> <p> <code>3</code> - Medium impact, the application is providing reduced service to customers.</p> </li> <li> <p> <code>4</code> - Low impact, customer aren't impacted by the problem yet.</p> </li> <li> <p> <code>5</code>\
  \ - No impact, customers aren't currently impacted but urgent action is needed to avoid impact.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"notificationTargets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationTargetSet\"\n        },\n        {\n          \"description\": \"<p>The Amazon SNS targets that Incident Manager notifies when a client updates an incident.</p> <p>Using multiple SNS topics creates redundancy in the event that a Region is down during the incident.</p>\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncidentRecordStatus\"\n        },\n        {\n          \"description\": \"The status of the incident. Possible statuses are <code>Open</code> or <code>Resolved</code>.\"\n        }\n      ]\n    },\n    \"summary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncidentSummary\"\n        },\n        {\n        \
  \  \"description\": \"A longer description of what occurred during the incident.\"\n        }\n      ]\n    },\n    \"title\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncidentTitle\"\n        },\n        {\n          \"description\": \"A brief description of the incident.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-update-incident-record-input-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: UpdateIncidentRecordInput
---
