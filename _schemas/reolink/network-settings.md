---
description: Network configuration settings including local link, ports, WiFi, DDNS, NTP, and service endpoints.
layout: schema
name: Reolink Network Settings
properties_list:
- description: Local network link configuration
  name: LocalLink
  type: object
- description: Network port configuration
  name: NetPort
  type: object
- description: WiFi connection configuration
  name: Wifi
  type: object
provider_name: Reolink
provider_slug: reolink
schema_file: json-schema/network-settings.json
slug: network-settings
source_filename: network-settings.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"network-settings.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Reolink Network Settings\",\n  \"description\": \"Network configuration settings including local link, ports, WiFi, DDNS, NTP, and service endpoints.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LocalLink\": {\n      \"type\": \"object\",\n      \"description\": \"Local network link configuration\",\n      \"properties\": {\n        \"dns\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"auto\": {\n              \"type\": \"integer\",\n              \"description\": \"Automatic DNS (0 = manual, 1 = auto)\"\n            },\n            \"dns1\": {\n              \"type\": \"string\",\n              \"description\": \"Primary DNS server address\"\n            },\n            \"dns2\": {\n              \"type\": \"string\",\n              \"description\": \"Secondary DNS server address\"\n            }\n         \
  \ }\n        },\n        \"mac\": {\n          \"type\": \"string\",\n          \"description\": \"MAC address of the network interface\"\n        },\n        \"static\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"gateway\": {\n              \"type\": \"string\",\n              \"description\": \"Default gateway address\"\n            },\n            \"ip\": {\n              \"type\": \"string\",\n              \"description\": \"Static IP address\"\n            },\n            \"mask\": {\n              \"type\": \"string\",\n              \"description\": \"Subnet mask\"\n            }\n          }\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Link type (DHCP or Static)\",\n          \"enum\": [\"DHCP\", \"Static\"]\n        }\n      }\n    },\n    \"NetPort\": {\n      \"type\": \"object\",\n      \"description\": \"Network port configuration\",\n      \"properties\": {\n        \"httpPort\": {\n \
  \         \"type\": \"integer\",\n          \"description\": \"HTTP service port (default 80)\"\n        },\n        \"httpsPort\": {\n          \"type\": \"integer\",\n          \"description\": \"HTTPS service port (default 443)\"\n        },\n        \"mediaPort\": {\n          \"type\": \"integer\",\n          \"description\": \"Media streaming port (default 9000)\"\n        },\n        \"onvifPort\": {\n          \"type\": \"integer\",\n          \"description\": \"ONVIF service port (default 8000)\"\n        },\n        \"rtmpPort\": {\n          \"type\": \"integer\",\n          \"description\": \"RTMP streaming port (default 1935)\"\n        },\n        \"rtspPort\": {\n          \"type\": \"integer\",\n          \"description\": \"RTSP streaming port (default 554)\"\n        }\n      }\n    },\n    \"Wifi\": {\n      \"type\": \"object\",\n      \"description\": \"WiFi connection configuration\",\n      \"properties\": {\n        \"ssid\": {\n          \"type\": \"string\",\n\
  \          \"description\": \"WiFi network name\"\n        },\n        \"password\": {\n          \"type\": \"string\",\n          \"description\": \"WiFi password\"\n        },\n        \"security\": {\n          \"type\": \"string\",\n          \"description\": \"Security protocol (e.g., WPA2-PSK)\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/json-schema/network-settings.json
tags:
- IoT
- Security Cameras
- Surveillance
- Smart Home
- AI Detection
title: Reolink Network Settings
---
