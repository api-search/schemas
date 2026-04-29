---
description: ''
layout: schema
name: DiscreteJob
properties_list:
- description: WIP entity identifier
  name: wipEntityId
  type: integer
- description: Job name/number
  name: wipEntityName
  type: string
- description: Organization identifier
  name: organizationId
  type: integer
- description: Primary assembly item identifier
  name: primaryItemId
  type: integer
- description: Primary assembly item number
  name: primaryItemNumber
  type: string
- description: Job status (1=Unreleased, 3=Released, 4=Complete, 5=Complete-No Charges, 6=On Hold, 7=Cancelled, 12=Closed, 14=Pending Close, 15=Failed Close)
  name: statusType
  type: integer
- description: Job type (1=Standard, 3=Non-Standard)
  name: jobType
  type: integer
- description: Start quantity
  name: startQuantity
  type: number
- description: Quantity completed
  name: quantityCompleted
  type: number
- description: Quantity scrapped
  name: quantityScrapped
  type: number
- description: Net quantity remaining
  name: netQuantity
  type: number
- description: Scheduled start date
  name: scheduledStartDate
  type: string
- description: Scheduled completion date
  name: scheduledCompletionDate
  type: string
- description: Date released
  name: dateReleased
  type: string
- description: Date completed
  name: dateCompleted
  type: string
- description: Date closed
  name: dateClosed
  type: string
- description: Accounting class code
  name: classCode
  type: string
- description: BOM revision
  name: bomRevision
  type: string
- description: Routing revision
  name: routingRevision
  type: string
- description: Job description
  name: description
  type: string
- description: Firm planned flag (1=Firm, 2=Not Firm)
  name: firmPlannedFlag
  type: integer
- description: ''
  name: creationDate
  type: string
- description: ''
  name: lastUpdateDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/manufacturing-discrete-job-schema.json
slug: manufacturing-discrete-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DiscreteJob\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"wipEntityId\": {\n      \"type\": \"integer\",\n      \"description\": \"WIP entity identifier\"\n    },\n    \"wipEntityName\": {\n      \"type\": \"string\",\n      \"description\": \"Job name/number\"\n    },\n    \"organizationId\": {\n      \"type\": \"integer\",\n      \"description\": \"Organization identifier\"\n    },\n    \"primaryItemId\": {\n      \"type\": \"integer\",\n      \"description\": \"Primary assembly item identifier\"\n    },\n    \"primaryItemNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Primary assembly item number\"\n    },\n    \"statusType\": {\n      \"type\": \"integer\",\n      \"description\": \"Job status (1=Unreleased, 3=Released, 4=Complete, 5=Complete-No Charges, 6=On Hold, 7=Cancelled, 12=Closed, 14=Pending Close, 15=Failed Close)\"\n    },\n    \"jobType\": {\n    \
  \  \"type\": \"integer\",\n      \"description\": \"Job type (1=Standard, 3=Non-Standard)\"\n    },\n    \"startQuantity\": {\n      \"type\": \"number\",\n      \"description\": \"Start quantity\"\n    },\n    \"quantityCompleted\": {\n      \"type\": \"number\",\n      \"description\": \"Quantity completed\"\n    },\n    \"quantityScrapped\": {\n      \"type\": \"number\",\n      \"description\": \"Quantity scrapped\"\n    },\n    \"netQuantity\": {\n      \"type\": \"number\",\n      \"description\": \"Net quantity remaining\"\n    },\n    \"scheduledStartDate\": {\n      \"type\": \"string\",\n      \"description\": \"Scheduled start date\"\n    },\n    \"scheduledCompletionDate\": {\n      \"type\": \"string\",\n      \"description\": \"Scheduled completion date\"\n    },\n    \"dateReleased\": {\n      \"type\": \"string\",\n      \"description\": \"Date released\"\n    },\n    \"dateCompleted\": {\n      \"type\": \"string\",\n      \"description\": \"Date completed\"\n    },\n\
  \    \"dateClosed\": {\n      \"type\": \"string\",\n      \"description\": \"Date closed\"\n    },\n    \"classCode\": {\n      \"type\": \"string\",\n      \"description\": \"Accounting class code\"\n    },\n    \"bomRevision\": {\n      \"type\": \"string\",\n      \"description\": \"BOM revision\"\n    },\n    \"routingRevision\": {\n      \"type\": \"string\",\n      \"description\": \"Routing revision\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Job description\"\n    },\n    \"firmPlannedFlag\": {\n      \"type\": \"integer\",\n      \"description\": \"Firm planned flag (1=Firm, 2=Not Firm)\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\"\n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/manufacturing-discrete-job-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: DiscreteJob
---
