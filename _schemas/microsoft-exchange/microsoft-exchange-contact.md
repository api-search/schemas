---
description: Represents an Outlook contact in a user's mailbox as exposed through the Microsoft Graph Contacts API. A contact is an item where you can organize and save information about people and organizations you communicate with. Contacts are contained in contact folders.
layout: schema
name: Microsoft Exchange Contact
properties_list:
- description: The contact's unique identifier. By default changes when moved to a different container.
  name: id
  type: string
- description: The contact's display name
  name: displayName
  type: string
- description: The contact's given name (first name)
  name: givenName
  type: string
- description: The contact's surname (last name)
  name: surname
  type: string
- description: The contact's middle name
  name: middleName
  type: string
- description: The contact's nickname
  name: nickName
  type: string
- description: The contact's title (e.g. Mr., Mrs., Dr.)
  name: title
  type: string
- description: The contact's initials
  name: initials
  type: string
- description: The contact's suffix (e.g. Jr., Sr., III)
  name: generation
  type: string
- description: The contact's email addresses
  name: emailAddresses
  type: array
- description: The contact's business phone numbers
  name: businessPhones
  type: array
- description: The contact's home phone numbers
  name: homePhones
  type: array
- description: The contact's mobile phone number
  name: mobilePhone
  type:
  - string
  - 'null'
- description: The contact's instant messaging addresses
  name: imAddresses
  type: array
- description: The contact's job title
  name: jobTitle
  type: string
- description: The name of the contact's company
  name: companyName
  type: string
- description: The contact's department
  name: department
  type: string
- description: The location of the contact's office
  name: officeLocation
  type: string
- description: The contact's profession
  name: profession
  type: string
- description: The name of the contact's manager
  name: manager
  type: string
- description: The name of the contact's assistant
  name: assistantName
  type: string
- description: The business home page of the contact
  name: businessHomePage
  type: string
- description: The contact's business address
  name: businessAddress
  type: object
- description: The contact's home address
  name: homeAddress
  type: object
- description: Other addresses for the contact
  name: otherAddress
  type: object
- description: The name of the contact's spouse or partner
  name: spouseName
  type: string
- description: The contact's birthday in ISO 8601 format (always UTC)
  name: birthday
  type: string
- description: The names of the contact's children
  name: children
  type: array
- description: The user's notes about the contact
  name: personalNotes
  type: string
- description: The name the contact is filed under
  name: fileAs
  type: string
- description: The categories associated with the contact
  name: categories
  type: array
- description: The ID of the contact's parent folder
  name: parentFolderId
  type: string
- description: Identifies the version of the contact
  name: changeKey
  type: string
- description: The time the contact was created
  name: createdDateTime
  type: string
- description: The time the contact was last modified
  name: lastModifiedDateTime
  type: string
- description: Phonetic Japanese given name
  name: yomiGivenName
  type: string
- description: Phonetic Japanese surname
  name: yomiSurname
  type: string
- description: Phonetic Japanese company name
  name: yomiCompanyName
  type: string
provider_name: Microsoft Exchange
provider_slug: microsoft-exchange
schema_file: json-schema/microsoft-exchange-contact-schema.json
slug: microsoft-exchange-contact
source_filename: microsoft-exchange-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/microsoft-exchange/json-schema/microsoft-exchange-contact-schema.json\",\n  \"title\": \"Microsoft Exchange Contact\",\n  \"description\": \"Represents an Outlook contact in a user's mailbox as exposed through the Microsoft Graph Contacts API. A contact is an item where you can organize and save information about people and organizations you communicate with. Contacts are contained in contact folders.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The contact's unique identifier. By default changes when moved to a different container.\",\n      \"readOnly\": true\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The contact's display name\"\n    },\n    \"givenName\": {\n      \"type\": \"string\",\n      \"description\": \"The contact's given name (first\
  \ name)\"\n    },\n    \"surname\": {\n      \"type\": \"string\",\n      \"description\": \"The contact's surname (last name)\"\n    },\n    \"middleName\": {\n      \"type\": \"string\",\n      \"description\": \"The contact's middle name\"\n    },\n    \"nickName\": {\n      \"type\": \"string\",\n      \"description\": \"The contact's nickname\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The contact's title (e.g. Mr., Mrs., Dr.)\"\n    },\n    \"initials\": {\n      \"type\": \"string\",\n      \"description\": \"The contact's initials\"\n    },\n    \"generation\": {\n      \"type\": \"string\",\n      \"description\": \"The contact's suffix (e.g. Jr., Sr., III)\"\n    },\n    \"emailAddresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/emailAddress\"\n      },\n      \"description\": \"The contact's email addresses\"\n    },\n    \"businessPhones\": {\n      \"type\": \"array\",\n      \"items\": {\n    \
  \    \"type\": \"string\"\n      },\n      \"description\": \"The contact's business phone numbers\"\n    },\n    \"homePhones\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The contact's home phone numbers\"\n    },\n    \"mobilePhone\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The contact's mobile phone number\"\n    },\n    \"imAddresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The contact's instant messaging addresses\"\n    },\n    \"jobTitle\": {\n      \"type\": \"string\",\n      \"description\": \"The contact's job title\"\n    },\n    \"companyName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the contact's company\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"The contact's department\"\n    },\n    \"officeLocation\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The location of the contact's office\"\n    },\n    \"profession\": {\n      \"type\": \"string\",\n      \"description\": \"The contact's profession\"\n    },\n    \"manager\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the contact's manager\"\n    },\n    \"assistantName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the contact's assistant\"\n    },\n    \"businessHomePage\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The business home page of the contact\"\n    },\n    \"businessAddress\": {\n      \"$ref\": \"#/$defs/physicalAddress\",\n      \"description\": \"The contact's business address\"\n    },\n    \"homeAddress\": {\n      \"$ref\": \"#/$defs/physicalAddress\",\n      \"description\": \"The contact's home address\"\n    },\n    \"otherAddress\": {\n      \"$ref\": \"#/$defs/physicalAddress\",\n      \"description\": \"Other addresses for the\
  \ contact\"\n    },\n    \"spouseName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the contact's spouse or partner\"\n    },\n    \"birthday\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The contact's birthday in ISO 8601 format (always UTC)\"\n    },\n    \"children\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The names of the contact's children\"\n    },\n    \"personalNotes\": {\n      \"type\": \"string\",\n      \"description\": \"The user's notes about the contact\"\n    },\n    \"fileAs\": {\n      \"type\": \"string\",\n      \"description\": \"The name the contact is filed under\"\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The categories associated with the contact\"\n    },\n    \"parentFolderId\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"The ID of the contact's parent folder\",\n      \"readOnly\": true\n    },\n    \"changeKey\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the version of the contact\",\n      \"readOnly\": true\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the contact was created\",\n      \"readOnly\": true\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the contact was last modified\",\n      \"readOnly\": true\n    },\n    \"yomiGivenName\": {\n      \"type\": \"string\",\n      \"description\": \"Phonetic Japanese given name\"\n    },\n    \"yomiSurname\": {\n      \"type\": \"string\",\n      \"description\": \"Phonetic Japanese surname\"\n    },\n    \"yomiCompanyName\": {\n      \"type\": \"string\",\n      \"description\": \"Phonetic Japanese company name\"\n    }\n  },\n\
  \  \"$defs\": {\n    \"emailAddress\": {\n      \"type\": \"object\",\n      \"description\": \"Email address of a person or entity\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name\"\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The email address\"\n        }\n      }\n    },\n    \"physicalAddress\": {\n      \"type\": \"object\",\n      \"description\": \"Physical street address\",\n      \"properties\": {\n        \"street\": {\n          \"type\": \"string\",\n          \"description\": \"The street address\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"The city\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"The state or province\"\n        },\n        \"countryOrRegion\": {\n          \"type\": \"string\",\n       \
  \   \"description\": \"The country or region\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\",\n          \"description\": \"The postal code\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/json-schema/microsoft-exchange-contact-schema.json
tags:
- Calendar
- Collaboration
- Contacts
- Email
- Enterprise
title: Microsoft Exchange Contact
---
