---
description: A business entity tracked within the Harbor Compliance platform, including formation details, compliance status, registered agent, licenses, and filing obligations.
layout: schema
name: Harbor Compliance Business Entity
properties_list:
- description: Unique entity identifier assigned by Harbor Compliance
  name: id
  type: string
- description: Legal name of the business entity
  name: name
  type: string
- description: Legal structure of the business entity
  name: entity_type
  type: string
- description: Two-letter US state code where the entity was formed
  name: state_of_formation
  type: string
- description: Employer Identification Number in XX-XXXXXXX format
  name: ein
  type: string
- description: Current compliance and operational status of the entity
  name: status
  type: string
- description: ''
  name: registered_agent
  type: object
- description: Business licenses associated with this entity
  name: licenses
  type: array
- description: State filing obligations for this entity
  name: filings
  type: array
- description: States where the entity is foreign-qualified to do business
  name: foreign_qualifications
  type: array
- description: ISO 8601 timestamp when the entity record was created
  name: created_at
  type: string
- description: ISO 8601 timestamp of the most recent update
  name: updated_at
  type: string
provider_name: Harbor Compliance
provider_slug: harbor-compliance
schema_file: json-schema/harbor-compliance-entity-schema.json
slug: harbor-compliance-entity
source_filename: harbor-compliance-entity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.harborcompliance.com/schemas/entity.json\",\n  \"title\": \"Harbor Compliance Business Entity\",\n  \"description\": \"A business entity tracked within the Harbor Compliance platform, including formation details, compliance status, registered agent, licenses, and filing obligations.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"entity_type\", \"state_of_formation\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique entity identifier assigned by Harbor Compliance\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Legal name of the business entity\"\n    },\n    \"entity_type\": {\n      \"type\": \"string\",\n      \"enum\": [\"corporation\", \"llc\", \"partnership\", \"nonprofit\", \"sole_proprietorship\"],\n      \"description\": \"Legal structure of the business entity\"\n    },\n\
  \    \"state_of_formation\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{2}$\",\n      \"description\": \"Two-letter US state code where the entity was formed\"\n    },\n    \"ein\": {\n      \"type\": \"string\",\n      \"pattern\": \"^\\\\d{2}-\\\\d{7}$\",\n      \"description\": \"Employer Identification Number in XX-XXXXXXX format\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"inactive\", \"dissolved\", \"suspended\"],\n      \"description\": \"Current compliance and operational status of the entity\"\n    },\n    \"registered_agent\": {\n      \"$ref\": \"#/$defs/RegisteredAgent\"\n    },\n    \"licenses\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/License\" },\n      \"description\": \"Business licenses associated with this entity\"\n    },\n    \"filings\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/Filing\" },\n      \"description\": \"State filing obligations for this\
  \ entity\"\n    },\n    \"foreign_qualifications\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^[A-Z]{2}$\"\n      },\n      \"description\": \"States where the entity is foreign-qualified to do business\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the entity record was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the most recent update\"\n    }\n  },\n  \"$defs\": {\n    \"RegisteredAgent\": {\n      \"type\": \"object\",\n      \"required\": [\"id\", \"jurisdiction\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Registered agent service identifier\"\n        },\n        \"agent_name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of\
  \ the registered agent\"\n        },\n        \"address\": {\n          \"$ref\": \"#/$defs/Address\"\n        },\n        \"jurisdiction\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{2}$\",\n          \"description\": \"State where the registered agent is serving\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"active\", \"inactive\"],\n          \"description\": \"Registered agent service status\"\n        },\n        \"service_start\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Date when the registered agent service began\"\n        }\n      }\n    },\n    \"License\": {\n      \"type\": \"object\",\n      \"required\": [\"id\", \"license_type\", \"jurisdiction\", \"status\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique license identifier\"\n        },\n        \"license_type\": {\n        \
  \  \"type\": \"string\",\n          \"description\": \"Type or category of business license\"\n        },\n        \"jurisdiction\": {\n          \"type\": \"string\",\n          \"description\": \"State or locality where the license is issued\"\n        },\n        \"license_number\": {\n          \"type\": \"string\",\n          \"description\": \"Official license number from the issuing authority\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"active\", \"expired\", \"pending\", \"cancelled\"],\n          \"description\": \"Current license status\"\n        },\n        \"issued_date\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Date the license was issued\"\n        },\n        \"expiration_date\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"License expiration date\"\n        },\n        \"renewal_date\": {\n          \"type\": \"\
  string\",\n          \"format\": \"date\",\n          \"description\": \"Recommended renewal date before expiration\"\n        },\n        \"fee\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"description\": \"License fee amount in USD\"\n        }\n      }\n    },\n    \"Filing\": {\n      \"type\": \"object\",\n      \"required\": [\"id\", \"filing_type\", \"jurisdiction\", \"status\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique filing identifier\"\n        },\n        \"filing_type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of required filing (e.g., annual_report)\"\n        },\n        \"jurisdiction\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{2}$\",\n          \"description\": \"State requiring the filing\"\n        },\n        \"due_date\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\"\
  : \"Filing deadline\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"pending\", \"filed\", \"overdue\", \"waived\"],\n          \"description\": \"Current filing status\"\n        },\n        \"filed_date\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Date the filing was submitted\"\n        },\n        \"fee\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"description\": \"Filing fee in USD\"\n        }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"required\": [\"street1\", \"city\", \"state\", \"zip\"],\n      \"properties\": {\n        \"street1\": {\n          \"type\": \"string\",\n          \"description\": \"Primary street address line\"\n        },\n        \"street2\": {\n          \"type\": \"string\",\n          \"description\": \"Secondary address line (suite, unit, floor)\"\n        },\n        \"city\": {\n          \"\
  type\": \"string\",\n          \"description\": \"City name\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{2}$\",\n          \"description\": \"Two-letter US state code\"\n        },\n        \"zip\": {\n          \"type\": \"string\",\n          \"pattern\": \"^\\\\d{5}(-\\\\d{4})?$\",\n          \"description\": \"ZIP or ZIP+4 postal code\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"default\": \"US\",\n          \"description\": \"ISO 3166-1 alpha-2 country code\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/harbor-compliance/refs/heads/main/json-schema/harbor-compliance-entity-schema.json
tags:
- Business Licensing
- Compliance
- Legal
- Regulatory
title: Harbor Compliance Business Entity
---
