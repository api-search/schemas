---
description: Business that represents a customer or potential customer. The company that is billed in business transactions. Based on the Microsoft Dataverse account entity (Microsoft.Dynamics.CRM.account).
layout: schema
name: Microsoft Dynamics 365 Account
properties_list:
- description: Unique identifier of the account.
  name: accountid
  type: string
- description: The company or business name. This is the primary name column for the account entity.
  name: name
  type: string
- description: ID number or code for the account to quickly search and identify the account in system views.
  name: accountnumber
  type: string
- description: Additional information to describe the account, such as an excerpt from the company website.
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
- description: Main phone number for this account.
  name: telephone1
  type: string
- description: Second phone number for this account.
  name: telephone2
  type: string
- description: Third phone number for this account.
  name: telephone3
  type: string
- description: Fax number for the account.
  name: fax
  type: string
- description: Website URL for the account.
  name: websiteurl
  type: string
- description: Annual revenue for the account, used as an indicator in financial performance analysis.
  name: revenue
  type: number
- description: Annual revenue converted to the system default base currency.
  name: revenue_base
  type: number
- description: Number of employees that work at the account for use in marketing segmentation and demographic analysis.
  name: numberofemployees
  type: integer
- description: Standard Industrial Classification (SIC) code that indicates the account primary industry of business.
  name: sic
  type: string
- description: Stock exchange symbol for the account to track financial performance.
  name: tickersymbol
  type: string
- description: Stock exchange at which the account is listed.
  name: stockexchange
  type: string
- description: Primary industry for the account for use in marketing segmentation and demographic analysis.
  name: industrycode
  type: integer
- description: Ownership structure of the account.
  name: ownershipcode
  type: integer
- description: Category indicating whether the customer account is standard or preferred.
  name: accountcategorycode
  type: integer
- description: Classification code indicating the potential value of the customer account.
  name: accountclassificationcode
  type: integer
- description: Rating to indicate the value of the customer account.
  name: accountratingcode
  type: integer
- description: Category describing the relationship between the account and your organization.
  name: customertypecode
  type: integer
- description: Size category of the account for segmentation and reporting purposes.
  name: customersizecode
  type: integer
- description: Legal designation or other business type of the account for contracts or reporting purposes.
  name: businesstypecode
  type: integer
- description: Preferred method of contact.
  name: preferredcontactmethodcode
  type: integer
- description: Payment terms indicating when the customer needs to pay the total amount.
  name: paymenttermscode
  type: integer
- description: Shipping method for deliveries sent to the account address.
  name: shippingmethodcode
  type: integer
- description: Credit limit of the account for reference when addressing invoice and accounting issues.
  name: creditlimit
  type: number
- description: Credit limit converted to the system default base currency.
  name: creditlimit_base
  type: number
- description: Whether the credit for the account is on hold.
  name: creditonhold
  type: boolean
- description: Whether the account allows direct email sent from Microsoft Dynamics 365.
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
- description: Whether the account allows bulk email sent through campaigns.
  name: donotbulkemail
  type: boolean
- description: Whether the account allows bulk postal mail sent through marketing campaigns.
  name: donotbulkpostalmail
  type: boolean
- description: Whether the account accepts marketing materials such as brochures or catalogs.
  name: donotsendmm
  type: boolean
- description: Whether the account is only for marketing purposes.
  name: marketingonly
  type: boolean
- description: Whether to allow following email activity like opens, attachment views, and link clicks.
  name: followemail
  type: boolean
- description: Primary address for the account.
  name: address1
  type: object
- description: Secondary address for the account.
  name: address2
  type: object
- description: Market capitalization of the account, used as an indicator in financial performance analysis.
  name: marketcap
  type: number
- description: Market capitalization converted to the system default base currency.
  name: marketcap_base
  type: number
- description: Number of shares available to the public for the account.
  name: sharesoutstanding
  type: integer
- description: URL for the account FTP site.
  name: ftpsiteurl
  type: string
- description: Phonetic spelling of the company name, if specified in Japanese.
  name: yominame
  type: string
- description: Whether the account is active or inactive.
  name: statecode
  type: integer
- description: Account status reason.
  name: statuscode
  type: integer
- description: Aging 30 value for system use.
  name: aging30
  type: number
- description: Aging 60 value for system use.
  name: aging60
  type: number
- description: Aging 90 value for system use.
  name: aging90
  type: number
- description: Whether the account has been merged with another account.
  name: merged
  type: boolean
- description: Primary contact for the account.
  name: _primarycontactid_value
  type: string
- description: Parent account associated with this account.
  name: _parentaccountid_value
  type: string
- description: Master account that the account was merged with.
  name: _masterid_value
  type: string
- description: Local currency for the record.
  name: _transactioncurrencyid_value
  type: string
- description: User or team assigned to manage the record.
  name: _ownerid_value
  type: string
- description: Business unit that the record owner belongs to.
  name: _owningbusinessunit_value
  type: string
- description: Team that owns the account.
  name: _owningteam_value
  type: string
- description: User that owns the account.
  name: _owninguser_value
  type: string
- description: Preferred service representative for the account.
  name: _preferredsystemuserid_value
  type: string
- description: Service level agreement applied to the account.
  name: _slaid_value
  type: string
- description: User who created the record.
  name: _createdby_value
  type: string
- description: User who created the record on behalf of another user.
  name: _createdonbehalfby_value
  type: string
- description: User who last updated the record.
  name: _modifiedby_value
  type: string
- description: User who last updated the record on behalf of another user.
  name: _modifiedonbehalfby_value
  type: string
- description: Date and time when the record was created.
  name: createdon
  type: string
- description: Date and time when the record was last updated.
  name: modifiedon
  type: string
- description: Version number of the account.
  name: versionnumber
  type: integer
- description: Conversion rate of the record currency.
  name: exchangerate
  type: number
- description: For system use only. Legacy Microsoft Dynamics CRM 3.0 workflow data.
  name: participatesinworkflow
  type: boolean
- description: ID of the process associated with the account.
  name: processid
  type: string
- description: Unique identifier of the data import or data migration that created this record.
  name: importsequencenumber
  type: integer
- description: Date and time that the record was migrated.
  name: overriddencreatedon
  type: string
- description: Date and time stamp of the last on hold time.
  name: lastonholdtime
  type: string
- description: Date when the account was last included in a marketing campaign or quick campaign.
  name: lastusedincampaign
  type: string
- description: How long, in minutes, that the record was on hold.
  name: onholdtime
  type: integer
provider_name: Microsoft Dynamics 365
provider_slug: microsoft-dynamics-365
schema_file: json-schema/microsoft-dynamics-365-account-schema.json
slug: microsoft-dynamics-365-account
source_filename: microsoft-dynamics-365-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://github.com/api-search/microsoft-dynamics-365/blob/main/json-schema/microsoft-dynamics-365-account-schema.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Microsoft Dynamics 365 Account\",\n  \"description\": \"Business that represents a customer or potential customer. The company that is billed in business transactions. Based on the Microsoft Dataverse account entity (Microsoft.Dynamics.CRM.account).\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"properties\": {\n    \"accountid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier of the account.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"maxLength\": 160,\n      \"description\": \"The company or business name. This is the primary name column for the account entity.\"\n    },\n    \"accountnumber\": {\n      \"type\": \"string\",\n  \
  \    \"maxLength\": 20,\n      \"description\": \"ID number or code for the account to quickly search and identify the account in system views.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Additional information to describe the account, such as an excerpt from the company website.\"\n    },\n    \"emailaddress1\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"maxLength\": 100,\n      \"description\": \"Primary email address for the account.\"\n    },\n    \"emailaddress2\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"maxLength\": 100,\n      \"description\": \"Secondary email address for the account.\"\n    },\n    \"emailaddress3\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"maxLength\": 100,\n      \"description\": \"Alternate email address for the account.\"\n    },\n    \"telephone1\": {\n      \"type\": \"string\",\n      \"maxLength\": 50,\n      \"description\"\
  : \"Main phone number for this account.\"\n    },\n    \"telephone2\": {\n      \"type\": \"string\",\n      \"maxLength\": 50,\n      \"description\": \"Second phone number for this account.\"\n    },\n    \"telephone3\": {\n      \"type\": \"string\",\n      \"maxLength\": 50,\n      \"description\": \"Third phone number for this account.\"\n    },\n    \"fax\": {\n      \"type\": \"string\",\n      \"maxLength\": 50,\n      \"description\": \"Fax number for the account.\"\n    },\n    \"websiteurl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"maxLength\": 200,\n      \"description\": \"Website URL for the account.\"\n    },\n    \"revenue\": {\n      \"type\": \"number\",\n      \"description\": \"Annual revenue for the account, used as an indicator in financial performance analysis.\"\n    },\n    \"revenue_base\": {\n      \"type\": \"number\",\n      \"description\": \"Annual revenue converted to the system default base currency.\",\n      \"readOnly\": true\n\
  \    },\n    \"numberofemployees\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of employees that work at the account for use in marketing segmentation and demographic analysis.\"\n    },\n    \"sic\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"Standard Industrial Classification (SIC) code that indicates the account primary industry of business.\"\n    },\n    \"tickersymbol\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"Stock exchange symbol for the account to track financial performance.\"\n    },\n    \"stockexchange\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"Stock exchange at which the account is listed.\"\n    },\n    \"industrycode\": {\n      \"type\": \"integer\",\n      \"description\": \"Primary industry for the account for use in marketing segmentation and demographic analysis.\",\n      \"enum\": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12,\
  \ 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33],\n      \"x-enum-descriptions\": {\n        \"1\": \"Accounting\",\n        \"2\": \"Agriculture and Non-petrol Natural Resource Extraction\",\n        \"3\": \"Broadcasting Printing and Publishing\",\n        \"4\": \"Brokers\",\n        \"5\": \"Building Supply Retail\",\n        \"6\": \"Business Services\",\n        \"7\": \"Consulting\",\n        \"8\": \"Consumer Services\",\n        \"9\": \"Design, Direction and Creative Management\",\n        \"10\": \"Distributors, Dispatchers and Processors\",\n        \"11\": \"Doctor's Offices and Clinics\",\n        \"12\": \"Durable Manufacturing\",\n        \"13\": \"Eating and Drinking Places\",\n        \"14\": \"Entertainment Retail\",\n        \"15\": \"Equipment Rental and Leasing\",\n        \"16\": \"Financial\",\n        \"17\": \"Food and Tobacco Processing\",\n        \"18\": \"Inbound Capital Intensive Processing\",\n        \"19\": \"Inbound\
  \ Repair and Services\",\n        \"20\": \"Insurance\",\n        \"21\": \"Legal Services\",\n        \"22\": \"Non-Durable Merchandise Retail\",\n        \"23\": \"Outbound Consumer Service\",\n        \"24\": \"Petrochemical Extraction and Distribution\",\n        \"25\": \"Service Retail\",\n        \"26\": \"SIG Affiliations\",\n        \"27\": \"Social Services\",\n        \"28\": \"Special Outbound Trade Contractors\",\n        \"29\": \"Specialty Realty\",\n        \"30\": \"Transportation\",\n        \"31\": \"Utility Creation and Distribution\",\n        \"32\": \"Vehicle Retail\",\n        \"33\": \"Wholesale\"\n      }\n    },\n    \"ownershipcode\": {\n      \"type\": \"integer\",\n      \"description\": \"Ownership structure of the account.\",\n      \"enum\": [1, 2, 3, 4],\n      \"x-enum-descriptions\": {\n        \"1\": \"Public\",\n        \"2\": \"Private\",\n        \"3\": \"Subsidiary\",\n        \"4\": \"Other\"\n      }\n    },\n    \"accountcategorycode\": {\n \
  \     \"type\": \"integer\",\n      \"description\": \"Category indicating whether the customer account is standard or preferred.\",\n      \"enum\": [1, 2],\n      \"x-enum-descriptions\": {\n        \"1\": \"Preferred Customer\",\n        \"2\": \"Standard\"\n      }\n    },\n    \"accountclassificationcode\": {\n      \"type\": \"integer\",\n      \"description\": \"Classification code indicating the potential value of the customer account.\"\n    },\n    \"accountratingcode\": {\n      \"type\": \"integer\",\n      \"description\": \"Rating to indicate the value of the customer account.\"\n    },\n    \"customertypecode\": {\n      \"type\": \"integer\",\n      \"description\": \"Category describing the relationship between the account and your organization.\",\n      \"enum\": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12],\n      \"x-enum-descriptions\": {\n        \"1\": \"Competitor\",\n        \"2\": \"Consultant\",\n        \"3\": \"Customer\",\n        \"4\": \"Investor\",\n      \
  \  \"5\": \"Partner\",\n        \"6\": \"Influencer\",\n        \"7\": \"Press\",\n        \"8\": \"Prospect\",\n        \"9\": \"Reseller\",\n        \"10\": \"Supplier\",\n        \"11\": \"Vendor\",\n        \"12\": \"Other\"\n      }\n    },\n    \"customersizecode\": {\n      \"type\": \"integer\",\n      \"description\": \"Size category of the account for segmentation and reporting purposes.\"\n    },\n    \"businesstypecode\": {\n      \"type\": \"integer\",\n      \"description\": \"Legal designation or other business type of the account for contracts or reporting purposes.\"\n    },\n    \"preferredcontactmethodcode\": {\n      \"type\": \"integer\",\n      \"description\": \"Preferred method of contact.\",\n      \"enum\": [1, 2, 3, 4, 5],\n      \"x-enum-descriptions\": {\n        \"1\": \"Any\",\n        \"2\": \"Email\",\n        \"3\": \"Phone\",\n        \"4\": \"Fax\",\n        \"5\": \"Mail\"\n      }\n    },\n    \"paymenttermscode\": {\n      \"type\": \"integer\",\n\
  \      \"description\": \"Payment terms indicating when the customer needs to pay the total amount.\",\n      \"enum\": [1, 2, 3, 4],\n      \"x-enum-descriptions\": {\n        \"1\": \"Net 30\",\n        \"2\": \"2% 10, Net 30\",\n        \"3\": \"Net 45\",\n        \"4\": \"Net 60\"\n      }\n    },\n    \"shippingmethodcode\": {\n      \"type\": \"integer\",\n      \"description\": \"Shipping method for deliveries sent to the account address.\"\n    },\n    \"creditlimit\": {\n      \"type\": \"number\",\n      \"description\": \"Credit limit of the account for reference when addressing invoice and accounting issues.\"\n    },\n    \"creditlimit_base\": {\n      \"type\": \"number\",\n      \"description\": \"Credit limit converted to the system default base currency.\",\n      \"readOnly\": true\n    },\n    \"creditonhold\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the credit for the account is on hold.\"\n    },\n    \"donotemail\": {\n      \"type\": \"\
  boolean\",\n      \"description\": \"Whether the account allows direct email sent from Microsoft Dynamics 365.\"\n    },\n    \"donotphone\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account allows phone calls.\"\n    },\n    \"donotfax\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account allows faxes.\"\n    },\n    \"donotpostalmail\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account allows direct mail.\"\n    },\n    \"donotbulkemail\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account allows bulk email sent through campaigns.\"\n    },\n    \"donotbulkpostalmail\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account allows bulk postal mail sent through marketing campaigns.\"\n    },\n    \"donotsendmm\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account accepts marketing materials such as brochures or catalogs.\"\n \
  \   },\n    \"marketingonly\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account is only for marketing purposes.\"\n    },\n    \"followemail\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to allow following email activity like opens, attachment views, and link clicks.\"\n    },\n    \"address1\": {\n      \"type\": \"object\",\n      \"description\": \"Primary address for the account.\",\n      \"properties\": {\n        \"address1_addressid\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique identifier for address 1.\"\n        },\n        \"address1_name\": {\n          \"type\": \"string\",\n          \"maxLength\": 200,\n          \"description\": \"Descriptive name for the primary address, such as Corporate Headquarters.\"\n        },\n        \"address1_line1\": {\n          \"type\": \"string\",\n          \"maxLength\": 250,\n          \"description\": \"First line of the\
  \ primary address.\"\n        },\n        \"address1_line2\": {\n          \"type\": \"string\",\n          \"maxLength\": 250,\n          \"description\": \"Second line of the primary address.\"\n        },\n        \"address1_line3\": {\n          \"type\": \"string\",\n          \"maxLength\": 250,\n          \"description\": \"Third line of the primary address.\"\n        },\n        \"address1_city\": {\n          \"type\": \"string\",\n          \"maxLength\": 80,\n          \"description\": \"City for the primary address.\"\n        },\n        \"address1_stateorprovince\": {\n          \"type\": \"string\",\n          \"maxLength\": 50,\n          \"description\": \"State or province of the primary address.\"\n        },\n        \"address1_postalcode\": {\n          \"type\": \"string\",\n          \"maxLength\": 20,\n          \"description\": \"ZIP Code or postal code for the primary address.\"\n        },\n        \"address1_country\": {\n          \"type\": \"string\",\n \
  \         \"maxLength\": 80,\n          \"description\": \"Country or region for the primary address.\"\n        },\n        \"address1_county\": {\n          \"type\": \"string\",\n          \"maxLength\": 50,\n          \"description\": \"County for the primary address.\"\n        },\n        \"address1_telephone1\": {\n          \"type\": \"string\",\n          \"maxLength\": 50,\n          \"description\": \"Main phone number associated with the primary address.\"\n        },\n        \"address1_telephone2\": {\n          \"type\": \"string\",\n          \"maxLength\": 50,\n          \"description\": \"Second phone number associated with the primary address.\"\n        },\n        \"address1_telephone3\": {\n          \"type\": \"string\",\n          \"maxLength\": 50,\n          \"description\": \"Third phone number associated with the primary address.\"\n        },\n        \"address1_fax\": {\n          \"type\": \"string\",\n          \"maxLength\": 50,\n          \"description\"\
  : \"Fax number associated with the primary address.\"\n        },\n        \"address1_latitude\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Latitude value for the primary address.\"\n        },\n        \"address1_longitude\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Longitude value for the primary address.\"\n        },\n        \"address1_postofficebox\": {\n          \"type\": \"string\",\n          \"maxLength\": 20,\n          \"description\": \"Post office box number of the primary address.\"\n        },\n        \"address1_primarycontactname\": {\n          \"type\": \"string\",\n          \"maxLength\": 100,\n          \"description\": \"Name of the main contact at the primary address.\"\n        },\n        \"address1_addresstypecode\": {\n          \"type\": \"integer\",\n          \"description\": \"Primary address type.\",\n          \"enum\": [1, 2, 3, 4],\n\
  \          \"x-enum-descriptions\": {\n            \"1\": \"Bill To\",\n            \"2\": \"Ship To\",\n            \"3\": \"Primary\",\n            \"4\": \"Other\"\n          }\n        },\n        \"address1_shippingmethodcode\": {\n          \"type\": \"integer\",\n          \"description\": \"Shipping method for deliveries sent to the primary address.\",\n          \"enum\": [1, 2, 3, 4, 5, 6, 7],\n          \"x-enum-descriptions\": {\n            \"1\": \"Airborne\",\n            \"2\": \"DHL\",\n            \"3\": \"FedEx\",\n            \"4\": \"UPS\",\n            \"5\": \"Postal Mail\",\n            \"6\": \"Full Load\",\n            \"7\": \"Will Call\"\n          }\n        },\n        \"address1_freighttermscode\": {\n          \"type\": \"integer\",\n          \"description\": \"Freight terms for the primary address.\",\n          \"enum\": [1, 2],\n          \"x-enum-descriptions\": {\n            \"1\": \"FOB\",\n            \"2\": \"No Charge\"\n          }\n        },\n\
  \        \"address1_upszone\": {\n          \"type\": \"string\",\n          \"maxLength\": 4,\n          \"description\": \"UPS zone of the primary address.\"\n        },\n        \"address1_utcoffset\": {\n          \"type\": \"integer\",\n          \"description\": \"UTC offset for the primary address time zone.\"\n        },\n        \"address1_composite\": {\n          \"type\": \"string\",\n          \"description\": \"Complete primary address.\",\n          \"readOnly\": true\n        }\n      }\n    },\n    \"address2\": {\n      \"type\": \"object\",\n      \"description\": \"Secondary address for the account.\",\n      \"properties\": {\n        \"address2_addressid\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique identifier for address 2.\"\n        },\n        \"address2_name\": {\n          \"type\": \"string\",\n          \"maxLength\": 200,\n          \"description\": \"Descriptive name for the secondary address.\"\
  \n        },\n        \"address2_line1\": {\n          \"type\": \"string\",\n          \"maxLength\": 250,\n          \"description\": \"First line of the secondary address.\"\n        },\n        \"address2_line2\": {\n          \"type\": \"string\",\n          \"maxLength\": 250,\n          \"description\": \"Second line of the secondary address.\"\n        },\n        \"address2_line3\": {\n          \"type\": \"string\",\n          \"maxLength\": 250,\n          \"description\": \"Third line of the secondary address.\"\n        },\n        \"address2_city\": {\n          \"type\": \"string\",\n          \"maxLength\": 80,\n          \"description\": \"City for the secondary address.\"\n        },\n        \"address2_stateorprovince\": {\n          \"type\": \"string\",\n          \"maxLength\": 50,\n          \"description\": \"State or province of the secondary address.\"\n        },\n        \"address2_postalcode\": {\n          \"type\": \"string\",\n          \"maxLength\": 20,\n\
  \          \"description\": \"ZIP Code or postal code for the secondary address.\"\n        },\n        \"address2_country\": {\n          \"type\": \"string\",\n          \"maxLength\": 80,\n          \"description\": \"Country or region for the secondary address.\"\n        },\n        \"address2_county\": {\n          \"type\": \"string\",\n          \"maxLength\": 50,\n          \"description\": \"County for the secondary address.\"\n        },\n        \"address2_telephone1\": {\n          \"type\": \"string\",\n          \"maxLength\": 50,\n          \"description\": \"Main phone number associated with the secondary address.\"\n        },\n        \"address2_fax\": {\n          \"type\": \"string\",\n          \"maxLength\": 50,\n          \"description\": \"Fax number associated with the secondary address.\"\n        },\n        \"address2_latitude\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Latitude value for the secondary\
  \ address.\"\n        },\n        \"address2_longitude\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Longitude value for the secondary address.\"\n        },\n        \"address2_composite\": {\n          \"type\": \"string\",\n          \"description\": \"Complete secondary address.\",\n          \"readOnly\": true\n        }\n      }\n    },\n    \"marketcap\": {\n      \"type\": \"number\",\n      \"description\": \"Market capitalization of the account, used as an indicator in financial performance analysis.\"\n    },\n    \"marketcap_base\": {\n      \"type\": \"number\",\n      \"description\": \"Market capitalization converted to the system default base currency.\",\n      \"readOnly\": true\n    },\n    \"sharesoutstanding\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of shares available to the public for the account.\"\n    },\n    \"ftpsiteurl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\
  ,\n      \"description\": \"URL for the account FTP site.\"\n    },\n    \"yominame\": {\n      \"type\": \"string\",\n      \"maxLength\": 160,\n      \"description\": \"Phonetic spelling of the company name, if specified in Japanese.\"\n    },\n    \"statecode\": {\n      \"type\": \"integer\",\n      \"description\": \"Whether the account is active or inactive.\",\n      \"enum\": [0, 1],\n      \"x-enum-descriptions\": {\n        \"0\": \"Active\",\n        \"1\": \"Inactive\"\n      }\n    },\n    \"statuscode\": {\n      \"type\": \"integer\",\n      \"description\": \"Account status reason.\",\n      \"enum\": [1, 2],\n      \"x-enum-descriptions\": {\n        \"1\": \"Active\",\n        \"2\": \"Inactive\"\n      }\n    },\n    \"aging30\": {\n      \"type\": \"number\",\n      \"description\": \"Aging 30 value for system use.\",\n      \"readOnly\": true\n    },\n    \"aging60\": {\n      \"type\": \"number\",\n      \"description\": \"Aging 60 value for system use.\",\n     \
  \ \"readOnly\": true\n    },\n    \"aging90\": {\n      \"type\": \"number\",\n      \"description\": \"Aging 90 value for system use.\",\n      \"readOnly\": true\n    },\n    \"merged\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the account has been merged with another account.\",\n      \"readOnly\": true\n    },\n    \"_primarycontactid_value\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Primary contact for the account.\",\n      \"readOnly\": true\n    },\n    \"_parentaccountid_value\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Parent account associated with this account.\",\n      \"readOnly\": true\n    },\n    \"_masterid_value\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Master account that the account was merged with.\",\n      \"readOnly\": true\n    },\n    \"_transactioncurrencyid_value\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"uuid\",\n      \"description\": \"Local currency for the record.\",\n      \"readOnly\": true\n    },\n    \"_ownerid_value\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"User or team assigned to manage the record.\",\n      \"readOnly\": true\n    },\n    \"_owningbusinessunit_value\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Business unit that the record owner belongs to.\",\n      \"readOnly\": true\n    },\n    \"_owningteam_value\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Team that owns the account.\",\n      \"readOnly\": true\n    },\n    \"_owninguser_value\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"User that owns the account.\",\n      \"readOnly\": true\n    },\n    \"_preferredsystemuserid_value\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\"\
  : \"Preferred service representative for the account.\",\n      \"readOnly\": true\n    },\n    \"_slaid_value\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Service level agreement applied to the account.\",\n      \"readOnly\": true\n    },\n    \"_createdby_value\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"User who created the record.\",\n      \"readOnly\": true\n    },\n    \"_createdonbehalfby_value\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"User who created the record on behalf of another user.\",\n      \"readOnly\": true\n    },\n    \"_modifiedby_value\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"User who last updated the record.\",\n      \"readOnly\": true\n    },\n    \"_modifiedonbehalfby_value\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"User who last updated\
  \ the record on behalf of another user.\",\n      \"readOnly\": true\n    },\n    \"createdon\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when the record was created.\",\n      \"readOnly\": true\n    },\n    \"modifiedon\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when the record was last updated.\",\n      \"readOnly\": true\n    },\n    \"versionnumber\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Version number of the account.\",\n      \"readOnly\": true\n    },\n    \"exchangerate\": {\n      \"type\": \"number\",\n      \"description\": \"Conversion rate of the record currency.\",\n      \"readOnly\": true\n    },\n    \"participatesinworkflow\": {\n      \"type\": \"boolean\",\n      \"description\": \"For system use only. Legacy Microsoft Dynamics CRM 3.0 workflow data.\"\n    },\n    \"processid\": {\n   \
  \   \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"ID of the process associated with the account.\"\n    },\n    \"importsequencenumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier of the data import or data migration that created this record.\"\n    },\n    \"overriddencreatedon\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time that the record was migrated.\"\n    },\n    \"lastonholdtime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time stamp of the last on hold time.\"\n    },\n    \"lastusedincampaign\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date when the account was last included in a marketing campaign or quick campaign.\"\n    },\n    \"onholdtime\": {\n      \"type\": \"integer\",\n      \"description\": \"How long, in minutes, that the record was on\
  \ hold.\",\n      \"readOnly\": true\n    }\n  },\n  \"additionalProperties\": true,\n  \"examples\": [\n    {\n      \"name\": \"Contoso Ltd.\",\n      \"accountnumber\": \"ACC-001\",\n      \"description\": \"A global leader in technology solutions.\",\n      \"emailaddress1\": \"info@contoso.com\",\n      \"telephone1\": \"+1-425-555-0100\",\n      \"websiteurl\": \"https://www.contoso.com\",\n      \"revenue\": 5000000.00,\n      \"numberofemployees\": 250,\n      \"industrycode\": 6,\n      \"ownershipcode\": 2,\n      \"accountcategorycode\": 1,\n      \"customertypecode\": 3,\n      \"preferredcontactmethodcode\": 2,\n      \"paymenttermscode\": 1,\n      \"statecode\": 0,\n      \"statuscode\": 1,\n      \"address1\": {\n        \"address1_name\": \"Corporate Headquarters\",\n        \"address1_line1\": \"1 Microsoft Way\",\n        \"address1_city\": \"Redmond\",\n        \"address1_stateorprovince\": \"WA\",\n        \"address1_postalcode\": \"98052\",\n        \"address1_country\"\
  : \"United States\",\n        \"address1_addresstypecode\": 3\n      }\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics-365/refs/heads/main/json-schema/microsoft-dynamics-365-account-schema.json
tags:
- Business Applications
- Cloud
- CRM
- Enterprise
- ERP
- Microsoft
title: Microsoft Dynamics 365 Account
---
