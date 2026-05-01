---
description: A contact record in Oracle Eloqua representing an individual person tracked for marketing automation, email engagement, and lead management.
layout: schema
name: Eloqua Contact
properties_list:
- description: Unique identifier for the contact
  name: id
  type: string
- description: Asset type in Eloqua
  name: type
  type: string
- description: Contact display name
  name: name
  type: string
- description: Contact first name
  name: firstName
  type: string
- description: Contact last name
  name: lastName
  type: string
- description: Contact primary email address
  name: emailAddress
  type: string
- description: Contact job title
  name: title
  type: string
- description: Associated account identifier
  name: accountId
  type: string
- description: Associated account name
  name: accountName
  type: string
- description: Primary address line
  name: address1
  type: string
- description: Secondary address line
  name: address2
  type: string
- description: Tertiary address line
  name: address3
  type: string
- description: City
  name: city
  type: string
- description: State or province
  name: province
  type: string
- description: Postal or ZIP code
  name: postalCode
  type: string
- description: Country
  name: country
  type: string
- description: Business phone number
  name: businessPhone
  type: string
- description: Mobile phone number
  name: mobilePhone
  type: string
- description: Fax number
  name: fax
  type: string
- description: Account representative or sales person
  name: salesPerson
  type: string
- description: Email subscription status (true or false as string)
  name: isSubscribed
  type: string
- description: SMS subscription status
  name: isSmsSubscribed
  type: string
- description: Date the contact subscribed (Unix timestamp)
  name: subscriptionDate
  type: string
- description: Date the contact unsubscribed (Unix timestamp)
  name: unsubscriptionDate
  type: string
- description: Whether the contact email has bounced
  name: isBounceback
  type: string
- description: Date of the bounce (Unix timestamp)
  name: bouncebackDate
  type: string
- description: Custom field values for the contact
  name: fieldValues
  type: array
- description: Level of detail returned for the contact
  name: depth
  type: string
- description: Containing folder identifier
  name: folderId
  type: string
- description: Granted permissions on this contact
  name: permissions
  type: array
- description: Creation timestamp (Unix time)
  name: createdAt
  type: string
- description: User login who created the contact
  name: createdBy
  type: string
- description: Display name of the user who created the contact
  name: createdByName
  type: string
- description: Last update timestamp (Unix time)
  name: updatedAt
  type: string
- description: User login who last updated the contact
  name: updatedBy
  type: string
- description: Display name of the user who last updated the contact
  name: updatedByName
  type: string
provider_name: Oracle Eloqua
provider_slug: eloqua
schema_file: json-schema/eloqua-contact-schema.json
slug: eloqua-contact
source_filename: eloqua-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.oracle.com/en/cloud/saas/marketing/eloqua-rest-api/schemas/contact.json\",\n  \"title\": \"Eloqua Contact\",\n  \"description\": \"A contact record in Oracle Eloqua representing an individual person tracked for marketing automation, email engagement, and lead management.\",\n  \"type\": \"object\",\n  \"required\": [\"emailAddress\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the contact\",\n      \"readOnly\": true\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Asset type in Eloqua\",\n      \"const\": \"Contact\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Contact display name\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"Contact first name\"\n    },\n    \"lastName\": {\n \
  \     \"type\": \"string\",\n      \"description\": \"Contact last name\"\n    },\n    \"emailAddress\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Contact primary email address\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Contact job title\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated account identifier\",\n      \"readOnly\": true\n    },\n    \"accountName\": {\n      \"type\": \"string\",\n      \"description\": \"Associated account name\"\n    },\n    \"address1\": {\n      \"type\": \"string\",\n      \"description\": \"Primary address line\"\n    },\n    \"address2\": {\n      \"type\": \"string\",\n      \"description\": \"Secondary address line\"\n    },\n    \"address3\": {\n      \"type\": \"string\",\n      \"description\": \"Tertiary address line\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City\"\n    },\n\
  \    \"province\": {\n      \"type\": \"string\",\n      \"description\": \"State or province\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"Postal or ZIP code\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country\"\n    },\n    \"businessPhone\": {\n      \"type\": \"string\",\n      \"description\": \"Business phone number\"\n    },\n    \"mobilePhone\": {\n      \"type\": \"string\",\n      \"description\": \"Mobile phone number\"\n    },\n    \"fax\": {\n      \"type\": \"string\",\n      \"description\": \"Fax number\"\n    },\n    \"salesPerson\": {\n      \"type\": \"string\",\n      \"description\": \"Account representative or sales person\"\n    },\n    \"isSubscribed\": {\n      \"type\": \"string\",\n      \"description\": \"Email subscription status (true or false as string)\"\n    },\n    \"isSmsSubscribed\": {\n      \"type\": \"string\",\n      \"description\": \"SMS subscription status\"\n \
  \   },\n    \"subscriptionDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date the contact subscribed (Unix timestamp)\"\n    },\n    \"unsubscriptionDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date the contact unsubscribed (Unix timestamp)\"\n    },\n    \"isBounceback\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the contact email has bounced\"\n    },\n    \"bouncebackDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of the bounce (Unix timestamp)\"\n    },\n    \"fieldValues\": {\n      \"type\": \"array\",\n      \"description\": \"Custom field values for the contact\",\n      \"items\": {\n        \"$ref\": \"#/$defs/FieldValue\"\n      }\n    },\n    \"depth\": {\n      \"type\": \"string\",\n      \"enum\": [\"minimal\", \"partial\", \"complete\"],\n      \"description\": \"Level of detail returned for the contact\",\n      \"readOnly\": true\n    },\n    \"folderId\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Containing folder identifier\",\n      \"readOnly\": true\n    },\n    \"permissions\": {\n      \"type\": \"array\",\n      \"description\": \"Granted permissions on this contact\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"readOnly\": true\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"Creation timestamp (Unix time)\",\n      \"readOnly\": true\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"User login who created the contact\",\n      \"readOnly\": true\n    },\n    \"createdByName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the user who created the contact\",\n      \"readOnly\": true\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"Last update timestamp (Unix time)\",\n      \"readOnly\": true\n    },\n    \"updatedBy\": {\n      \"type\": \"string\",\n      \"description\": \"User login\
  \ who last updated the contact\",\n      \"readOnly\": true\n    },\n    \"updatedByName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the user who last updated the contact\",\n      \"readOnly\": true\n    }\n  },\n  \"$defs\": {\n    \"FieldValue\": {\n      \"type\": \"object\",\n      \"description\": \"A custom field value entry\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Field identifier\",\n          \"readOnly\": true\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Field type in Eloqua\",\n          \"readOnly\": true\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"Field value (dates are returned as Unix timestamps)\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/eloqua/refs/heads/main/json-schema/eloqua-contact-schema.json
tags:
- CRM
- Email Marketing
- Lead Management
- Marketing Automation
title: Eloqua Contact
---
