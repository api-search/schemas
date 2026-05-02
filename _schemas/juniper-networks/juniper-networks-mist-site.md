---
description: Schema for a Juniper Mist site object. Sites are the primary organizational unit in the Mist cloud platform, representing physical locations such as offices, campuses, retail stores, or warehouses. Each site contains devices (access points, switches, gateways), WLAN configurations, network policies, and location maps. Sites inherit configuration from organization-level templates and can be grouped into site groups for bulk management. RF templates and network templates define site-wide radio and network behavior.
layout: schema
name: Juniper Mist Site
properties_list:
- description: Site unique identifier assigned by the Mist cloud. Read-only.
  name: id
  type: string
- description: Parent organization identifier. Read-only.
  name: org_id
  type: string
- description: Site display name. Must be unique within the organization. Typically the location name or building identifier.
  name: name
  type: string
- description: 'Site timezone in IANA Time Zone Database format. Used for scheduling, analytics time windows, and alarm time display. Example: America/Los_Angeles, Europe/London.'
  name: timezone
  type: string
- description: ISO 3166-1 alpha-2 country code for the site location. Used to determine regulatory domain for radio channel and power settings.
  name: country_code
  type: string
- description: Physical street address of the site location. Used for geolocation and asset tracking context.
  name: address
  type: string
- description: Geographic coordinates of the site used for map placement and location-aware features.
  name: latlng
  type: object
- description: List of site group IDs this site belongs to. Site groups enable bulk configuration and policy assignment across multiple sites.
  name: sitegroup_ids
  type: array
- description: RF template ID applied to this site. RF templates define radio settings including channel width, transmit power, band steering, and client-balancing parameters across all APs at the site.
  name: rftemplate_id
  type:
  - string
  - 'null'
- description: Network template ID applied to this site. Network templates define switch port profiles, VLAN configurations, and wired network policies.
  name: networktemplate_id
  type:
  - string
  - 'null'
- description: Gateway template ID applied to this site. Gateway templates define WAN, LAN, and VPN configuration for SRX/SSR gateways.
  name: gatewaytemplate_id
  type:
  - string
  - 'null'
- description: Free-form notes for the site. Used for operational documentation and context.
  name: notes
  type: string
- description: Site creation timestamp in epoch seconds. Read-only.
  name: created_time
  type: number
- description: Last modification timestamp in epoch seconds. Read-only.
  name: modified_time
  type: number
provider_name: Juniper Networks
provider_slug: juniper-networks
schema_file: json-schema/juniper-networks-mist-site-schema.json
slug: juniper-networks-mist-site
source_filename: juniper-networks-mist-site-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/json-schema/juniper-networks-mist-site-schema.json\",\n  \"title\": \"Juniper Mist Site\",\n  \"description\": \"Schema for a Juniper Mist site object. Sites are the primary organizational unit in the Mist cloud platform, representing physical locations such as offices, campuses, retail stores, or warehouses. Each site contains devices (access points, switches, gateways), WLAN configurations, network policies, and location maps. Sites inherit configuration from organization-level templates and can be grouped into site groups for bulk management. RF templates and network templates define site-wide radio and network behavior.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Site unique identifier\
  \ assigned by the Mist cloud. Read-only.\"\n    },\n    \"org_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Parent organization identifier. Read-only.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Site display name. Must be unique within the organization. Typically the location name or building identifier.\",\n      \"minLength\": 1,\n      \"maxLength\": 64\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Site timezone in IANA Time Zone Database format. Used for scheduling, analytics time windows, and alarm time display. Example: America/Los_Angeles, Europe/London.\",\n      \"pattern\": \"^[A-Za-z]+/[A-Za-z_]+(/[A-Za-z_]+)?$\"\n    },\n    \"country_code\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code for the site location. Used to determine regulatory domain for radio channel and power settings.\",\n      \"pattern\": \"^[A-Z]{2}$\"\
  \n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Physical street address of the site location. Used for geolocation and asset tracking context.\"\n    },\n    \"latlng\": {\n      \"type\": \"object\",\n      \"description\": \"Geographic coordinates of the site used for map placement and location-aware features.\",\n      \"properties\": {\n        \"lat\": {\n          \"type\": \"number\",\n          \"minimum\": -90,\n          \"maximum\": 90,\n          \"description\": \"Latitude in decimal degrees.\"\n        },\n        \"lng\": {\n          \"type\": \"number\",\n          \"minimum\": -180,\n          \"maximum\": 180,\n          \"description\": \"Longitude in decimal degrees.\"\n        }\n      },\n      \"required\": [\"lat\", \"lng\"]\n    },\n    \"sitegroup_ids\": {\n      \"type\": \"array\",\n      \"description\": \"List of site group IDs this site belongs to. Site groups enable bulk configuration and policy assignment across multiple\
  \ sites.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uuid\"\n      }\n    },\n    \"rftemplate_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uuid\",\n      \"description\": \"RF template ID applied to this site. RF templates define radio settings including channel width, transmit power, band steering, and client-balancing parameters across all APs at the site.\"\n    },\n    \"networktemplate_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uuid\",\n      \"description\": \"Network template ID applied to this site. Network templates define switch port profiles, VLAN configurations, and wired network policies.\"\n    },\n    \"gatewaytemplate_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uuid\",\n      \"description\": \"Gateway template ID applied to this site. Gateway templates define WAN, LAN, and VPN configuration for SRX/SSR gateways.\"\n    },\n    \"notes\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Free-form notes for the site. Used for operational documentation and context.\"\n    },\n    \"created_time\": {\n      \"type\": \"number\",\n      \"description\": \"Site creation timestamp in epoch seconds. Read-only.\"\n    },\n    \"modified_time\": {\n      \"type\": \"number\",\n      \"description\": \"Last modification timestamp in epoch seconds. Read-only.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/json-schema/juniper-networks-mist-site-schema.json
tags:
- Automation
- Cloud
- Data Center
- Enterprise
- Networking
- SDN
- Security
title: Juniper Mist Site
---
