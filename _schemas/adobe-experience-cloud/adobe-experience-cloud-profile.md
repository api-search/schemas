---
description: A unified customer profile representing an individual across Adobe Experience Cloud products, combining identity data, demographic attributes, behavioral signals, and segment memberships.
layout: schema
name: Adobe Experience Cloud Profile
properties_list:
- description: The unique identifier for the unified profile.
  name: profileId
  type: string
- description: A map of identity namespaces to identity values associated with this profile.
  name: identityMap
  type: object
- description: Demographic information about the individual.
  name: person
  type: object
- description: The personal email address.
  name: personalEmail
  type: object
- description: The mobile phone number.
  name: mobilePhone
  type: object
- description: The home postal address.
  name: homeAddress
  type: object
- description: A map of segment namespace to segment membership details.
  name: segmentMembership
  type: object
- description: Privacy and marketing consent preferences.
  name: consents
  type: object
- description: When the profile was first created.
  name: created
  type: string
- description: When the profile was last updated.
  name: lastModified
  type: string
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/adobe-experience-cloud-profile.json
slug: adobe-experience-cloud-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"adobe-experience-cloud-profile.json\",\n  \"title\": \"Adobe Experience Cloud Profile\",\n  \"description\": \"A unified customer profile representing an individual across Adobe Experience Cloud products, combining identity data, demographic attributes, behavioral signals, and segment memberships.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"profileId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the unified profile.\"\n    },\n    \"identityMap\": {\n      \"type\": \"object\",\n      \"description\": \"A map of identity namespaces to identity values associated with this profile.\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\",\n              \"description\": \"The identity value.\"\
  \n            },\n            \"primary\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether this is the primary identity for the namespace.\"\n            },\n            \"authenticatedState\": {\n              \"type\": \"string\",\n              \"enum\": [\"ambiguous\", \"authenticated\", \"loggedOut\"],\n              \"description\": \"The authentication state of this identity.\"\n            }\n          },\n          \"required\": [\"id\"]\n        }\n      }\n    },\n    \"person\": {\n      \"type\": \"object\",\n      \"description\": \"Demographic information about the individual.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"firstName\": {\n              \"type\": \"string\",\n              \"description\": \"The first name of the individual.\"\n            },\n            \"lastName\": {\n              \"type\": \"string\",\n              \"description\": \"The\
  \ last name of the individual.\"\n            },\n            \"fullName\": {\n              \"type\": \"string\",\n              \"description\": \"The full name of the individual.\"\n            }\n          }\n        },\n        \"birthDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"The date of birth.\"\n        },\n        \"gender\": {\n          \"type\": \"string\",\n          \"enum\": [\"male\", \"female\", \"not_specified\", \"non_specific\"],\n          \"description\": \"The gender of the individual.\"\n        }\n      }\n    },\n    \"personalEmail\": {\n      \"type\": \"object\",\n      \"description\": \"The personal email address.\",\n      \"properties\": {\n        \"address\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The email address.\"\n        },\n        \"primary\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this is\
  \ the primary email.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"active\", \"incomplete\", \"blacklisted\", \"blocked\"],\n          \"description\": \"The email subscription status.\"\n        }\n      }\n    },\n    \"mobilePhone\": {\n      \"type\": \"object\",\n      \"description\": \"The mobile phone number.\",\n      \"properties\": {\n        \"number\": {\n          \"type\": \"string\",\n          \"description\": \"The phone number.\"\n        },\n        \"countryCode\": {\n          \"type\": \"string\",\n          \"description\": \"The country dialing code.\"\n        }\n      }\n    },\n    \"homeAddress\": {\n      \"type\": \"object\",\n      \"description\": \"The home postal address.\",\n      \"properties\": {\n        \"street1\": {\n          \"type\": \"string\"\n        },\n        \"street2\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n     \
  \   \"stateProvince\": {\n          \"type\": \"string\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\"\n        },\n        \"country\": {\n          \"type\": \"string\"\n        },\n        \"countryCode\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 3166-1 alpha-2 country code.\"\n        }\n      }\n    },\n    \"segmentMembership\": {\n      \"type\": \"object\",\n      \"description\": \"A map of segment namespace to segment membership details.\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"additionalProperties\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"status\": {\n              \"type\": \"string\",\n              \"enum\": [\"realized\", \"existing\", \"exited\"],\n              \"description\": \"The segment membership status.\"\n            },\n            \"lastQualificationTime\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\"\
  ,\n              \"description\": \"When the profile last qualified for the segment.\"\n            }\n          }\n        }\n      }\n    },\n    \"consents\": {\n      \"type\": \"object\",\n      \"description\": \"Privacy and marketing consent preferences.\",\n      \"properties\": {\n        \"marketing\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"email\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"val\": {\n                  \"type\": \"string\",\n                  \"enum\": [\"y\", \"n\", \"p\", \"u\"],\n                  \"description\": \"Consent value: yes, no, pending, unknown.\"\n                }\n              }\n            },\n            \"push\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"val\": {\n                  \"type\": \"string\",\n                  \"enum\": [\"y\", \"n\", \"p\", \"u\"]\n                }\n              }\n    \
  \        },\n            \"sms\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"val\": {\n                  \"type\": \"string\",\n                  \"enum\": [\"y\", \"n\", \"p\", \"u\"]\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the profile was first created.\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the profile was last updated.\"\n    }\n  },\n  \"required\": [\"profileId\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/adobe-experience-cloud-profile.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: Adobe Experience Cloud Profile
---
