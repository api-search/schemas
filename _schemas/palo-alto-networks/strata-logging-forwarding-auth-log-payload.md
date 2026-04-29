---
description: Schema for a forwarded PAN-OS authentication log entry. Authentication logs capture user authentication events processed by the firewall's Authentication Policy, providing identity-based visibility for security monitoring, compliance, and zero-trust enforcement.
layout: schema
name: AuthLogPayload
properties_list:
- description: Timestamp when the authentication log entry was received by Strata Logging Service.
  name: receive_time
  type: string
- description: Serial number of the Palo Alto Networks device that generated this authentication log entry.
  name: serial
  type: string
- description: Log type identifier, always AUTH for authentication log entries.
  name: type
  type: string
- description: Authentication log subtype indicating the outcome of the authentication event.
  name: subtype
  type: string
- description: Source IP address of the authenticating client.
  name: src
  type: string
- description: Username or user principal name presented during authentication.
  name: src_user
  type: string
- description: Authentication protocol or method used to authenticate the user.
  name: auth_method
  type: string
- description: The name of the authentication source, server profile, or identity provider (e.g., Okta-SAML, corp-ldap, radius-server).
  name: auth_source
  type: string
- description: The result of the authentication attempt indicating whether it succeeded, failed, required an additional challenge, or timed out.
  name: auth_result
  type: string
- description: Multi-factor authentication vendor name if MFA was triggered during authentication (e.g., Duo, Okta, PingID, RSA SecurID).
  name: mfa_vendor
  type: string
- description: Result of the MFA challenge if multi-factor authentication was triggered as part of the authentication flow.
  name: mfa_result
  type: string
- description: Name of the Authentication Policy rule that triggered the authentication challenge for this session.
  name: rule_name
  type: string
- description: Name of the authentication profile configured on the firewall that was used to process this authentication event.
  name: auth_profile
  type: string
- description: Hostname of the firewall that generated this authentication log entry.
  name: device_name
  type: string
- description: Virtual system name or identifier on the firewall.
  name: vsys
  type: string
- description: Name of the log forwarding profile that forwarded this log entry.
  name: log_forwarding_profile
  type: string
- description: Output format in which this log entry was forwarded.
  name: output_format
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-logging-forwarding-auth-log-payload-schema.json
slug: strata-logging-forwarding-auth-log-payload
source_filename: strata-logging-forwarding-auth-log-payload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AuthLogPayload\",\n  \"description\": \"Schema for a forwarded PAN-OS authentication log entry. Authentication logs capture user authentication events processed by the firewall's Authentication Policy, providing identity-based visibility for security monitoring, compliance, and zero-trust enforcement.\\n\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-forwarding-auth-log-payload-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"receive_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the authentication log entry was received by Strata Logging Service.\\n\"\n    },\n    \"serial\": {\n      \"type\": \"string\",\n      \"description\": \"Serial number of the Palo Alto Networks device that generated this authentication log entry.\\n\"\
  \n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"AUTH\"\n      ],\n      \"description\": \"Log type identifier, always AUTH for authentication log entries.\\n\"\n    },\n    \"subtype\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"auth-success\",\n        \"auth-fail\",\n        \"auth-challenge\",\n        \"auth-timeout\"\n      ],\n      \"description\": \"Authentication log subtype indicating the outcome of the authentication event.\\n\"\n    },\n    \"src\": {\n      \"type\": \"string\",\n      \"description\": \"Source IP address of the authenticating client.\"\n    },\n    \"src_user\": {\n      \"type\": \"string\",\n      \"description\": \"Username or user principal name presented during authentication.\\n\"\n    },\n    \"auth_method\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SAML\",\n        \"Kerberos\",\n        \"LDAP\",\n        \"RADIUS\",\n        \"TACACS+\",\n        \"local-database\",\n  \
  \      \"client-certificate\",\n        \"MFA\"\n      ],\n      \"description\": \"Authentication protocol or method used to authenticate the user.\\n\"\n    },\n    \"auth_source\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the authentication source, server profile, or identity provider (e.g., Okta-SAML, corp-ldap, radius-server).\\n\"\n    },\n    \"auth_result\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"success\",\n        \"failure\",\n        \"challenge\",\n        \"timeout\"\n      ],\n      \"description\": \"The result of the authentication attempt indicating whether it succeeded, failed, required an additional challenge, or timed out.\\n\"\n    },\n    \"mfa_vendor\": {\n      \"type\": \"string\",\n      \"description\": \"Multi-factor authentication vendor name if MFA was triggered during authentication (e.g., Duo, Okta, PingID, RSA SecurID).\\n\"\n    },\n    \"mfa_result\": {\n      \"type\": \"string\",\n      \"enum\": [\n\
  \        \"success\",\n        \"failure\",\n        \"timeout\",\n        \"bypass\"\n      ],\n      \"description\": \"Result of the MFA challenge if multi-factor authentication was triggered as part of the authentication flow.\\n\"\n    },\n    \"rule_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the Authentication Policy rule that triggered the authentication challenge for this session.\\n\"\n    },\n    \"auth_profile\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the authentication profile configured on the firewall that was used to process this authentication event.\\n\"\n    },\n    \"device_name\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname of the firewall that generated this authentication log entry.\\n\"\n    },\n    \"vsys\": {\n      \"type\": \"string\",\n      \"description\": \"Virtual system name or identifier on the firewall.\"\n    },\n    \"log_forwarding_profile\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Name of the log forwarding profile that forwarded this log entry.\\n\"\n    },\n    \"output_format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CSV\",\n        \"LEEF\",\n        \"CEF\",\n        \"JSON\",\n        \"PARQUET\"\n      ],\n      \"description\": \"Output format in which this log entry was forwarded.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-forwarding-auth-log-payload-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AuthLogPayload
---
