---
description: Represents a Call to Action record in Gainsight CS Cockpit, used to drive proactive customer success actions based on risk, opportunity, or lifecycle events.
layout: schema
name: Gainsight Call to Action (CTA)
properties_list:
- description: CTA unique identifier
  name: Gsid
  type: string
- description: CTA name or subject
  name: Name
  type: string
- description: Associated company Gsid
  name: CompanyId
  type: string
- description: Associated company name
  name: CompanyName
  type: string
- description: CTA type identifier (e.g., Risk, Opportunity, Lifecycle)
  name: TypeId
  type: string
- description: CTA type display name
  name: TypeName
  type: string
- description: CTA reason identifier
  name: ReasonId
  type: string
- description: CTA reason display name
  name: ReasonName
  type: string
- description: Priority level identifier
  name: PriorityId
  type: string
- description: CTA status identifier
  name: StatusId
  type: string
- description: Status display name
  name: StatusName
  type: string
- description: Assigned owner user ID
  name: OwnerId
  type: string
- description: Assigned owner name
  name: OwnerName
  type: string
- description: Due date for the CTA
  name: DueDate
  type: string
- description: Date the CTA was closed
  name: ClosedDate
  type: string
- description: CTA comments or notes
  name: Comments
  type: string
- description: Source that triggered the CTA (e.g., Rule, Manual, API)
  name: Source
  type: string
- description: Associated playbook identifier
  name: PlaybookId
  type: string
- description: Record creation timestamp
  name: CreatedDate
  type: string
- description: Record last modification timestamp
  name: ModifiedDate
  type: string
provider_name: Gainsight
provider_slug: gainsight
schema_file: json-schema/gainsight-cta-schema.json
slug: gainsight-cta
source_filename: gainsight-cta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.gainsight.com/schemas/gainsight/cta.json\",\n  \"title\": \"Gainsight Call to Action (CTA)\",\n  \"description\": \"Represents a Call to Action record in Gainsight CS Cockpit, used to drive proactive customer success actions based on risk, opportunity, or lifecycle events.\",\n  \"type\": \"object\",\n  \"required\": [\"CompanyId\", \"TypeId\", \"ReasonId\", \"PriorityId\", \"StatusId\"],\n  \"properties\": {\n    \"Gsid\": {\n      \"type\": \"string\",\n      \"description\": \"CTA unique identifier\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"CTA name or subject\"\n    },\n    \"CompanyId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated company Gsid\"\n    },\n    \"CompanyName\": {\n      \"type\": \"string\",\n      \"description\": \"Associated company name\"\n    },\n    \"TypeId\": {\n      \"type\": \"string\",\n \
  \     \"description\": \"CTA type identifier (e.g., Risk, Opportunity, Lifecycle)\"\n    },\n    \"TypeName\": {\n      \"type\": \"string\",\n      \"description\": \"CTA type display name\"\n    },\n    \"ReasonId\": {\n      \"type\": \"string\",\n      \"description\": \"CTA reason identifier\"\n    },\n    \"ReasonName\": {\n      \"type\": \"string\",\n      \"description\": \"CTA reason display name\"\n    },\n    \"PriorityId\": {\n      \"type\": \"string\",\n      \"description\": \"Priority level identifier\"\n    },\n    \"StatusId\": {\n      \"type\": \"string\",\n      \"description\": \"CTA status identifier\"\n    },\n    \"StatusName\": {\n      \"type\": \"string\",\n      \"description\": \"Status display name\"\n    },\n    \"OwnerId\": {\n      \"type\": \"string\",\n      \"description\": \"Assigned owner user ID\"\n    },\n    \"OwnerName\": {\n      \"type\": \"string\",\n      \"description\": \"Assigned owner name\"\n    },\n    \"DueDate\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"date\",\n      \"description\": \"Due date for the CTA\"\n    },\n    \"ClosedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the CTA was closed\"\n    },\n    \"Comments\": {\n      \"type\": \"string\",\n      \"description\": \"CTA comments or notes\"\n    },\n    \"Source\": {\n      \"type\": \"string\",\n      \"description\": \"Source that triggered the CTA (e.g., Rule, Manual, API)\"\n    },\n    \"PlaybookId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated playbook identifier\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record creation timestamp\"\n    },\n    \"ModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record last modification timestamp\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/json-schema/gainsight-cta-schema.json
tags: []
title: Gainsight Call to Action (CTA)
---
