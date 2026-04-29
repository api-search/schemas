---
description: A Customer represents a consumer of the service or product that the business offers. Customers can be organized as sub-customers (jobs) within a parent customer hierarchy.
layout: schema
name: Customer
properties_list:
- description: Unique identifier for the customer
  name: Id
  type: string
- description: Version number for optimistic locking
  name: SyncToken
  type: string
- description: Title of the person (e.g., Mr., Mrs., Ms.)
  name: Title
  type: string
- description: Given (first) name of the customer
  name: GivenName
  type: string
- description: Middle name of the customer
  name: MiddleName
  type: string
- description: Family (last) name of the customer
  name: FamilyName
  type: string
- description: Suffix of the person (e.g., Jr., Sr., III)
  name: Suffix
  type: string
- description: The name displayed to identify the customer. Must be unique across Customer, Employee, and Vendor objects.
  name: DisplayName
  type: string
- description: The name of the company associated with the customer
  name: CompanyName
  type: string
- description: Name of the customer as printed on a check
  name: PrintOnCheckName
  type: string
- description: Whether the customer is currently active
  name: Active
  type: boolean
- description: Whether the customer is taxable
  name: Taxable
  type: boolean
- description: Free-form text about the customer
  name: Notes
  type: string
- description: Whether this customer is a sub-customer (job)
  name: Job
  type: boolean
- description: Depth level in the customer hierarchy (0 = top)
  name: Level
  type: integer
- description: Fully qualified name of the entity, including parent names separated by colons
  name: FullyQualifiedName
  type: string
- description: Preferred delivery method for communications
  name: PreferredDeliveryMethod
  type: string
- description: Open balance amount for the customer
  name: Balance
  type: number
- description: Open balance amount including balances of sub-customers (jobs)
  name: BalanceWithJobs
  type: number
- description: Tax exemption reason ID
  name: TaxExemptionReasonId
  type: string
- description: ''
  name: WebAddr
  type: object
- description: ''
  name: domain
  type: string
- description: ''
  name: sparse
  type: boolean
provider_name: Intuit
provider_slug: intuit
schema_file: json-schema/quickbooks-accounting-customer-schema.json
slug: quickbooks-accounting-customer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Customer\",\n  \"type\": \"object\",\n  \"description\": \"A Customer represents a consumer of the service or product that the business offers. Customers can be organized as sub-customers (jobs) within a parent customer hierarchy.\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the customer\"\n    },\n    \"SyncToken\": {\n      \"type\": \"string\",\n      \"description\": \"Version number for optimistic locking\"\n    },\n    \"Title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the person (e.g., Mr., Mrs., Ms.)\"\n    },\n    \"GivenName\": {\n      \"type\": \"string\",\n      \"description\": \"Given (first) name of the customer\"\n    },\n    \"MiddleName\": {\n      \"type\": \"string\",\n      \"description\": \"Middle name of the customer\"\n    },\n    \"FamilyName\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Family (last) name of the customer\"\n    },\n    \"Suffix\": {\n      \"type\": \"string\",\n      \"description\": \"Suffix of the person (e.g., Jr., Sr., III)\"\n    },\n    \"DisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"The name displayed to identify the customer. Must be unique across Customer, Employee, and Vendor objects.\"\n    },\n    \"CompanyName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the company associated with the customer\"\n    },\n    \"PrintOnCheckName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the customer as printed on a check\"\n    },\n    \"Active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the customer is currently active\"\n    },\n    \"Taxable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the customer is taxable\"\n    },\n    \"Notes\": {\n      \"type\": \"string\",\n      \"description\": \"Free-form\
  \ text about the customer\"\n    },\n    \"Job\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this customer is a sub-customer (job)\"\n    },\n    \"Level\": {\n      \"type\": \"integer\",\n      \"description\": \"Depth level in the customer hierarchy (0 = top)\"\n    },\n    \"FullyQualifiedName\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified name of the entity, including parent names separated by colons\"\n    },\n    \"PreferredDeliveryMethod\": {\n      \"type\": \"string\",\n      \"description\": \"Preferred delivery method for communications\"\n    },\n    \"Balance\": {\n      \"type\": \"number\",\n      \"description\": \"Open balance amount for the customer\"\n    },\n    \"BalanceWithJobs\": {\n      \"type\": \"number\",\n      \"description\": \"Open balance amount including balances of sub-customers (jobs)\"\n    },\n    \"TaxExemptionReasonId\": {\n      \"type\": \"string\",\n      \"description\": \"Tax exemption reason\
  \ ID\"\n    },\n    \"WebAddr\": {\n      \"type\": \"object\"\n    },\n    \"domain\": {\n      \"type\": \"string\"\n    },\n    \"sparse\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/json-schema/quickbooks-accounting-customer-schema.json
tags:
- Accounting
- Custom Fields
- Financial
- Financial Services
- Invoicing
- Payments
- Payroll
- Project Management
- Sales Tax
- Small Business
- Tax
- Tax Preparation
- Taxes
- Time Tracking
title: Customer
---
