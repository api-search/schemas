---
description: An Account business component record in Oracle Siebel CRM representing a customer, prospect, or partner organization. Accounts are the primary organizational entity in Siebel CRM and serve as the parent for contacts, opportunities, service requests, orders, and other related business components.
layout: schema
name: Oracle Siebel CRM Account
properties_list:
- description: Unique system-generated row identifier for the account record
  name: Id
  type: string
- description: Account name representing the organization
  name: Name
  type: string
- description: Location identifier distinguishing multiple sites for the same organization (e.g., Headquarters, HQ-Distribution)
  name: Location
  type: string
- description: Current lifecycle status of the account
  name: Account Status
  type: string
- description: Type classification of the account (e.g., Customer, Prospect, Partner, Competitor)
  name: Account Type
  type: string
- description: Detailed description of the account and business relationship
  name: Description
  type: string
- description: Industry classification for the organization
  name: Industry
  type: string
- description: Name of the primary Siebel organization associated with the account for visibility and access control
  name: Primary Organization
  type: string
- description: Row identifier of the primary Siebel organization
  name: Primary Organization Id
  type: string
- description: Primary telephone number for the account
  name: Main Phone Number
  type: string
- description: Primary fax number for the account
  name: Main Fax Number
  type: string
- description: Primary email address for the account
  name: Email Address
  type: string
- description: Website URL for the account organization
  name: Home Page
  type: string
- description: Current business volume or revenue amount
  name: Current Volume
  type: number
- description: Alternate name or alias for the account
  name: Alias
  type: string
- description: Row identifier of the parent account for hierarchical account structures
  name: Parent Account Id
  type: string
- description: Customer service number assigned to the account
  name: CSN
  type: string
- description: Dun and Bradstreet DUNS number for the organization
  name: DUNS Number
  type: string
- description: Approximate number of employees in the organization
  name: Number of Employees
  type: integer
- description: Estimated annual revenue of the organization
  name: Annual Revenue
  type: number
- description: ISO 4217 currency code for monetary values
  name: Currency Code
  type: string
- description: ''
  name: Address
  type: object
provider_name: Oracle Siebel
provider_slug: oracle-siebel
schema_file: json-schema/oracle-siebel-account-schema.json
slug: oracle-siebel-account
source_filename: oracle-siebel-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.oracle.com/schemas/oracle-siebel/account.json\",\n  \"title\": \"Oracle Siebel CRM Account\",\n  \"description\": \"An Account business component record in Oracle Siebel CRM representing a customer, prospect, or partner organization. Accounts are the primary organizational entity in Siebel CRM and serve as the parent for contacts, opportunities, service requests, orders, and other related business components.\",\n  \"type\": \"object\",\n  \"required\": [\"Name\"],\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique system-generated row identifier for the account record\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Account name representing the organization\",\n      \"minLength\": 1,\n      \"maxLength\": 100\n    },\n    \"Location\": {\n      \"type\": \"string\",\n      \"description\": \"Location\
  \ identifier distinguishing multiple sites for the same organization (e.g., Headquarters, HQ-Distribution)\"\n    },\n    \"Account Status\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle status of the account\",\n      \"enum\": [\"Active\", \"Inactive\", \"Unverified\", \"Verified\"]\n    },\n    \"Account Type\": {\n      \"type\": \"string\",\n      \"description\": \"Type classification of the account (e.g., Customer, Prospect, Partner, Competitor)\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of the account and business relationship\"\n    },\n    \"Industry\": {\n      \"type\": \"string\",\n      \"description\": \"Industry classification for the organization\"\n    },\n    \"Primary Organization\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the primary Siebel organization associated with the account for visibility and access control\"\n    },\n    \"Primary Organization\
  \ Id\": {\n      \"type\": \"string\",\n      \"description\": \"Row identifier of the primary Siebel organization\"\n    },\n    \"Main Phone Number\": {\n      \"type\": \"string\",\n      \"description\": \"Primary telephone number for the account\"\n    },\n    \"Main Fax Number\": {\n      \"type\": \"string\",\n      \"description\": \"Primary fax number for the account\"\n    },\n    \"Email Address\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Primary email address for the account\"\n    },\n    \"Home Page\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Website URL for the account organization\"\n    },\n    \"Current Volume\": {\n      \"type\": \"number\",\n      \"description\": \"Current business volume or revenue amount\",\n      \"minimum\": 0\n    },\n    \"Alias\": {\n      \"type\": \"string\",\n      \"description\": \"Alternate name or alias for the account\"\n    },\n    \"Parent Account\
  \ Id\": {\n      \"type\": \"string\",\n      \"description\": \"Row identifier of the parent account for hierarchical account structures\"\n    },\n    \"CSN\": {\n      \"type\": \"string\",\n      \"description\": \"Customer service number assigned to the account\"\n    },\n    \"DUNS Number\": {\n      \"type\": \"string\",\n      \"description\": \"Dun and Bradstreet DUNS number for the organization\",\n      \"pattern\": \"^[0-9]{9}$\"\n    },\n    \"Number of Employees\": {\n      \"type\": \"integer\",\n      \"description\": \"Approximate number of employees in the organization\",\n      \"minimum\": 0\n    },\n    \"Annual Revenue\": {\n      \"type\": \"number\",\n      \"description\": \"Estimated annual revenue of the organization\",\n      \"minimum\": 0\n    },\n    \"Currency Code\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code for monetary values\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"Address\": {\n      \"$ref\": \"#/$defs/Address\"\
  \n    }\n  },\n  \"$defs\": {\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"Physical address associated with the account\",\n      \"properties\": {\n        \"Street Address\": {\n          \"type\": \"string\",\n          \"description\": \"Street address line\"\n        },\n        \"Street Address 2\": {\n          \"type\": \"string\",\n          \"description\": \"Secondary address line\"\n        },\n        \"City\": {\n          \"type\": \"string\",\n          \"description\": \"City name\"\n        },\n        \"State\": {\n          \"type\": \"string\",\n          \"description\": \"State or province\"\n        },\n        \"Postal Code\": {\n          \"type\": \"string\",\n          \"description\": \"Postal or ZIP code\"\n        },\n        \"Country\": {\n          \"type\": \"string\",\n          \"description\": \"Country name\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/json-schema/oracle-siebel-account-schema.json
tags:
- CRM
- Customer Management
- Enterprise Software
- Marketing Automation
- Oracle
- Sales Automation
- Service Automation
title: Oracle Siebel CRM Account
---
