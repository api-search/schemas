---
description: RetrieveAnAdministeredOrganizationResponse200 from LinkedIn API
layout: schema
name: RetrieveAnAdministeredOrganizationResponse200
properties_list:
- description: ''
  name: vanityName
  type: string
- description: ''
  name: localizedName
  type: string
- description: ''
  name: website
  type: object
- description: ''
  name: groups
  type: array
- description: ''
  name: versionTag
  type: string
- description: ''
  name: defaultLocale
  type: object
- description: ''
  name: alternativeNames
  type: array
- description: ''
  name: specialties
  type: array
- description: ''
  name: parentRelationship
  type: object
- description: ''
  name: localizedSpecialties
  type: array
- description: ''
  name: industries
  type: array
- description: ''
  name: name
  type: object
- description: ''
  name: primaryOrganizationType
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: autoCreated
  type: boolean
- description: ''
  name: localizedWebsite
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-community-retrieve-an-administered-organization-response200-schema.json
slug: linkedin-marketing-community-retrieve-an-administered-organization-response200
source_filename: linkedin-marketing-community-retrieve-an-administered-organization-response200-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-community-retrieve-an-administered-organization-response200-schema.json\",\n  \"title\": \"RetrieveAnAdministeredOrganizationResponse200\",\n  \"description\": \"RetrieveAnAdministeredOrganizationResponse200 from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vanityName\": {\n      \"type\": \"string\",\n      \"example\": \"Example Name\"\n    },\n    \"localizedName\": {\n      \"type\": \"string\",\n      \"example\": \"Example Name\"\n    },\n    \"website\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"localized\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"en_US\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"preferredLocale\": {\n          \"type\": \"object\",\n\
  \          \"properties\": {\n            \"country\": {\n              \"type\": \"string\"\n            },\n            \"language\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"items\": {}\n    },\n    \"versionTag\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"defaultLocale\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"country\": {\n          \"type\": \"string\"\n        },\n        \"language\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"alternativeNames\": {\n      \"type\": \"array\",\n      \"items\": {}\n    },\n    \"specialties\": {\n      \"type\": \"array\",\n      \"items\": {}\n    },\n    \"parentRelationship\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"relationshipStatus\": {\n          \"type\": \"string\"\n        },\n        \"parent\": {\n       \
  \   \"type\": \"string\"\n        }\n      }\n    },\n    \"localizedSpecialties\": {\n      \"type\": \"array\",\n      \"items\": {}\n    },\n    \"industries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"name\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"localized\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"en_US\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"preferredLocale\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"country\": {\n              \"type\": \"string\"\n            },\n            \"language\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"primaryOrganizationType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 42\n  \
  \  },\n    \"autoCreated\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"localizedWebsite\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-community-retrieve-an-administered-organization-response200-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: RetrieveAnAdministeredOrganizationResponse200
---
