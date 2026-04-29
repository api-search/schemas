---
description: Person with whom a business unit has a relationship, such as a customer, supplier, or colleague. Corresponds to the contact entity type in the Microsoft.Dynamics.CRM namespace.
layout: schema
name: Contact
properties_list:
- description: Unique identifier of the contact.
  name: contactid
  type: string
- description: First name of the contact.
  name: firstname
  type: string
- description: Last name of the contact.
  name: lastname
  type: string
- description: Full name of the contact, combining first name, middle name, and last name.
  name: fullname
  type: string
- description: Middle name or initial of the contact.
  name: middlename
  type: string
- description: Nickname of the contact.
  name: nickname
  type: string
- description: Salutation for correspondence with the contact.
  name: salutation
  type: string
- description: Suffix used in the contact's name.
  name: suffix
  type: string
- description: Job title of the contact.
  name: jobtitle
  type: string
- description: Department or business unit where the contact works.
  name: department
  type: string
- description: Primary email address for the contact.
  name: emailaddress1
  type: string
- description: Secondary email address for the contact.
  name: emailaddress2
  type: string
- description: Alternate email address for the contact.
  name: emailaddress3
  type: string
- description: Main phone number for the contact.
  name: telephone1
  type: string
- description: Second phone number for the contact.
  name: telephone2
  type: string
- description: Third phone number for the contact.
  name: telephone3
  type: string
- description: Mobile phone number for the contact.
  name: mobilephone
  type: string
- description: Fax number for the contact.
  name: fax
  type: string
- description: Website URL for the contact.
  name: websiteurl
  type: string
- description: Additional information to describe the contact.
  name: description
  type: string
- description: Gender of the contact. 1 = Male, 2 = Female.
  name: gendercode
  type: integer
- description: Marital status of the contact. 1 = Single, 2 = Married, 3 = Divorced, 4 = Widowed.
  name: familystatuscode
  type: integer
- description: Birthday of the contact.
  name: birthdate
  type: string
- description: Anniversary date of the contact.
  name: anniversary
  type: string
- description: Name of the contact's spouse or partner.
  name: spousesname
  type: string
- description: Number of children the contact has.
  name: numberofchildren
  type: integer
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
- description: Preferred method of contact. 1 = Any, 2 = Email, 3 = Phone, 4 = Fax, 5 = Mail.
  name: preferredcontactmethodcode
  type: integer
- description: Whether the contact allows direct email.
  name: donotemail
  type: boolean
- description: Whether the contact allows phone calls.
  name: donotphone
  type: boolean
- description: Whether the contact allows faxes.
  name: donotfax
  type: boolean
- description: Whether the contact allows direct mail.
  name: donotpostalmail
  type: boolean
- description: Whether the contact allows bulk email through campaigns.
  name: donotbulkemail
  type: boolean
- description: Whether the contact accepts marketing materials.
  name: donotsendmm
  type: boolean
- description: Credit limit of the contact.
  name: creditlimit
  type: number
- description: Whether the credit for the contact is on hold.
  name: creditonhold
  type: boolean
- description: Status of the contact. 0 = Active, 1 = Inactive. Inactive contacts are read-only.
  name: statecode
  type: integer
- description: Status reason for the contact. 1 = Active, 2 = Inactive.
  name: statuscode
  type: integer
- description: Date and time when the contact record was created.
  name: createdon
  type: string
- description: Date and time when the contact record was last updated.
  name: modifiedon
  type: string
- description: Version number of the contact record.
  name: versionnumber
  type: integer
- description: Lookup property for the parent customer (account or contact) associated with this contact.
  name: _parentcustomerid_value
  type: string
- description: Lookup property for the user or team assigned to manage the record.
  name: _ownerid_value
  type: string
- description: Lookup property for the currency associated with the record.
  name: _transactioncurrencyid_value
  type: string
- description: Phonetic spelling of the first name (Japanese).
  name: yomifirstname
  type: string
- description: Phonetic spelling of the last name (Japanese).
  name: yomilastname
  type: string
- description: Phonetic spelling of the middle name (Japanese).
  name: yomimiddlename
  type: string
- description: Phonetic spelling of the full name (Japanese).
  name: yomifullname
  type: string
provider_name: Microsoft Power Apps
provider_slug: microsoft-power-apps
schema_file: json-schema/microsoft-power-apps-dataverse-web-contact-schema.json
slug: microsoft-power-apps-dataverse-web-contact
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Contact\",\n  \"type\": \"object\",\n  \"description\": \"Person with whom a business unit has a relationship, such as a customer, supplier, or colleague. Corresponds to the contact entity type in the Microsoft.Dynamics.CRM namespace.\",\n  \"properties\": {\n    \"contactid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the contact.\"\n    },\n    \"firstname\": {\n      \"type\": \"string\",\n      \"description\": \"First name of the contact.\"\n    },\n    \"lastname\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the contact.\"\n    },\n    \"fullname\": {\n      \"type\": \"string\",\n      \"description\": \"Full name of the contact, combining first name, middle name, and last name.\"\n    },\n    \"middlename\": {\n      \"type\": \"string\",\n      \"description\": \"Middle name or initial of the contact.\"\n    },\n    \"nickname\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Nickname of the contact.\"\n    },\n    \"salutation\": {\n      \"type\": \"string\",\n      \"description\": \"Salutation for correspondence with the contact.\"\n    },\n    \"suffix\": {\n      \"type\": \"string\",\n      \"description\": \"Suffix used in the contact's name.\"\n    },\n    \"jobtitle\": {\n      \"type\": \"string\",\n      \"description\": \"Job title of the contact.\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"Department or business unit where the contact works.\"\n    },\n    \"emailaddress1\": {\n      \"type\": \"string\",\n      \"description\": \"Primary email address for the contact.\"\n    },\n    \"emailaddress2\": {\n      \"type\": \"string\",\n      \"description\": \"Secondary email address for the contact.\"\n    },\n    \"emailaddress3\": {\n      \"type\": \"string\",\n      \"description\": \"Alternate email address for the contact.\"\n    },\n  \
  \  \"telephone1\": {\n      \"type\": \"string\",\n      \"description\": \"Main phone number for the contact.\"\n    },\n    \"telephone2\": {\n      \"type\": \"string\",\n      \"description\": \"Second phone number for the contact.\"\n    },\n    \"telephone3\": {\n      \"type\": \"string\",\n      \"description\": \"Third phone number for the contact.\"\n    },\n    \"mobilephone\": {\n      \"type\": \"string\",\n      \"description\": \"Mobile phone number for the contact.\"\n    },\n    \"fax\": {\n      \"type\": \"string\",\n      \"description\": \"Fax number for the contact.\"\n    },\n    \"websiteurl\": {\n      \"type\": \"string\",\n      \"description\": \"Website URL for the contact.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Additional information to describe the contact.\"\n    },\n    \"gendercode\": {\n      \"type\": \"integer\",\n      \"description\": \"Gender of the contact. 1 = Male, 2 = Female.\"\n    },\n    \"\
  familystatuscode\": {\n      \"type\": \"integer\",\n      \"description\": \"Marital status of the contact. 1 = Single, 2 = Married, 3 = Divorced, 4 = Widowed.\"\n    },\n    \"birthdate\": {\n      \"type\": \"string\",\n      \"description\": \"Birthday of the contact.\"\n    },\n    \"anniversary\": {\n      \"type\": \"string\",\n      \"description\": \"Anniversary date of the contact.\"\n    },\n    \"spousesname\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the contact's spouse or partner.\"\n    },\n    \"numberofchildren\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of children the contact has.\"\n    },\n    \"address1_name\": {\n      \"type\": \"string\",\n      \"description\": \"Descriptive name for the primary address.\"\n    },\n    \"address1_line1\": {\n      \"type\": \"string\",\n      \"description\": \"First line of the primary address.\"\n    },\n    \"address1_line2\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Second line of the primary address.\"\n    },\n    \"address1_line3\": {\n      \"type\": \"string\",\n      \"description\": \"Third line of the primary address.\"\n    },\n    \"address1_city\": {\n      \"type\": \"string\",\n      \"description\": \"City for the primary address.\"\n    },\n    \"address1_stateorprovince\": {\n      \"type\": \"string\",\n      \"description\": \"State or province for the primary address.\"\n    },\n    \"address1_postalcode\": {\n      \"type\": \"string\",\n      \"description\": \"ZIP code or postal code for the primary address.\"\n    },\n    \"address1_country\": {\n      \"type\": \"string\",\n      \"description\": \"Country or region for the primary address.\"\n    },\n    \"address1_county\": {\n      \"type\": \"string\",\n      \"description\": \"County for the primary address.\"\n    },\n    \"address1_telephone1\": {\n      \"type\": \"string\",\n      \"description\": \"Main phone number for the primary address.\"\n    },\n    \"address1_fax\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Fax number for the primary address.\"\n    },\n    \"address1_latitude\": {\n      \"type\": \"number\",\n      \"description\": \"Latitude value for the primary address.\"\n    },\n    \"address1_longitude\": {\n      \"type\": \"number\",\n      \"description\": \"Longitude value for the primary address.\"\n    },\n    \"address2_name\": {\n      \"type\": \"string\",\n      \"description\": \"Descriptive name for the secondary address.\"\n    },\n    \"address2_line1\": {\n      \"type\": \"string\",\n      \"description\": \"First line of the secondary address.\"\n    },\n    \"address2_line2\": {\n      \"type\": \"string\",\n      \"description\": \"Second line of the secondary address.\"\n    },\n    \"address2_line3\": {\n      \"type\": \"string\",\n      \"description\": \"Third line of the secondary address.\"\n    },\n    \"address2_city\": {\n      \"type\": \"string\",\n      \"description\": \"City for the secondary\
  \ address.\"\n    },\n    \"address2_stateorprovince\": {\n      \"type\": \"string\",\n      \"description\": \"State or province for the secondary address.\"\n    },\n    \"address2_postalcode\": {\n      \"type\": \"string\",\n      \"description\": \"ZIP code or postal code for the secondary address.\"\n    },\n    \"address2_country\": {\n      \"type\": \"string\",\n      \"description\": \"Country or region for the secondary address.\"\n    },\n    \"preferredcontactmethodcode\": {\n      \"type\": \"integer\",\n      \"description\": \"Preferred method of contact. 1 = Any, 2 = Email, 3 = Phone, 4 = Fax, 5 = Mail.\"\n    },\n    \"donotemail\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the contact allows direct email.\"\n    },\n    \"donotphone\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the contact allows phone calls.\"\n    },\n    \"donotfax\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the contact allows\
  \ faxes.\"\n    },\n    \"donotpostalmail\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the contact allows direct mail.\"\n    },\n    \"donotbulkemail\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the contact allows bulk email through campaigns.\"\n    },\n    \"donotsendmm\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the contact accepts marketing materials.\"\n    },\n    \"creditlimit\": {\n      \"type\": \"number\",\n      \"description\": \"Credit limit of the contact.\"\n    },\n    \"creditonhold\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the credit for the contact is on hold.\"\n    },\n    \"statecode\": {\n      \"type\": \"integer\",\n      \"description\": \"Status of the contact. 0 = Active, 1 = Inactive. Inactive contacts are read-only.\"\n    },\n    \"statuscode\": {\n      \"type\": \"integer\",\n      \"description\": \"Status reason for the contact. 1 = Active, 2 = Inactive.\"\
  \n    },\n    \"createdon\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the contact record was created.\"\n    },\n    \"modifiedon\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the contact record was last updated.\"\n    },\n    \"versionnumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Version number of the contact record.\"\n    },\n    \"_parentcustomerid_value\": {\n      \"type\": \"string\",\n      \"description\": \"Lookup property for the parent customer (account or contact) associated with this contact.\"\n    },\n    \"_ownerid_value\": {\n      \"type\": \"string\",\n      \"description\": \"Lookup property for the user or team assigned to manage the record.\"\n    },\n    \"_transactioncurrencyid_value\": {\n      \"type\": \"string\",\n      \"description\": \"Lookup property for the currency associated with the record.\"\n    },\n    \"yomifirstname\": {\n      \"type\": \"string\",\n   \
  \   \"description\": \"Phonetic spelling of the first name (Japanese).\"\n    },\n    \"yomilastname\": {\n      \"type\": \"string\",\n      \"description\": \"Phonetic spelling of the last name (Japanese).\"\n    },\n    \"yomimiddlename\": {\n      \"type\": \"string\",\n      \"description\": \"Phonetic spelling of the middle name (Japanese).\"\n    },\n    \"yomifullname\": {\n      \"type\": \"string\",\n      \"description\": \"Phonetic spelling of the full name (Japanese).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-power-apps/refs/heads/main/json-schema/microsoft-power-apps-dataverse-web-contact-schema.json
tags:
- Business Applications
- Cloud
- Enterprise
- Low-Code
- Microsoft
- No-Code
- Power Platform
- SaaS
title: Contact
---
