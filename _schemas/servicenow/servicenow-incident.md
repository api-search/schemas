---
description: A ServiceNow incident record used for tracking disruptions to IT services, reporting issues, and managing resolution workflows within IT Service Management.
layout: schema
name: ServiceNow Incident
properties_list:
- description: The unique 32-character system identifier for the incident record.
  name: sys_id
  type: string
- description: The human-readable incident number, prefixed with INC.
  name: number
  type: string
- description: A brief summary of the incident used as the primary display title.
  name: short_description
  type: string
- description: A detailed description of the incident including symptoms and impact.
  name: description
  type:
  - string
  - 'null'
- description: 'The current state of the incident: 1=New, 2=In Progress, 3=On Hold, 6=Resolved, 7=Closed, 8=Canceled.'
  name: state
  type: string
- description: 'The impact level: 1=High, 2=Medium, 3=Low.'
  name: impact
  type: string
- description: 'The urgency level: 1=High, 2=Medium, 3=Low.'
  name: urgency
  type: string
- description: 'The calculated priority: 1=Critical, 2=High, 3=Moderate, 4=Low, 5=Planning.'
  name: priority
  type: string
- description: 'The severity level: 1=High, 2=Medium, 3=Low.'
  name: severity
  type: string
- description: The category of the incident, such as Inquiry, Software, Hardware, or Network.
  name: category
  type:
  - string
  - 'null'
- description: The subcategory providing further classification within the category.
  name: subcategory
  type:
  - string
  - 'null'
- description: The method through which the incident was reported, such as phone, email, or self-service.
  name: contact_type
  type:
  - string
  - 'null'
- description: The user who reported the incident.
  name: caller_id
  type: object
- description: The user assigned to work on the incident.
  name: assigned_to
  type: object
- description: The group responsible for resolving the incident.
  name: assignment_group
  type: object
- description: The user who created the incident record.
  name: opened_by
  type: object
- description: The date and time the incident was opened.
  name: opened_at
  type: string
- description: The user who resolved the incident.
  name: resolved_by
  type: object
- description: The date and time the incident was resolved.
  name: resolved_at
  type:
  - string
  - 'null'
- description: The user who closed the incident.
  name: closed_by
  type: object
- description: The date and time the incident was closed.
  name: closed_at
  type:
  - string
  - 'null'
- description: The code indicating how the incident was resolved.
  name: close_code
  type:
  - string
  - 'null'
- description: Notes recorded at the time of resolution or closure.
  name: close_notes
  type:
  - string
  - 'null'
- description: The configuration item affected by the incident.
  name: cmdb_ci
  type: object
- description: The business service impacted by the incident.
  name: business_service
  type: object
- description: The company associated with the incident.
  name: company
  type: object
- description: The location associated with the incident.
  name: location
  type: object
- description: 'Notification preference: 1=Do Not Notify, 2=Send Notifications, 3=Send Notifications for state changes.'
  name: notify
  type: string
- description: Internal work notes visible only to the fulfillment team.
  name: work_notes
  type:
  - string
  - 'null'
- description: Additional comments visible to the caller.
  name: comments
  type:
  - string
  - 'null'
- description: The number of times the incident has been reopened.
  name: reopen_count
  type: integer
- description: The number of times the incident has been reassigned.
  name: reassignment_count
  type: integer
- description: 'The escalation level: 0=Normal, 1=Overdue, 2=Moderate, 3=High.'
  name: escalation
  type: string
- description: Action to take when an approval is rejected.
  name: upon_reject
  type:
  - string
  - 'null'
- description: Action to take when an approval is granted.
  name: upon_approval
  type:
  - string
  - 'null'
- description: Whether the incident record is active.
  name: active
  type: boolean
- description: Whether the incident has been flagged as a knowledge candidate.
  name: knowledge
  type: boolean
- description: Whether the incident resolution met the SLA target.
  name: made_sla
  type: boolean
- description: The date and time the record was created.
  name: sys_created_on
  type: string
- description: The user who created the record.
  name: sys_created_by
  type: string
- description: The date and time the record was last updated.
  name: sys_updated_on
  type: string
- description: The user who last updated the record.
  name: sys_updated_by
  type: string
- description: The number of times the record has been modified.
  name: sys_mod_count
  type: integer
- description: The table class name for the record.
  name: sys_class_name
  type: string
- description: The domain of the record.
  name: sys_domain
  type: object
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-incident-schema.json
slug: servicenow-incident
source_filename: servicenow-incident-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://servicenow.com/schemas/servicenow/incident.json\",\n  \"title\": \"ServiceNow Incident\",\n  \"description\": \"A ServiceNow incident record used for tracking disruptions to IT services, reporting issues, and managing resolution workflows within IT Service Management.\",\n  \"type\": \"object\",\n  \"required\": [\"sys_id\", \"number\", \"short_description\", \"state\"],\n  \"properties\": {\n    \"sys_id\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[a-f0-9]{32}$\",\n      \"description\": \"The unique 32-character system identifier for the incident record.\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"pattern\": \"^INC[0-9]+$\",\n      \"description\": \"The human-readable incident number, prefixed with INC.\"\n    },\n    \"short_description\": {\n      \"type\": \"string\",\n      \"maxLength\": 160,\n      \"description\": \"A brief summary of the incident\
  \ used as the primary display title.\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A detailed description of the incident including symptoms and impact.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"1\", \"2\", \"3\", \"6\", \"7\", \"8\"],\n      \"description\": \"The current state of the incident: 1=New, 2=In Progress, 3=On Hold, 6=Resolved, 7=Closed, 8=Canceled.\"\n    },\n    \"impact\": {\n      \"type\": \"string\",\n      \"enum\": [\"1\", \"2\", \"3\"],\n      \"description\": \"The impact level: 1=High, 2=Medium, 3=Low.\"\n    },\n    \"urgency\": {\n      \"type\": \"string\",\n      \"enum\": [\"1\", \"2\", \"3\"],\n      \"description\": \"The urgency level: 1=High, 2=Medium, 3=Low.\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"enum\": [\"1\", \"2\", \"3\", \"4\", \"5\"],\n      \"description\": \"The calculated priority: 1=Critical, 2=High, 3=Moderate, 4=Low, 5=Planning.\"\
  \n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\"1\", \"2\", \"3\"],\n      \"description\": \"The severity level: 1=High, 2=Medium, 3=Low.\"\n    },\n    \"category\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The category of the incident, such as Inquiry, Software, Hardware, or Network.\"\n    },\n    \"subcategory\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The subcategory providing further classification within the category.\"\n    },\n    \"contact_type\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The method through which the incident was reported, such as phone, email, or self-service.\"\n    },\n    \"caller_id\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The user who reported the incident.\"\n    },\n    \"assigned_to\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The user assigned to work on the incident.\"\n\
  \    },\n    \"assignment_group\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The group responsible for resolving the incident.\"\n    },\n    \"opened_by\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The user who created the incident record.\"\n    },\n    \"opened_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the incident was opened.\"\n    },\n    \"resolved_by\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The user who resolved the incident.\"\n    },\n    \"resolved_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the incident was resolved.\"\n    },\n    \"closed_by\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The user who closed the incident.\"\n    },\n    \"closed_at\": {\n      \"type\": [\"string\", \"null\"],\n\
  \      \"format\": \"date-time\",\n      \"description\": \"The date and time the incident was closed.\"\n    },\n    \"close_code\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The code indicating how the incident was resolved.\"\n    },\n    \"close_notes\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Notes recorded at the time of resolution or closure.\"\n    },\n    \"cmdb_ci\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The configuration item affected by the incident.\"\n    },\n    \"business_service\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The business service impacted by the incident.\"\n    },\n    \"company\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The company associated with the incident.\"\n    },\n    \"location\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The location associated with the incident.\"\
  \n    },\n    \"notify\": {\n      \"type\": \"string\",\n      \"enum\": [\"1\", \"2\", \"3\"],\n      \"description\": \"Notification preference: 1=Do Not Notify, 2=Send Notifications, 3=Send Notifications for state changes.\"\n    },\n    \"work_notes\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Internal work notes visible only to the fulfillment team.\"\n    },\n    \"comments\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Additional comments visible to the caller.\"\n    },\n    \"reopen_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of times the incident has been reopened.\"\n    },\n    \"reassignment_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of times the incident has been reassigned.\"\n    },\n    \"escalation\": {\n      \"type\": \"string\",\n      \"enum\": [\"0\", \"1\", \"2\", \"3\"],\n      \"description\": \"\
  The escalation level: 0=Normal, 1=Overdue, 2=Moderate, 3=High.\"\n    },\n    \"upon_reject\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Action to take when an approval is rejected.\"\n    },\n    \"upon_approval\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Action to take when an approval is granted.\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the incident record is active.\"\n    },\n    \"knowledge\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the incident has been flagged as a knowledge candidate.\"\n    },\n    \"made_sla\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the incident resolution met the SLA target.\"\n    },\n    \"sys_created_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the record was created.\"\n    },\n    \"sys_created_by\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The user who created the record.\"\n    },\n    \"sys_updated_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the record was last updated.\"\n    },\n    \"sys_updated_by\": {\n      \"type\": \"string\",\n      \"description\": \"The user who last updated the record.\"\n    },\n    \"sys_mod_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of times the record has been modified.\"\n    },\n    \"sys_class_name\": {\n      \"type\": \"string\",\n      \"description\": \"The table class name for the record.\"\n    },\n    \"sys_domain\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The domain of the record.\"\n    }\n  },\n  \"$defs\": {\n    \"ReferenceField\": {\n      \"type\": [\"object\", \"string\", \"null\"],\n      \"description\": \"A ServiceNow reference field that can be a sys_id string or an object containing\
  \ a link and value.\",\n      \"properties\": {\n        \"link\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The API URL to the referenced record.\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The sys_id of the referenced record.\"\n        },\n        \"display_value\": {\n          \"type\": \"string\",\n          \"description\": \"The display value of the referenced record.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-incident-schema.json
tags:
- Automation
- Cloud Services
- Digital Workflows
- Enterprise Platform
- IT Service Management
- ITSM
- Processes
- T1
- Workflow Automation
- Workflows
title: ServiceNow Incident
---
