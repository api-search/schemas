---
description: Physical site or location used to geographically organize network devices within Aruba Central.
layout: schema
name: Site
properties_list:
- description: Unique identifier for the site.
  name: site_id
  type: integer
- description: Name of the site.
  name: site_name
  type: string
- description: Street address of the site.
  name: address
  type: string
- description: City where the site is located.
  name: city
  type: string
- description: State or province where the site is located.
  name: state
  type: string
- description: Country where the site is located.
  name: country
  type: string
- description: Postal code for the site location.
  name: zipcode
  type: string
- description: Geographic longitude coordinate.
  name: longitude
  type: number
- description: Geographic latitude coordinate.
  name: latitude
  type: number
- description: Tags applied to the site.
  name: tags
  type: array
- description: Number of devices associated with the site.
  name: associated_device_count
  type: integer
provider_name: Aruba
provider_slug: aruba
schema_file: json-schema/aruba-central-site-schema.json
slug: aruba-central-site
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Site\",\n  \"type\": \"object\",\n  \"description\": \"Physical site or location used to geographically organize network devices within Aruba Central.\",\n  \"properties\": {\n    \"site_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the site.\"\n    },\n    \"site_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the site.\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Street address of the site.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City where the site is located.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State or province where the site is located.\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country where the site is located.\"\n    },\n    \"zipcode\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Postal code for the site location.\"\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"description\": \"Geographic longitude coordinate.\"\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"description\": \"Geographic latitude coordinate.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags applied to the site.\"\n    },\n    \"associated_device_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of devices associated with the site.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/json-schema/aruba-central-site-schema.json
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
title: Site
---
