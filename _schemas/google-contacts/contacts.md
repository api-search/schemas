---
description: A person resource from the Google People API representing a contact.
layout: schema
name: Google Contact (Person)
properties_list:
- description: The resource name for the person, assigned by the server.
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
- description: The person's street addresses.
  name: addresses
  type: array
- description: The person's past or current organizations.
  name: organizations
  type: array
- description: The person's birthdays.
  name: birthdays
  type: array
- description: The person's photos.
  name: photos
  type: array
provider_name: Google People API
provider_slug: google-contacts
schema_file: json-schema/contacts.json
slug: contacts
source_filename: contacts.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-contacts/refs/heads/main/json-schema/contacts.json\",\n  \"title\": \"Google Contact (Person)\",\n  \"description\": \"A person resource from the Google People API representing a contact.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceName\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name for the person, assigned by the server.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The HTTP entity tag of the resource.\"\n    },\n    \"names\": {\n      \"type\": \"array\",\n      \"description\": \"The person's names.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"displayName\": {\n            \"type\": \"string\",\n            \"description\": \"The display name formatted according to the locale.\"\n          },\n      \
  \    \"familyName\": {\n            \"type\": \"string\",\n            \"description\": \"The family name.\"\n          },\n          \"givenName\": {\n            \"type\": \"string\",\n            \"description\": \"The given name.\"\n          },\n          \"middleName\": {\n            \"type\": \"string\",\n            \"description\": \"The middle name.\"\n          }\n        }\n      }\n    },\n    \"emailAddresses\": {\n      \"type\": \"array\",\n      \"description\": \"The person's email addresses.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"value\": {\n            \"type\": \"string\",\n            \"format\": \"email\"\n          },\n          \"type\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"phoneNumbers\": {\n      \"type\": \"array\",\n      \"description\": \"The person's phone numbers.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n      \
  \    \"value\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"addresses\": {\n      \"type\": \"array\",\n      \"description\": \"The person's street addresses.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"formattedValue\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"string\"\n          },\n          \"streetAddress\": {\n            \"type\": \"string\"\n          },\n          \"city\": {\n            \"type\": \"string\"\n          },\n          \"region\": {\n            \"type\": \"string\"\n          },\n          \"postalCode\": {\n            \"type\": \"string\"\n          },\n          \"country\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"organizations\": {\n      \"type\": \"array\",\n      \"description\": \"The person's past\
  \ or current organizations.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"title\": {\n            \"type\": \"string\"\n          },\n          \"department\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"birthdays\": {\n      \"type\": \"array\",\n      \"description\": \"The person's birthdays.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"date\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"year\": { \"type\": \"integer\" },\n              \"month\": { \"type\": \"integer\" },\n              \"day\": { \"type\": \"integer\" }\n            }\n          }\n        }\n      }\n    },\n    \"photos\": {\n      \"type\": \"array\",\n      \"description\": \"The person's photos.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\"\
  : {\n          \"url\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          },\n          \"default\": {\n            \"type\": \"boolean\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"resourceName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-contacts/refs/heads/main/json-schema/contacts.json
tags:
- Address Book
- Contacts
- Directory
- Google
- People
- Profiles
title: Google Contact (Person)
---
