---
description: ''
layout: schema
name: SiteCreate
properties_list:
- description: Name for the new site.
  name: site_name
  type: string
- description: Street address.
  name: address
  type: string
- description: City name.
  name: city
  type: string
- description: State or province.
  name: state
  type: string
- description: Country name.
  name: country
  type: string
- description: Postal code.
  name: zipcode
  type: string
- description: Geographic longitude.
  name: longitude
  type: number
- description: Geographic latitude.
  name: latitude
  type: number
provider_name: Aruba
provider_slug: aruba
schema_file: json-schema/aruba-central-site-create-schema.json
slug: aruba-central-site-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SiteCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"site_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name for the new site.\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Street address.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City name.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State or province.\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country name.\"\n    },\n    \"zipcode\": {\n      \"type\": \"string\",\n      \"description\": \"Postal code.\"\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"description\": \"Geographic longitude.\"\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"description\": \"Geographic latitude.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/json-schema/aruba-central-site-create-schema.json
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
title: SiteCreate
---
