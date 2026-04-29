---
description: ''
layout: schema
name: Address
properties_list:
- description: Address line 1. If the any of the address line value is present but line 1 value is absent then blank value will be considered. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - <BR/>
  name: line1
  type: string
- description: Address line 2. If the any of the address line value is present but line 2 value is absent then blank value will be considered. <BR/> This field is required if configured as **Business Mandatory**<fon
  name: line2
  type: string
- description: Address line 3. If the any of the address line value is present but line 3 value is absent then blank value will be considered. <BR/> This field is required if configured as **Business Mandatory**<fon
  name: line3
  type: string
- description: Address line 4. If the any of the address line value is present but line 4 value is absent then blank value will be considered. <BR/> This field is required if configured as **Business Mandatory**<fon
  name: line4
  type: string
- description: City (free text). <BR/> This field will be ignored and populated internally if given country is same as institution country, and city is configured to be auto populated in Card Management > Institutio
  name: city
  type: string
- description: State. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font> * If zip flag is configured at Institution level by selecting the 'Domestic Postal Code Mandatory
  name: state
  type: string
- description: Country Code. Expressed as a 2-letter (Alpha-2) country code as defined in ISO 3166. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - <BR/> * Current Address country is required whil
  name: country
  type: string
- description: Zip Code. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - <BR/> * Required if given country is same as 'institution country', and 'zip code' is configured as mandatory in 'Card Mana
  name: zipCode
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-address-schema.json
slug: mastercard-card-issuance-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Address\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"line1\": {\n      \"type\": \"string\",\n      \"description\": \"Address line 1. If the any of the address line value is present but line 1 value is absent then blank value will be considered. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - <BR/> Current Address line1 is required while creating new client. <BR/> Office or Permanent Address line1 is required if selected as preferred Mailing Address.\"\n    },\n    \"line2\": {\n      \"type\": \"string\",\n      \"description\": \"Address line 2. If the any of the address line value is present but line 2 value is absent then blank value will be considered. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    },\n    \"line3\": {\n      \"type\": \"string\",\n      \"description\": \"Address line 3. If the any\
  \ of the address line value is present but line 3 value is absent then blank value will be considered. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    },\n    \"line4\": {\n      \"type\": \"string\",\n      \"description\": \"Address line 4. If the any of the address line value is present but line 4 value is absent then blank value will be considered. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City (free text). <BR/> This field will be ignored and populated internally if given country is same as institution country, and city is configured to be auto populated in Card Management > Institution Parameter Setup by selecting the option 'Validate Domestic Postal Code [Y]' or 'Do Not Validate Domestic Postal Code-Auto populate [D]'.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"State. <BR/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>\\n* If zip flag is configured at Institution level by selecting the 'Domestic Postal Code Mandatory' check box, then the state code must be present in the request, as per the state master configured in the system.\\n* Otherwise, if the zip flag is not configured at institution level, then regardless of the applicant's state code, this field is a free text.\\n* This field will be ignored and populated internally if given country is same as institution country,     and state is configured to be auto populated in 'Card Management > Institution Parameter Setup'     by selecting the option 'Validate Domestic Postal Code [Y]' or 'Do Not Validate Domestic Postal Code-Auto populate [D]'.\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country Code. Expressed as a 2-letter (Alpha-2) country code as defined in ISO 3166. <BR/> **Conditional Mandatory**<font\
  \ color='red'>* </font> field - <BR/>\\n* Current Address country is required while creating new client. <BR/>\\n* Office or Permanent Address country is required if selected as preferred Mailing Address.\"\n    },\n    \"zipCode\": {\n      \"type\": \"string\",\n      \"description\": \"Zip Code. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - <BR/>\\n* Required if given country is same as 'institution country', and 'zip code' is configured as mandatory     in 'Card Management > Institution Parameter Setup' by selecting the 'Validate Domestic Postal Code [Y]'. <BR/>\\n* Office or 'permanent address zip code' is required if selected as preferred 'mailing address'.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-address-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Address
---
