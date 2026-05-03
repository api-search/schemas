---
description: A federal contract opportunity published on SAM.gov
layout: schema
name: SAM.gov Contract Opportunity
properties_list:
- description: Unique identifier for the notice
  name: noticeId
  type: string
- description: Title of the contract opportunity
  name: title
  type: string
- description: Solicitation number assigned by the agency
  name: solicitationNumber
  type: string
- description: Type of notice
  name: type
  type: string
- description: Base type of the notice
  name: baseType
  type: string
- description: Archive type
  name: archiveType
  type: string
- description: Date when opportunity will be archived
  name: archiveDate
  type: string
- description: North American Industry Classification System code
  name: naicsCode
  type: string
- description: Federal Supply Classification (FSC) or Product Service Code (PSC)
  name: classificationCode
  type: string
- description: Contracting department/agency details
  name: department
  type: object
- description: Office address of the contracting office
  name: officeAddress
  type: object
- description: Location where work will be performed
  name: placeOfPerformance
  type: object
- description: Full text description of the opportunity
  name: description
  type: string
- description: Type of organization
  name: organizationType
  type: string
- description: Small business set-aside details
  name: setAside
  type: object
- description: Deadline for responses/proposals
  name: responseDeadLine
  type: string
- description: Whether the opportunity is currently active
  name: active
  type: string
- description: Award details if this notice is an award
  name: award
  type: object
- description: URL to view opportunity on SAM.gov
  name: uiLink
  type: string
- description: Date opportunity was posted
  name: postedDate
  type: string
- description: Date opportunity was last modified
  name: modifiedDate
  type: string
provider_name: SAM.gov
provider_slug: sam.gov
schema_file: json-schema/sam-gov-opportunity-schema.json
slug: sam-gov-opportunity
source_filename: sam-gov-opportunity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/sam.gov/json-schema/sam-gov-opportunity-schema.json\",\n  \"title\": \"SAM.gov Contract Opportunity\",\n  \"description\": \"A federal contract opportunity published on SAM.gov\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"noticeId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the notice\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the contract opportunity\"\n    },\n    \"solicitationNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Solicitation number assigned by the agency\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of notice\",\n      \"enum\": [\n        \"Presolicitation\",\n        \"Combined Synopsis/Solicitation\",\n        \"Solicitation\",\n        \"Award Notice\",\n        \"Special Notice\",\n   \
  \     \"Sources Sought\",\n        \"Intent to Bundle Requirements\",\n        \"Justification and Approval\"\n      ]\n    },\n    \"baseType\": {\n      \"type\": \"string\",\n      \"description\": \"Base type of the notice\"\n    },\n    \"archiveType\": {\n      \"type\": \"string\",\n      \"description\": \"Archive type\"\n    },\n    \"archiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date when opportunity will be archived\"\n    },\n    \"naicsCode\": {\n      \"type\": \"string\",\n      \"description\": \"North American Industry Classification System code\"\n    },\n    \"classificationCode\": {\n      \"type\": \"string\",\n      \"description\": \"Federal Supply Classification (FSC) or Product Service Code (PSC)\"\n    },\n    \"department\": {\n      \"type\": \"object\",\n      \"description\": \"Contracting department/agency details\",\n      \"properties\": {\n        \"departmentId\": {\n          \"type\": \"string\"\
  \n        },\n        \"departmentName\": {\n          \"type\": \"string\"\n        },\n        \"subTier\": {\n          \"type\": \"string\"\n        },\n        \"office\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"officeAddress\": {\n      \"type\": \"object\",\n      \"description\": \"Office address of the contracting office\",\n      \"properties\": {\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"state\": {\n          \"type\": \"string\"\n        },\n        \"zip\": {\n          \"type\": \"string\"\n        },\n        \"countryCode\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"placeOfPerformance\": {\n      \"type\": \"object\",\n      \"description\": \"Location where work will be performed\",\n      \"properties\": {\n        \"city\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"code\": {\"type\": \"string\"},\n            \"name\": {\"type\": \"string\"}\n\
  \          }\n        },\n        \"state\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"code\": {\"type\": \"string\"},\n            \"name\": {\"type\": \"string\"}\n          }\n        },\n        \"country\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"code\": {\"type\": \"string\"},\n            \"name\": {\"type\": \"string\"}\n          }\n        },\n        \"zip\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Full text description of the opportunity\"\n    },\n    \"organizationType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of organization\"\n    },\n    \"setAside\": {\n      \"type\": \"object\",\n      \"description\": \"Small business set-aside details\",\n      \"properties\": {\n        \"setAsideCode\": {\n          \"type\": \"string\"\n        },\n        \"setAsideDescription\":\
  \ {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"responseDeadLine\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Deadline for responses/proposals\"\n    },\n    \"active\": {\n      \"type\": \"string\",\n      \"enum\": [\"Yes\", \"No\"],\n      \"description\": \"Whether the opportunity is currently active\"\n    },\n    \"award\": {\n      \"type\": \"object\",\n      \"description\": \"Award details if this notice is an award\",\n      \"properties\": {\n        \"date\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"number\": {\n          \"type\": \"string\"\n        },\n        \"amount\": {\n          \"type\": \"string\"\n        },\n        \"awardee\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": {\"type\": \"string\"},\n            \"location\": {\n              \"type\": \"object\"\n            },\n            \"ueiSAM\"\
  : {\"type\": \"string\"}\n          }\n        }\n      }\n    },\n    \"uiLink\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to view opportunity on SAM.gov\"\n    },\n    \"postedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date opportunity was posted\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date opportunity was last modified\"\n    }\n  },\n  \"required\": [\"noticeId\", \"title\", \"type\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sam.gov/refs/heads/main/json-schema/sam-gov-opportunity-schema.json
tags:
- Federal Government
- Procurement
- Contracts
- Entity Management
- Location Services
- GSA
title: SAM.gov Contract Opportunity
---
