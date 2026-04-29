---
description: NetScaler appliance configuration including network settings, system parameters, and operational options.
layout: schema
name: NsConfig
properties_list:
- description: The NetScaler IP (NSIP) address of the appliance. This is the primary management IP address.
  name: ipaddress
  type: string
- description: Subnet mask associated with the NSIP address.
  name: netmask
  type: string
- description: VLAN ID for the NSIP address. Range 2-4094.
  name: nsvlan
  type: integer
- description: Network interfaces bound to the NSVLAN. Format is slot/port (e.g., 1/1).
  name: ifnum
  type: string
- description: Whether the NSVLAN is tagged or untagged.
  name: tagged
  type: string
- description: HTTP port(s) on the appliance. Default is 80.
  name: httpport
  type: array
- description: Maximum number of connections per service. Zero means unlimited.
  name: maxconn
  type: integer
- description: Maximum number of requests per connection. Zero means unlimited.
  name: maxreq
  type: integer
- description: Whether to insert the client IP address into the HTTP header of requests forwarded to the service.
  name: cip
  type: string
- description: Name of the HTTP header used to insert the client IP address when CIP is enabled.
  name: cipheader
  type: string
- description: Version of the cookie inserted by the NetScaler for persistence.
  name: cookieversion
  type: string
- description: Whether the secure flag is set on persistence cookies.
  name: securecookie
  type: string
- description: Minimum path MTU value. Range 168-1500.
  name: pmtumin
  type: integer
- description: Timeout in minutes for path MTU discovery. Range 1-1440.
  name: pmtutimeout
  type: integer
- description: Port range for FTP data connections (e.g., 1024-65535).
  name: ftpportrange
  type: string
- description: Time zone setting for the appliance (e.g., GMT+05:30-IST-Asia/Kolkata).
  name: timezone
  type: string
- description: Percentage of shared quota to be granted at a time for max client connections.
  name: grantquotamaxclient
  type: integer
- description: Percentage of shared quota to be granted at a time for spillover threshold.
  name: grantquotaspillover
  type: integer
- description: Port range for cache redirection.
  name: crportrange
  type: string
- description: The type of the NetScaler appliance.
  name: systemtype
  type: string
- description: Primary IP address of the HA pair.
  name: primaryip
  type: string
- description: Primary IPv6 address of the HA pair.
  name: primaryip6
  type: string
- description: Internal flags for the configuration.
  name: flags
  type: integer
- description: Timestamp of the last configuration change.
  name: lastconfigchangedtime
  type: string
- description: Timestamp of the last configuration save.
  name: lastconfigsavetime
  type: string
- description: Current system time on the appliance.
  name: currentsytemtime
  type: string
- description: Current system time as epoch seconds.
  name: systemtime
  type: integer
- description: Whether the running configuration has unsaved changes.
  name: configchanged
  type: boolean
- description: Mapped IP address for the NSIP.
  name: mappedip
  type: string
- description: Number of consecutive IP addresses in the range beginning with the mapped IP.
  name: range
  type: integer
provider_name: Citrix NetScaler
provider_slug: citrix-netscaler
schema_file: json-schema/citrix-netscaler-nitro-ns-config-schema.json
slug: citrix-netscaler-nitro-ns-config
source_filename: citrix-netscaler-nitro-ns-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NsConfig\",\n  \"type\": \"object\",\n  \"description\": \"NetScaler appliance configuration including network settings, system parameters, and operational options.\",\n  \"properties\": {\n    \"ipaddress\": {\n      \"type\": \"string\",\n      \"description\": \"The NetScaler IP (NSIP) address of the appliance. This is the primary management IP address.\"\n    },\n    \"netmask\": {\n      \"type\": \"string\",\n      \"description\": \"Subnet mask associated with the NSIP address.\"\n    },\n    \"nsvlan\": {\n      \"type\": \"integer\",\n      \"description\": \"VLAN ID for the NSIP address. Range 2-4094.\"\n    },\n    \"ifnum\": {\n      \"type\": \"string\",\n      \"description\": \"Network interfaces bound to the NSVLAN. Format is slot/port (e.g., 1/1).\"\n    },\n    \"tagged\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the NSVLAN is tagged or untagged.\"\n\
  \    },\n    \"httpport\": {\n      \"type\": \"array\",\n      \"description\": \"HTTP port(s) on the appliance. Default is 80.\"\n    },\n    \"maxconn\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of connections per service. Zero means unlimited.\"\n    },\n    \"maxreq\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of requests per connection. Zero means unlimited.\"\n    },\n    \"cip\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to insert the client IP address into the HTTP header of requests forwarded to the service.\"\n    },\n    \"cipheader\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the HTTP header used to insert the client IP address when CIP is enabled.\"\n    },\n    \"cookieversion\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the cookie inserted by the NetScaler for persistence.\"\n    },\n    \"securecookie\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"Whether the secure flag is set on persistence cookies.\"\n    },\n    \"pmtumin\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum path MTU value. Range 168-1500.\"\n    },\n    \"pmtutimeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Timeout in minutes for path MTU discovery. Range 1-1440.\"\n    },\n    \"ftpportrange\": {\n      \"type\": \"string\",\n      \"description\": \"Port range for FTP data connections (e.g., 1024-65535).\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Time zone setting for the appliance (e.g., GMT+05:30-IST-Asia/Kolkata).\"\n    },\n    \"grantquotamaxclient\": {\n      \"type\": \"integer\",\n      \"description\": \"Percentage of shared quota to be granted at a time for max client connections.\"\n    },\n    \"grantquotaspillover\": {\n      \"type\": \"integer\",\n      \"description\": \"Percentage of shared quota to be granted at a time for spillover threshold.\"\
  \n    },\n    \"crportrange\": {\n      \"type\": \"string\",\n      \"description\": \"Port range for cache redirection.\"\n    },\n    \"systemtype\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the NetScaler appliance.\"\n    },\n    \"primaryip\": {\n      \"type\": \"string\",\n      \"description\": \"Primary IP address of the HA pair.\"\n    },\n    \"primaryip6\": {\n      \"type\": \"string\",\n      \"description\": \"Primary IPv6 address of the HA pair.\"\n    },\n    \"flags\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal flags for the configuration.\"\n    },\n    \"lastconfigchangedtime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of the last configuration change.\"\n    },\n    \"lastconfigsavetime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of the last configuration save.\"\n    },\n    \"currentsytemtime\": {\n      \"type\": \"string\",\n      \"description\": \"Current system\
  \ time on the appliance.\"\n    },\n    \"systemtime\": {\n      \"type\": \"integer\",\n      \"description\": \"Current system time as epoch seconds.\"\n    },\n    \"configchanged\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the running configuration has unsaved changes.\"\n    },\n    \"mappedip\": {\n      \"type\": \"string\",\n      \"description\": \"Mapped IP address for the NSIP.\"\n    },\n    \"range\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of consecutive IP addresses in the range beginning with the mapped IP.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/json-schema/citrix-netscaler-nitro-ns-config-schema.json
tags:
- API Gateway
- Application Delivery Controller
- Application Security
- Load Balancing
- SSL Offloading
- Traffic Management
- Web Application Firewall
title: NsConfig
---
