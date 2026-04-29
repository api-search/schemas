---
description: A Customer represents a consumer of the service or product that the business offers. The Customer entity supports a hierarchy where customers can have sub-customers (jobs) organized under a parent customer. DisplayName must be unique across all Customer, Employee, and Vendor objects within a QuickBooks Online company.
layout: schema
name: QuickBooks Online Customer
properties_list:
- description: Unique identifier for the customer, assigned by QuickBooks Online.
  name: Id
  type: string
- description: Version number of the entity used for optimistic concurrency control. Required for update operations.
  name: SyncToken
  type: string
- description: ''
  name: MetaData
  type: object
- description: Title of the person (e.g., Mr., Mrs., Ms., Dr.).
  name: Title
  type: string
- description: Given (first) name of the customer.
  name: GivenName
  type: string
- description: Middle name of the customer.
  name: MiddleName
  type: string
- description: Family (last) name of the customer.
  name: FamilyName
  type: string
- description: Suffix of the person (e.g., Jr., Sr., III).
  name: Suffix
  type: string
- description: The name displayed to identify the customer in the QuickBooks UI and on transaction forms. Must be unique across all Customer, Employee, and Vendor objects.
  name: DisplayName
  type: string
- description: The company name associated with the customer.
  name: CompanyName
  type: string
- description: Name to print on checks issued to this customer.
  name: PrintOnCheckName
  type: string
- description: Whether the customer is currently active. Inactive customers do not appear in transaction drop-downs but their data is retained.
  name: Active
  type: boolean
- description: Whether transactions for this customer are taxable.
  name: Taxable
  type: boolean
- description: Primary email address for the customer.
  name: PrimaryEmailAddr
  type: object
- description: Primary phone number.
  name: PrimaryPhone
  type: object
- description: Mobile phone number.
  name: Mobile
  type: object
- description: Fax number.
  name: Fax
  type: object
- description: Alternate phone number.
  name: AlternatePhone
  type: object
- description: Default billing address for the customer.
  name: BillAddr
  type: object
- description: Default shipping address for the customer.
  name: ShipAddr
  type: object
- description: Free-form text notes about the customer.
  name: Notes
  type: string
- description: Whether this customer represents a job (sub-customer) rather than a top-level customer.
  name: Job
  type: boolean
- description: Reference to the parent customer if this is a sub-customer (job).
  name: ParentRef
  type: object
- description: Depth level in the customer hierarchy. 0 indicates a top-level customer.
  name: Level
  type: integer
- description: Fully qualified name of the customer including all parent names separated by colons (e.g., 'ParentCustomer:SubCustomer').
  name: FullyQualifiedName
  type: string
- description: Reference to the currency used by this customer. Only applicable for companies with multicurrency enabled.
  name: CurrencyRef
  type: object
- description: Preferred method for delivering communications to this customer.
  name: PreferredDeliveryMethod
  type: string
- description: Open balance amount for the customer (sum of all open invoices minus payments).
  name: Balance
  type: number
- description: Open balance amount including balances of all sub-customers (jobs).
  name: BalanceWithJobs
  type: number
- description: Default sales terms for transactions with this customer.
  name: SalesTermRef
  type: object
- description: Default payment method for this customer.
  name: PaymentMethodRef
  type: object
- description: The tax exemption reason identifier if the customer is tax-exempt.
  name: TaxExemptionReasonId
  type: string
- description: The customer's website address.
  name: WebAddr
  type: object
- description: Whether this customer is a project (QuickBooks Online Plus and Advanced only).
  name: IsProject
  type: boolean
- description: Source of the customer record.
  name: Source
  type: string
- description: Primary tax identifier for the customer (e.g., ABN in Australia, GSTIN in India).
  name: PrimaryTaxIdentifier
  type: string
- description: GST registration type (applicable for India and Australia editions).
  name: GSTRegistrationType
  type: string
- description: Business number of the customer (used in certain international editions).
  name: BusinessNumber
  type: string
- description: GST Identification Number (India edition).
  name: GSTIN
  type: string
- description: Domain of the entity (e.g., QBO).
  name: domain
  type: string
- description: Indicates whether this is a sparse (partial) representation of the entity.
  name: sparse
  type: boolean
provider_name: Intuit
provider_slug: intuit
schema_file: json-schema/intuit-customer-schema.json
slug: intuit-customer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/intuit/json-schema/intuit-customer-schema.json\",\n  \"title\": \"QuickBooks Online Customer\",\n  \"description\": \"A Customer represents a consumer of the service or product that the business offers. The Customer entity supports a hierarchy where customers can have sub-customers (jobs) organized under a parent customer. DisplayName must be unique across all Customer, Employee, and Vendor objects within a QuickBooks Online company.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the customer, assigned by QuickBooks Online.\",\n      \"readOnly\": true\n    },\n    \"SyncToken\": {\n      \"type\": \"string\",\n      \"description\": \"Version number of the entity used for optimistic concurrency control. Required for update operations.\"\n    },\n    \"MetaData\": {\n\
  \      \"$ref\": \"#/$defs/MetaData\"\n    },\n    \"Title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the person (e.g., Mr., Mrs., Ms., Dr.).\",\n      \"maxLength\": 16\n    },\n    \"GivenName\": {\n      \"type\": \"string\",\n      \"description\": \"Given (first) name of the customer.\",\n      \"maxLength\": 100\n    },\n    \"MiddleName\": {\n      \"type\": \"string\",\n      \"description\": \"Middle name of the customer.\",\n      \"maxLength\": 100\n    },\n    \"FamilyName\": {\n      \"type\": \"string\",\n      \"description\": \"Family (last) name of the customer.\",\n      \"maxLength\": 100\n    },\n    \"Suffix\": {\n      \"type\": \"string\",\n      \"description\": \"Suffix of the person (e.g., Jr., Sr., III).\",\n      \"maxLength\": 16\n    },\n    \"DisplayName\": {\n      \"type\": \"string\",\n      \"description\": \"The name displayed to identify the customer in the QuickBooks UI and on transaction forms. Must be unique across all Customer,\
  \ Employee, and Vendor objects.\",\n      \"maxLength\": 500\n    },\n    \"CompanyName\": {\n      \"type\": \"string\",\n      \"description\": \"The company name associated with the customer.\",\n      \"maxLength\": 500\n    },\n    \"PrintOnCheckName\": {\n      \"type\": \"string\",\n      \"description\": \"Name to print on checks issued to this customer.\",\n      \"maxLength\": 110\n    },\n    \"Active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the customer is currently active. Inactive customers do not appear in transaction drop-downs but their data is retained.\",\n      \"default\": true\n    },\n    \"Taxable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether transactions for this customer are taxable.\"\n    },\n    \"PrimaryEmailAddr\": {\n      \"$ref\": \"#/$defs/EmailAddress\",\n      \"description\": \"Primary email address for the customer.\"\n    },\n    \"PrimaryPhone\": {\n      \"$ref\": \"#/$defs/TelephoneNumber\",\n\
  \      \"description\": \"Primary phone number.\"\n    },\n    \"Mobile\": {\n      \"$ref\": \"#/$defs/TelephoneNumber\",\n      \"description\": \"Mobile phone number.\"\n    },\n    \"Fax\": {\n      \"$ref\": \"#/$defs/TelephoneNumber\",\n      \"description\": \"Fax number.\"\n    },\n    \"AlternatePhone\": {\n      \"$ref\": \"#/$defs/TelephoneNumber\",\n      \"description\": \"Alternate phone number.\"\n    },\n    \"BillAddr\": {\n      \"$ref\": \"#/$defs/PhysicalAddress\",\n      \"description\": \"Default billing address for the customer.\"\n    },\n    \"ShipAddr\": {\n      \"$ref\": \"#/$defs/PhysicalAddress\",\n      \"description\": \"Default shipping address for the customer.\"\n    },\n    \"Notes\": {\n      \"type\": \"string\",\n      \"description\": \"Free-form text notes about the customer.\",\n      \"maxLength\": 2000\n    },\n    \"Job\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this customer represents a job (sub-customer) rather than\
  \ a top-level customer.\"\n    },\n    \"ParentRef\": {\n      \"$ref\": \"#/$defs/ReferenceType\",\n      \"description\": \"Reference to the parent customer if this is a sub-customer (job).\"\n    },\n    \"Level\": {\n      \"type\": \"integer\",\n      \"description\": \"Depth level in the customer hierarchy. 0 indicates a top-level customer.\",\n      \"readOnly\": true,\n      \"minimum\": 0\n    },\n    \"FullyQualifiedName\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified name of the customer including all parent names separated by colons (e.g., 'ParentCustomer:SubCustomer').\",\n      \"readOnly\": true\n    },\n    \"CurrencyRef\": {\n      \"$ref\": \"#/$defs/ReferenceType\",\n      \"description\": \"Reference to the currency used by this customer. Only applicable for companies with multicurrency enabled.\"\n    },\n    \"PreferredDeliveryMethod\": {\n      \"type\": \"string\",\n      \"description\": \"Preferred method for delivering communications\
  \ to this customer.\",\n      \"enum\": [\"Print\", \"Email\", \"None\"]\n    },\n    \"Balance\": {\n      \"type\": \"number\",\n      \"description\": \"Open balance amount for the customer (sum of all open invoices minus payments).\",\n      \"readOnly\": true\n    },\n    \"BalanceWithJobs\": {\n      \"type\": \"number\",\n      \"description\": \"Open balance amount including balances of all sub-customers (jobs).\",\n      \"readOnly\": true\n    },\n    \"SalesTermRef\": {\n      \"$ref\": \"#/$defs/ReferenceType\",\n      \"description\": \"Default sales terms for transactions with this customer.\"\n    },\n    \"PaymentMethodRef\": {\n      \"$ref\": \"#/$defs/ReferenceType\",\n      \"description\": \"Default payment method for this customer.\"\n    },\n    \"TaxExemptionReasonId\": {\n      \"type\": \"string\",\n      \"description\": \"The tax exemption reason identifier if the customer is tax-exempt.\"\n    },\n    \"WebAddr\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"The customer's website address.\",\n      \"properties\": {\n        \"URI\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The website URL.\"\n        }\n      }\n    },\n    \"IsProject\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this customer is a project (QuickBooks Online Plus and Advanced only).\",\n      \"readOnly\": true\n    },\n    \"Source\": {\n      \"type\": \"string\",\n      \"description\": \"Source of the customer record.\",\n      \"readOnly\": true\n    },\n    \"PrimaryTaxIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"Primary tax identifier for the customer (e.g., ABN in Australia, GSTIN in India).\"\n    },\n    \"GSTRegistrationType\": {\n      \"type\": \"string\",\n      \"description\": \"GST registration type (applicable for India and Australia editions).\",\n      \"enum\": [\n        \"GST_REG_REG\",\n        \"GST_REG_COMP\",\n        \"GST_UNREG\",\n \
  \       \"CONSUMER\",\n        \"OVERSEAS\",\n        \"SEZ\",\n        \"DEEMED\"\n      ]\n    },\n    \"BusinessNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Business number of the customer (used in certain international editions).\"\n    },\n    \"GSTIN\": {\n      \"type\": \"string\",\n      \"description\": \"GST Identification Number (India edition).\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Domain of the entity (e.g., QBO).\",\n      \"readOnly\": true\n    },\n    \"sparse\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether this is a sparse (partial) representation of the entity.\"\n    }\n  },\n  \"required\": [\"DisplayName\"],\n  \"$defs\": {\n    \"ReferenceType\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to another entity in QuickBooks Online.\",\n      \"properties\": {\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"\
  The unique identifier of the referenced entity.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"An identifying name for the referenced entity.\"\n        }\n      },\n      \"required\": [\"value\"]\n    },\n    \"PhysicalAddress\": {\n      \"type\": \"object\",\n      \"description\": \"A physical (mailing) address.\",\n      \"properties\": {\n        \"Id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the address.\"\n        },\n        \"Line1\": {\n          \"type\": \"string\",\n          \"description\": \"First line of the street address.\",\n          \"maxLength\": 500\n        },\n        \"Line2\": {\n          \"type\": \"string\",\n          \"description\": \"Second line of the street address.\",\n          \"maxLength\": 500\n        },\n        \"Line3\": {\n          \"type\": \"string\",\n          \"description\": \"Third line of the street address.\",\n          \"maxLength\"\
  : 500\n        },\n        \"Line4\": {\n          \"type\": \"string\",\n          \"description\": \"Fourth line of the street address.\",\n          \"maxLength\": 500\n        },\n        \"Line5\": {\n          \"type\": \"string\",\n          \"description\": \"Fifth line of the street address.\",\n          \"maxLength\": 500\n        },\n        \"City\": {\n          \"type\": \"string\",\n          \"description\": \"City name.\",\n          \"maxLength\": 255\n        },\n        \"CountrySubDivisionCode\": {\n          \"type\": \"string\",\n          \"description\": \"Region within a country (e.g., state, province).\",\n          \"maxLength\": 255\n        },\n        \"PostalCode\": {\n          \"type\": \"string\",\n          \"description\": \"Postal code.\",\n          \"maxLength\": 30\n        },\n        \"Country\": {\n          \"type\": \"string\",\n          \"description\": \"Country name or code.\",\n          \"maxLength\": 255\n        },\n        \"Lat\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Latitude coordinate.\"\n        },\n        \"Long\": {\n          \"type\": \"string\",\n          \"description\": \"Longitude coordinate.\"\n        }\n      }\n    },\n    \"EmailAddress\": {\n      \"type\": \"object\",\n      \"description\": \"An email address.\",\n      \"properties\": {\n        \"Address\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The email address.\",\n          \"maxLength\": 100\n        }\n      }\n    },\n    \"TelephoneNumber\": {\n      \"type\": \"object\",\n      \"description\": \"A telephone number.\",\n      \"properties\": {\n        \"FreeFormNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Telephone number in free-form format.\",\n          \"maxLength\": 30\n        }\n      }\n    },\n    \"MetaData\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata about entity creation and modification\
  \ timestamps.\",\n      \"properties\": {\n        \"CreateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the entity was created.\"\n        },\n        \"LastUpdatedTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the entity was last updated.\"\n        }\n      }\n    }\n  },\n  \"examples\": [\n    {\n      \"DisplayName\": \"Amy's Bird Sanctuary\",\n      \"GivenName\": \"Amy\",\n      \"FamilyName\": \"Lauterbach\",\n      \"CompanyName\": \"Amy's Bird Sanctuary\",\n      \"PrimaryEmailAddr\": {\n        \"Address\": \"amy@birdsnest.example.com\"\n      },\n      \"PrimaryPhone\": {\n        \"FreeFormNumber\": \"(555) 555-1234\"\n      },\n      \"BillAddr\": {\n        \"Line1\": \"4581 Finch St.\",\n        \"City\": \"Bayshore\",\n        \"CountrySubDivisionCode\": \"CA\",\n        \"PostalCode\": \"94326\",\n        \"Country\"\
  : \"US\"\n      },\n      \"PreferredDeliveryMethod\": \"Email\",\n      \"Active\": true,\n      \"Taxable\": true\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/json-schema/intuit-customer-schema.json
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
title: QuickBooks Online Customer
---
