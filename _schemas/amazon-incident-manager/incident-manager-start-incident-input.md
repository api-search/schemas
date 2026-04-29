---
description: StartIncidentInput schema
layout: schema
name: StartIncidentInput
properties_list:
- description: ''
  name: clientToken
  type: object
- description: ''
  name: impact
  type: object
- description: ''
  name: relatedItems
  type: object
- description: ''
  name: responsePlanArn
  type: object
- description: ''
  name: title
  type: object
- description: ''
  name: triggerDetails
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-start-incident-input-schema.json
slug: incident-manager-start-incident-input
source_filename: incident-manager-start-incident-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-start-incident-input-schema.json\",\n  \"title\": \"StartIncidentInput\",\n  \"description\": \"StartIncidentInput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A token ensuring that the operation is called only once with the specified details.\"\n        }\n      ]\n    },\n    \"impact\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Impact\"\n        },\n        {\n          \"description\": \"<p>Defines the impact to the customers. Providing an impact overwrites the impact provided by a response plan.</p> <p class=\\\"title\\\"> <b>Possible impacts:</b> </p> <ul> <li> <p>\
  \ <code>1</code> - Critical impact, this typically relates to full application failure that impacts many to all customers. </p> </li> <li> <p> <code>2</code> - High impact, partial application failure with impact to many customers.</p> </li> <li> <p> <code>3</code> - Medium impact, the application is providing reduced service to customers.</p> </li> <li> <p> <code>4</code> - Low impact, customer might aren't impacted by the problem yet.</p> </li> <li> <p> <code>5</code> - No impact, customers aren't currently impacted but urgent action is needed to avoid impact.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"relatedItems\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RelatedItemList\"\n        },\n        {\n          \"description\": \"Add related items to the incident for other responders to use. Related items are Amazon Web Services resources, external links, or files uploaded to an Amazon S3 bucket. \"\n        }\n      ]\n    },\n    \"responsePlanArn\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the response plan that pre-defines summary, chat channels, Amazon SNS topics, runbooks, title, and impact of the incident. \"\n        }\n      ]\n    },\n    \"title\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncidentTitle\"\n        },\n        {\n          \"description\": \"Provide a title for the incident. Providing a title overwrites the title provided by the response plan. \"\n        }\n      ]\n    },\n    \"triggerDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TriggerDetails\"\n        },\n        {\n          \"description\": \"Details of what created the incident record in Incident Manager.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"responsePlanArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-start-incident-input-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: StartIncidentInput
---
