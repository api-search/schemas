---
description: Represents an aggregation of information about a person from across mail, contacts, and social networks as exposed through the Microsoft Graph People API. People can be local contacts, contacts from social networking, the organization's directory, and people from recent communications.
layout: schema
name: Microsoft Exchange Person
properties_list:
- description: The person's unique identifier
  name: id
  type: string
- description: The person's display name
  name: displayName
  type: string
- description: The person's given name
  name: givenName
  type: string
- description: The person's surname
  name: surname
  type: string
- description: The person's birthday
  name: birthday
  type: string
- description: Free-form notes about this person
  name: personNotes
  type: string
- description: Whether the user has flagged this person as a favorite
  name: isFavorite
  type: boolean
- description: The person's job title
  name: jobTitle
  type: string
- description: The name of the person's company
  name: companyName
  type: string
- description: The person's department
  name: department
  type: string
- description: The location of the person's office
  name: officeLocation
  type: string
- description: The person's profession
  name: profession
  type: string
- description: The user principal name (UPN) in alias@domain format per RFC 822
  name: userPrincipalName
  type: string
- description: The SIP address for VOIP instant messaging
  name: imAddress
  type: string
- description: The person's email addresses with relevance scores
  name: scoredEmailAddresses
  type: array
- description: The person's phone numbers
  name: phones
  type: array
- description: The person's addresses
  name: postalAddresses
  type: array
- description: The person's websites
  name: websites
  type: array
- description: The type of person
  name: personType
  type: object
- description: Phonetic Japanese company name
  name: yomiCompany
  type: string
provider_name: Microsoft Exchange
provider_slug: microsoft-exchange
schema_file: json-schema/microsoft-exchange-person-schema.json
slug: microsoft-exchange-person
source_filename: microsoft-exchange-person-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/microsoft-exchange/json-schema/microsoft-exchange-person-schema.json\",\n  \"title\": \"Microsoft Exchange Person\",\n  \"description\": \"Represents an aggregation of information about a person from across mail, contacts, and social networks as exposed through the Microsoft Graph People API. People can be local contacts, contacts from social networking, the organization's directory, and people from recent communications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The person's unique identifier\",\n      \"readOnly\": true\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The person's display name\"\n    },\n    \"givenName\": {\n      \"type\": \"string\",\n      \"description\": \"The person's given name\"\n    },\n    \"surname\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The person's surname\"\n    },\n    \"birthday\": {\n      \"type\": \"string\",\n      \"description\": \"The person's birthday\"\n    },\n    \"personNotes\": {\n      \"type\": \"string\",\n      \"description\": \"Free-form notes about this person\"\n    },\n    \"isFavorite\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user has flagged this person as a favorite\"\n    },\n    \"jobTitle\": {\n      \"type\": \"string\",\n      \"description\": \"The person's job title\"\n    },\n    \"companyName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the person's company\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"The person's department\"\n    },\n    \"officeLocation\": {\n      \"type\": \"string\",\n      \"description\": \"The location of the person's office\"\n    },\n    \"profession\": {\n      \"type\": \"string\",\n      \"description\": \"The person's\
  \ profession\"\n    },\n    \"userPrincipalName\": {\n      \"type\": \"string\",\n      \"description\": \"The user principal name (UPN) in alias@domain format per RFC 822\"\n    },\n    \"imAddress\": {\n      \"type\": \"string\",\n      \"description\": \"The SIP address for VOIP instant messaging\",\n      \"readOnly\": true\n    },\n    \"scoredEmailAddresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/scoredEmailAddress\"\n      },\n      \"description\": \"The person's email addresses with relevance scores\"\n    },\n    \"phones\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/phone\"\n      },\n      \"description\": \"The person's phone numbers\"\n    },\n    \"postalAddresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/location\"\n      },\n      \"description\": \"The person's addresses\"\n    },\n    \"websites\": {\n      \"type\": \"array\",\n      \"items\": {\n\
  \        \"$ref\": \"#/$defs/website\"\n      },\n      \"description\": \"The person's websites\"\n    },\n    \"personType\": {\n      \"$ref\": \"#/$defs/personType\",\n      \"description\": \"The type of person\"\n    },\n    \"yomiCompany\": {\n      \"type\": \"string\",\n      \"description\": \"Phonetic Japanese company name\"\n    }\n  },\n  \"$defs\": {\n    \"scoredEmailAddress\": {\n      \"type\": \"object\",\n      \"description\": \"An email address with a relevance score\",\n      \"properties\": {\n        \"address\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The email address\"\n        },\n        \"relevanceScore\": {\n          \"type\": \"number\",\n          \"description\": \"The relevance score (0.0 to 100.0)\"\n        },\n        \"selectionLikelihood\": {\n          \"type\": \"string\",\n          \"enum\": [\"notSpecified\", \"high\"],\n          \"description\": \"The likelihood the email would be\
  \ selected\"\n        }\n      }\n    },\n    \"phone\": {\n      \"type\": \"object\",\n      \"description\": \"A phone number\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"home\", \"business\", \"mobile\", \"other\", \"assistant\", \"homeFax\", \"businessFax\", \"otherFax\", \"pager\", \"radio\"],\n          \"description\": \"The type of phone number\"\n        },\n        \"number\": {\n          \"type\": \"string\",\n          \"description\": \"The phone number\"\n        }\n      }\n    },\n    \"location\": {\n      \"type\": \"object\",\n      \"description\": \"Location information\",\n      \"properties\": {\n        \"displayName\": {\n          \"type\": \"string\"\n        },\n        \"locationType\": {\n          \"type\": \"string\"\n        },\n        \"locationUri\": {\n          \"type\": \"string\"\n        },\n        \"address\": {\n          \"$ref\": \"#/$defs/physicalAddress\"\n        }\n      }\n\
  \    },\n    \"physicalAddress\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"street\": { \"type\": \"string\" },\n        \"city\": { \"type\": \"string\" },\n        \"state\": { \"type\": \"string\" },\n        \"countryOrRegion\": { \"type\": \"string\" },\n        \"postalCode\": { \"type\": \"string\" }\n      }\n    },\n    \"website\": {\n      \"type\": \"object\",\n      \"description\": \"A website\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"other\", \"home\", \"work\", \"blog\", \"profile\"],\n          \"description\": \"The type of website\"\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL of the website\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the website\"\n        }\n      }\n    },\n    \"personType\": {\n      \"\
  type\": \"object\",\n      \"description\": \"The type of person\",\n      \"properties\": {\n        \"class\": {\n          \"type\": \"string\",\n          \"description\": \"The data source type (e.g. Person, Group)\"\n        },\n        \"subclass\": {\n          \"type\": \"string\",\n          \"description\": \"The sub-type (e.g. OrganizationUser, PersonalContact, UnifiedGroup)\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/json-schema/microsoft-exchange-person-schema.json
tags:
- Calendar
- Collaboration
- Contacts
- Email
- Enterprise
title: Microsoft Exchange Person
---
