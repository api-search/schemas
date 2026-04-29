---
description: Business that represents a customer or potential customer. The company that is billed in business transactions. Corresponds to the account entity type in the Microsoft.Dynamics.CRM namespace.
layout: schema
name: Account
properties_list:
- description: Unique identifier of the account.
  name: accountid
  type: string
- description: Company or business name of the account.
  name: name
  type: string
- description: ID number or code for the account to quickly search and identify the account in system views.
  name: accountnumber
  type: string
- description: Category indicating whether the customer account is standard or preferred. 1 = Preferred Customer, 2 = Standard.
  name: accountcategorycode
  type: integer
- description: Classification code indicating the potential value of the customer account. 1 = Default Value.
  name: accountclassificationcode
  type: integer
- description: Rating indicating the value of the customer account.
  name: accountratingcode
  type: integer
- description: Additional information describing the account.
  name: description
  type: string
- description: Primary email address for the account.
  name: emailaddress1
  type: string
- description: Secondary email address for the account.
  name: emailaddress2
  type: string
- description: Alternate email address for the account.
  name: emailaddress3
  type: string
- description: Main phone number for the account.
  name: telephone1
  type: string
- description: Second phone number for the account.
  name: telephone2
  type: string
- description: Third phone number for the account.
  name: telephone3
  type: string
- description: Fax number for the account.
  name: fax
  type: string
- description: Website URL for the account.
  name: websiteurl
  type: string
- description: Primary industry of the account for marketing segmentation. Values include 1=Accounting, 2=Agriculture, 3=Broadcasting, 4=Brokers, 5=Building Supply, 6=Business Services, 7=Consulting, 8=Consumer Serv
  name: industrycode
  type: integer
- description: Number of employees at the account.
  name: numberofemployees
  type: integer
- description: Annual revenue for the account.
  name: revenue
  type: number
- description: Annual revenue converted to the system default base currency.
  name: revenue_base
  type: number
- description: Ownership structure of the account. 1 = Public, 2 = Private, 3 = Subsidiary, 4 = Other.
  name: ownershipcode
  type: integer
- description: Category describing the relationship between the account and the organization. 1=Competitor, 2=Consultant, 3=Customer, 4=Investor, 5=Partner, 6=Influencer, 7=Press, 8=Prospect, 9=Reseller, 10=Supplier
  name: customertypecode
  type: integer
- description: Legal designation or other business type of the account.
  name: businesstypecode
  type: integer
- description: Standard Industrial Classification (SIC) code.
  name: sic
  type: string
- description: Stock exchange symbol for the account.
  name: tickersymbol
  type: string
- description: Stock exchange at which the account is listed.
  name: stockexchange
  type: string
- description: Number of shares available to the public.
  name: sharesoutstanding
  type: integer
- description: Market capitalization of the account.
  name: marketcap
  type: number
- description: Credit limit of the account.
  name: creditlimit
  type: number
- description: Whether the credit for the account is on hold.
  name: creditonhold
  type: boolean
- description: Payment terms for the account. 1 = Net 30, 2 = 2% 10 Net 30, 3 = Net 45, 4 = Net 60.
  name: paymenttermscode
  type: integer
- description: Preferred method of contact. 1 = Any, 2 = Email, 3 = Phone, 4 = Fax, 5 = Mail.
  name: preferredcontactmethodcode
  type: integer
- description: Whether the account allows direct email.
  name: donotemail
  type: boolean
- description: Whether the account allows phone calls.
  name: donotphone
  type: boolean
- description: Whether the account allows faxes.
  name: donotfax
  type: boolean
- description: Whether the account allows direct mail.
  name: donotpostalmail
  type: boolean
- description: Whether the account allows bulk email through campaigns.
  name: donotbulkemail
  type: boolean
- description: Whether the account accepts marketing materials.
  name: donotsendmm
  type: boolean
- description: Descriptive name for the primary address.
  name: address1_name
  type: string
- description: First line of the primary address.
  name: address1_line1
  type: string
- description: Second line of the primary address.
  name: address1_line2
  type: string
- description: Third line of the primary address.
  name: address1_line3
  type: string
- description: City for the primary address.
  name: address1_city
  type: string
- description: State or province for the primary address.
  name: address1_stateorprovince
  type: string
- description: ZIP code or postal code for the primary address.
  name: address1_postalcode
  type: string
- description: Country or region for the primary address.
  name: address1_country
  type: string
- description: County for the primary address.
  name: address1_county
  type: string
- description: Main phone number for the primary address.
  name: address1_telephone1
  type: string
- description: Fax number for the primary address.
  name: address1_fax
  type: string
- description: Latitude value for the primary address.
  name: address1_latitude
  type: number
- description: Longitude value for the primary address.
  name: address1_longitude
  type: number
- description: Primary address type. 1 = Bill To, 2 = Ship To, 3 = Primary, 4 = Other.
  name: address1_addresstypecode
  type: integer
- description: Descriptive name for the secondary address.
  name: address2_name
  type: string
- description: First line of the secondary address.
  name: address2_line1
  type: string
- description: Second line of the secondary address.
  name: address2_line2
  type: string
- description: Third line of the secondary address.
  name: address2_line3
  type: string
- description: City for the secondary address.
  name: address2_city
  type: string
- description: State or province for the secondary address.
  name: address2_stateorprovince
  type: string
- description: ZIP code or postal code for the secondary address.
  name: address2_postalcode
  type: string
- description: Country or region for the secondary address.
  name: address2_country
  type: string
- description: Status of the account. 0 = Active, 1 = Inactive. Inactive accounts are read-only.
  name: statecode
  type: integer
- description: Status reason for the account. 1 = Active, 2 = Inactive.
  name: statuscode
  type: integer
- description: Date and time when the account record was created.
  name: createdon
  type: string
- description: Date and time when the account record was last updated.
  name: modifiedon
  type: string
- description: Version number of the account record.
  name: versionnumber
  type: integer
- description: Lookup property for the primary contact of the account.
  name: _primarycontactid_value
  type: string
- description: Lookup property for the parent account.
  name: _parentaccountid_value
  type: string
- description: Lookup property for the user or team assigned to manage the record.
  name: _ownerid_value
  type: string
- description: Lookup property for the currency associated with the record.
  name: _transactioncurrencyid_value
  type: string
- description: Phonetic spelling of the company name for Japanese pronunciation.
  name: yominame
  type: string
provider_name: Microsoft Power Apps
provider_slug: microsoft-power-apps
schema_file: json-schema/microsoft-power-apps-dataverse-web-account-schema.json
slug: microsoft-power-apps-dataverse-web-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Account\",\n  \"type\": \"object\",\n  \"description\": \"Business that represents a customer or potential customer. The company that is billed in business transactions. Corresponds to the account entity type in the Microsoft.Dynamics.CRM namespace.\",\n  \"properties\": {\n    \"accountid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the account.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Company or business name of the account.\"\n    },\n    \"accountnumber\": {\n      \"type\": \"string\",\n      \"description\": \"ID number or code for the account to quickly search and identify the account in system views.\"\n    },\n    \"accountcategorycode\": {\n      \"type\": \"integer\",\n      \"description\": \"Category indicating whether the customer account is standard or preferred. 1 = Preferred Customer, 2 = Standard.\"\
  \n    },\n    \"accountclassificationcode\": {\n      \"type\": \"integer\",\n      \"description\": \"Classification code indicating the potential value of the customer account. 1 = Default Value.\"\n    },\n    \"accountratingcode\": {\n      \"type\": \"integer\",\n      \"description\": \"Rating indicating the value of the customer account.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Additional information describing the account.\"\n    },\n    \"emailaddress1\": {\n      \"type\": \"string\",\n      \"description\": \"Primary email address for the account.\"\n    },\n    \"emailaddress2\": {\n      \"type\": \"string\",\n      \"description\": \"Secondary email address for the account.\"\n    },\n    \"emailaddress3\": {\n      \"type\": \"string\",\n      \"description\": \"Alternate email address for the account.\"\n    },\n    \"telephone1\": {\n      \"type\": \"string\",\n      \"description\": \"Main phone number for the account.\"\
  \n    },\n    \"telephone2\": {\n      \"type\": \"string\",\n      \"description\": \"Second phone number for the account.\"\n    },\n    \"telephone3\": {\n      \"type\": \"string\",\n      \"description\": \"Third phone number for the account.\"\n    },\n    \"fax\": {\n      \"type\": \"string\",\n      \"description\": \"Fax number for the account.\"\n    },\n    \"websiteurl\": {\n      \"type\": \"string\",\n      \"description\": \"Website URL for the account.\"\n    },\n    \"industrycode\": {\n      \"type\": \"integer\",\n      \"description\": \"Primary industry of the account for marketing segmentation. Values include 1=Accounting, 2=Agriculture, 3=Broadcasting, 4=Brokers, 5=Building Supply, 6=Business Services, 7=Consulting, 8=Consumer Services, and others up to 33=Wholesale.\"\n    },\n    \"numberofemployees\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of employees at the account.\"\n    },\n    \"revenue\": {\n      \"type\": \"number\",\n     \
  \ \"description\": \"Annual revenue for the account.\"\n    },\n    \"revenue_base\": {\n      \"type\": \"number\",\n      \"description\": \"Annual revenue converted to the system default base currency.\"\n    },\n    \"ownershipcode\": {\n      \"type\": \"integer\",\n      \"description\": \"Ownership structure of the account. 1 = Public, 2 = Private, 3 = Subsidiary, 4 = Other.\"\n    },\n    \"customertypecode\": {\n      \"type\": \"integer\",\n      \"description\": \"Category describing the relationship between the account and the organization. 1=Competitor, 2=Consultant, 3=Customer, 4=Investor, 5=Partner, 6=Influencer, 7=Press, 8=Prospect, 9=Reseller, 10=Supplier, 11=Vendor, 12=Other.\"\n    },\n    \"businesstypecode\": {\n      \"type\": \"integer\",\n      \"description\": \"Legal designation or other business type of the account.\"\n    },\n    \"sic\": {\n      \"type\": \"string\",\n      \"description\": \"Standard Industrial Classification (SIC) code.\"\n    },\n    \"\
  tickersymbol\": {\n      \"type\": \"string\",\n      \"description\": \"Stock exchange symbol for the account.\"\n    },\n    \"stockexchange\": {\n      \"type\": \"string\",\n      \"description\": \"Stock exchange at which the account is listed.\"\n    },\n    \"sharesoutstanding\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of shares available to the public.\"\n    },\n    \"marketcap\": {\n      \"type\": \"number\",\n      \"description\": \"Market capitalization of the account.\"\n    },\n    \"creditlimit\": {\n      \"type\": \"number\",\n      \"description\": \"Credit limit of the account.\"\n    },\n    \"creditonhold\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the credit for the account is on hold.\"\n    },\n    \"paymenttermscode\": {\n      \"type\": \"integer\",\n      \"description\": \"Payment terms for the account. 1 = Net 30, 2 = 2% 10 Net 30, 3 = Net 45, 4 = Net 60.\"\n    },\n    \"preferredcontactmethodcode\": {\n\
  \      \"type\": \"integer\",\n      \"description\": \"Preferred method of contact. 1 = Any, 2 = Email, 3 = Phone, 4 = Fax, 5 = Mail.\"\n    },\n    \"donotemail\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account allows direct email.\"\n    },\n    \"donotphone\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account allows phone calls.\"\n    },\n    \"donotfax\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account allows faxes.\"\n    },\n    \"donotpostalmail\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account allows direct mail.\"\n    },\n    \"donotbulkemail\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account allows bulk email through campaigns.\"\n    },\n    \"donotsendmm\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account accepts marketing materials.\"\n    },\n    \"address1_name\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Descriptive name for the primary address.\"\n    },\n    \"address1_line1\": {\n      \"type\": \"string\",\n      \"description\": \"First line of the primary address.\"\n    },\n    \"address1_line2\": {\n      \"type\": \"string\",\n      \"description\": \"Second line of the primary address.\"\n    },\n    \"address1_line3\": {\n      \"type\": \"string\",\n      \"description\": \"Third line of the primary address.\"\n    },\n    \"address1_city\": {\n      \"type\": \"string\",\n      \"description\": \"City for the primary address.\"\n    },\n    \"address1_stateorprovince\": {\n      \"type\": \"string\",\n      \"description\": \"State or province for the primary address.\"\n    },\n    \"address1_postalcode\": {\n      \"type\": \"string\",\n      \"description\": \"ZIP code or postal code for the primary address.\"\n    },\n    \"address1_country\": {\n      \"type\": \"string\",\n      \"description\": \"Country or region for the primary address.\"\
  \n    },\n    \"address1_county\": {\n      \"type\": \"string\",\n      \"description\": \"County for the primary address.\"\n    },\n    \"address1_telephone1\": {\n      \"type\": \"string\",\n      \"description\": \"Main phone number for the primary address.\"\n    },\n    \"address1_fax\": {\n      \"type\": \"string\",\n      \"description\": \"Fax number for the primary address.\"\n    },\n    \"address1_latitude\": {\n      \"type\": \"number\",\n      \"description\": \"Latitude value for the primary address.\"\n    },\n    \"address1_longitude\": {\n      \"type\": \"number\",\n      \"description\": \"Longitude value for the primary address.\"\n    },\n    \"address1_addresstypecode\": {\n      \"type\": \"integer\",\n      \"description\": \"Primary address type. 1 = Bill To, 2 = Ship To, 3 = Primary, 4 = Other.\"\n    },\n    \"address2_name\": {\n      \"type\": \"string\",\n      \"description\": \"Descriptive name for the secondary address.\"\n    },\n    \"address2_line1\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"First line of the secondary address.\"\n    },\n    \"address2_line2\": {\n      \"type\": \"string\",\n      \"description\": \"Second line of the secondary address.\"\n    },\n    \"address2_line3\": {\n      \"type\": \"string\",\n      \"description\": \"Third line of the secondary address.\"\n    },\n    \"address2_city\": {\n      \"type\": \"string\",\n      \"description\": \"City for the secondary address.\"\n    },\n    \"address2_stateorprovince\": {\n      \"type\": \"string\",\n      \"description\": \"State or province for the secondary address.\"\n    },\n    \"address2_postalcode\": {\n      \"type\": \"string\",\n      \"description\": \"ZIP code or postal code for the secondary address.\"\n    },\n    \"address2_country\": {\n      \"type\": \"string\",\n      \"description\": \"Country or region for the secondary address.\"\n    },\n    \"statecode\": {\n      \"type\": \"integer\",\n      \"description\": \"\
  Status of the account. 0 = Active, 1 = Inactive. Inactive accounts are read-only.\"\n    },\n    \"statuscode\": {\n      \"type\": \"integer\",\n      \"description\": \"Status reason for the account. 1 = Active, 2 = Inactive.\"\n    },\n    \"createdon\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the account record was created.\"\n    },\n    \"modifiedon\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the account record was last updated.\"\n    },\n    \"versionnumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Version number of the account record.\"\n    },\n    \"_primarycontactid_value\": {\n      \"type\": \"string\",\n      \"description\": \"Lookup property for the primary contact of the account.\"\n    },\n    \"_parentaccountid_value\": {\n      \"type\": \"string\",\n      \"description\": \"Lookup property for the parent account.\"\n    },\n    \"_ownerid_value\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Lookup property for the user or team assigned to manage the record.\"\n    },\n    \"_transactioncurrencyid_value\": {\n      \"type\": \"string\",\n      \"description\": \"Lookup property for the currency associated with the record.\"\n    },\n    \"yominame\": {\n      \"type\": \"string\",\n      \"description\": \"Phonetic spelling of the company name for Japanese pronunciation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-apps/refs/heads/main/json-schema/microsoft-power-apps-dataverse-web-account-schema.json
tags:
- Business Applications
- Cloud
- Enterprise
- Low-Code
- Microsoft
- No-Code
- Power Platform
- SaaS
title: Account
---
