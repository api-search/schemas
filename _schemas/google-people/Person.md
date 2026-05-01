---
description: A person resource from the Google People API representing a contact or profile.
layout: schema
name: Google People Person
properties_list:
- description: The resource name for the person.
  name: resourceName
  type: string
- description: The HTTP entity tag of the resource.
  name: etag
  type: string
- description: The person's names.
  name: names
  type: array
- description: The person's email addresses.
  name: emailAddresses
  type: array
- description: The person's phone numbers.
  name: phoneNumbers
  type: array
- description: The person's addresses.
  name: addresses
  type: array
- description: The person's organizations.
  name: organizations
  type: array
- description: The person's photos.
  name: photos
  type: array
- description: The person's birthdays.
  name: birthdays
  type: array
- description: The person's biographies.
  name: biographies
  type: array
- description: The person's associated URLs.
  name: urls
  type: array
provider_name: Google People
provider_slug: google-people
schema_file: json-schema/Person.json
slug: Person
source_filename: Person.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"Person.json\",\n  \"title\": \"Google People Person\",\n  \"description\": \"A person resource from the Google People API representing a contact or profile.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceName\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name for the person.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The HTTP entity tag of the resource.\"\n    },\n    \"names\": {\n      \"type\": \"array\",\n      \"description\": \"The person's names.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"displayName\": {\n            \"type\": \"string\"\n          },\n          \"familyName\": {\n            \"type\": \"string\"\n          },\n          \"givenName\": {\n            \"type\": \"string\"\n          },\n          \"middleName\": {\n            \"type\": \"\
  string\"\n          }\n        }\n      }\n    },\n    \"emailAddresses\": {\n      \"type\": \"array\",\n      \"description\": \"The person's email addresses.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"value\": {\n            \"type\": \"string\",\n            \"format\": \"email\"\n          },\n          \"type\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"phoneNumbers\": {\n      \"type\": \"array\",\n      \"description\": \"The person's phone numbers.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"value\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"addresses\": {\n      \"type\": \"array\",\n      \"description\": \"The person's addresses.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"\
  formattedValue\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"string\"\n          },\n          \"streetAddress\": {\n            \"type\": \"string\"\n          },\n          \"city\": {\n            \"type\": \"string\"\n          },\n          \"region\": {\n            \"type\": \"string\"\n          },\n          \"postalCode\": {\n            \"type\": \"string\"\n          },\n          \"country\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"organizations\": {\n      \"type\": \"array\",\n      \"description\": \"The person's organizations.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"title\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"photos\": {\n      \"type\": \"array\",\n      \"description\": \"The person's photos.\",\n \
  \     \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"url\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          }\n        }\n      }\n    },\n    \"birthdays\": {\n      \"type\": \"array\",\n      \"description\": \"The person's birthdays.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"date\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"year\": {\n                \"type\": \"integer\"\n              },\n              \"month\": {\n                \"type\": \"integer\"\n              },\n              \"day\": {\n                \"type\": \"integer\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"biographies\": {\n      \"type\": \"array\",\n      \"description\": \"The person's biographies.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"value\": {\n    \
  \        \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"urls\": {\n      \"type\": \"array\",\n      \"description\": \"The person's associated URLs.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"value\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          },\n          \"type\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-people/refs/heads/main/json-schema/Person.json
tags:
- Address Book
- Contacts
- Google
- People
- Profiles
title: Google People Person
---
