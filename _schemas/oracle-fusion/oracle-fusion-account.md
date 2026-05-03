---
description: A customer account (organization party) in Oracle Fusion Cloud CX representing a company or organization that is a prospect, customer, or partner in the CRM system.
layout: schema
name: Oracle Fusion Cloud CX Account
properties_list:
- description: Unique system-generated party identifier
  name: PartyId
  type: integer
- description: Unique party number for the account
  name: PartyNumber
  type: string
- description: Organization (account) name
  name: OrganizationName
  type: string
- description: Account type classification
  name: Type
  type: string
- description: Account owner (sales representative) name
  name: OwnerName
  type: string
- description: Industry classification (e.g., Technology, Healthcare, Finance)
  name: Industry
  type: string
- description: Estimated annual revenue of the organization
  name: AnnualRevenue
  type: number
- description: Approximate number of employees
  name: NumberOfEmployees
  type: integer
- description: Primary phone number
  name: PhoneNumber
  type: string
- description: Primary email address
  name: EmailAddress
  type: string
- description: Company website URL
  name: URL
  type: string
- description: ''
  name: PrimaryAddress
  type: object
- description: Customer classification or segmentation
  name: CustomerClassification
  type: string
- description: Account status
  name: Status
  type: string
- description: Record creation timestamp
  name: CreationDate
  type: string
- description: Last modification timestamp
  name: LastUpdateDate
  type: string
provider_name: Oracle Fusion Cloud Applications
provider_slug: oracle-fusion
schema_file: json-schema/oracle-fusion-account-schema.json
slug: oracle-fusion-account
source_filename: oracle-fusion-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.oracle.com/schemas/oracle-fusion/account.json\",\n  \"title\": \"Oracle Fusion Cloud CX Account\",\n  \"description\": \"A customer account (organization party) in Oracle Fusion Cloud CX representing a company or organization that is a prospect, customer, or partner in the CRM system.\",\n  \"type\": \"object\",\n  \"required\": [\"OrganizationName\"],\n  \"properties\": {\n    \"PartyId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique system-generated party identifier\"\n    },\n    \"PartyNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Unique party number for the account\"\n    },\n    \"OrganizationName\": {\n      \"type\": \"string\",\n      \"description\": \"Organization (account) name\",\n      \"minLength\": 1,\n      \"maxLength\": 360\n    },\n    \"Type\": {\n      \"type\": \"string\",\n      \"description\": \"Account type classification\"\
  \n    },\n    \"OwnerName\": {\n      \"type\": \"string\",\n      \"description\": \"Account owner (sales representative) name\"\n    },\n    \"Industry\": {\n      \"type\": \"string\",\n      \"description\": \"Industry classification (e.g., Technology, Healthcare, Finance)\"\n    },\n    \"AnnualRevenue\": {\n      \"type\": \"number\",\n      \"description\": \"Estimated annual revenue of the organization\",\n      \"minimum\": 0\n    },\n    \"NumberOfEmployees\": {\n      \"type\": \"integer\",\n      \"description\": \"Approximate number of employees\",\n      \"minimum\": 0\n    },\n    \"PhoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Primary phone number\"\n    },\n    \"EmailAddress\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Primary email address\"\n    },\n    \"URL\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Company website URL\"\n    },\n    \"PrimaryAddress\"\
  : {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"CustomerClassification\": {\n      \"type\": \"string\",\n      \"description\": \"Customer classification or segmentation\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Active\", \"Inactive\"],\n      \"description\": \"Account status\"\n    },\n    \"CreationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record creation timestamp\"\n    },\n    \"LastUpdateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp\"\n    }\n  },\n  \"$defs\": {\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"Physical address for the account\",\n      \"properties\": {\n        \"AddressLine1\": {\n          \"type\": \"string\",\n          \"description\": \"Primary address line\"\n        },\n        \"AddressLine2\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Secondary address line\"\n        },\n        \"City\": {\n          \"type\": \"string\",\n          \"description\": \"City name\"\n        },\n        \"State\": {\n          \"type\": \"string\",\n          \"description\": \"State or province\"\n        },\n        \"PostalCode\": {\n          \"type\": \"string\",\n          \"description\": \"Postal or ZIP code\"\n        },\n        \"Country\": {\n          \"type\": \"string\",\n          \"description\": \"Country name or ISO code\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-fusion/refs/heads/main/json-schema/oracle-fusion-account-schema.json
tags:
- Cloud
- CX
- Enterprise
- EPM
- ERP
- HCM
- Project Management
- REST API
- SaaS
- SCM
title: Oracle Fusion Cloud CX Account
---
