---
description: Schema for a forwarded PAN-OS URL filtering log entry. URL logs capture web access events evaluated by the URL Filtering security profile, providing visibility into browsing activity, policy enforcement, and URL category decisions.
layout: schema
name: UrlLogPayload
properties_list:
- description: Timestamp when the URL log entry was received by Strata Logging Service.
  name: receive_time
  type: string
- description: Serial number of the Palo Alto Networks device that generated this URL log entry.
  name: serial
  type: string
- description: Log type identifier, always URL for URL filtering log entries.
  name: type
  type: string
- description: Source IP address of the client making the web request.
  name: src
  type: string
- description: Destination IP address of the web server being accessed.
  name: dst
  type: string
- description: Source port number of the HTTP/HTTPS session.
  name: sport
  type: integer
- description: Destination port number of the HTTP/HTTPS session.
  name: dport
  type: integer
- description: Application identified by App-ID for the web session (e.g., web-browsing, ssl, google-base).
  name: app
  type: string
- description: The full URL that was requested, including protocol, hostname, path, and query parameters if present.
  name: url
  type: string
- description: URL category classification assigned by PAN-DB URL filtering database (e.g., business-and-economy, malware, social-networking, command-and-control).
  name: url_category
  type: string
- description: Action applied to the URL request by the URL Filtering security profile configured on the matching security policy rule.
  name: action
  type: string
- description: HTTP method of the web request.
  name: http_method
  type: string
- description: MIME content type of the HTTP response.
  name: content_type
  type: string
- description: Source user identity associated with the web request if User-ID is enabled.
  name: src_user
  type: string
- description: Name of the security policy rule that matched the session containing this URL request.
  name: rule_name
  type: string
- description: Hostname of the firewall that generated this URL log entry.
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
schema_file: json-schema/strata-logging-forwarding-url-log-payload-schema.json
slug: strata-logging-forwarding-url-log-payload
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UrlLogPayload\",\n  \"description\": \"Schema for a forwarded PAN-OS URL filtering log entry. URL logs capture web access events evaluated by the URL Filtering security profile, providing visibility into browsing activity, policy enforcement, and URL category decisions.\\n\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-forwarding-url-log-payload-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"receive_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the URL log entry was received by Strata Logging Service.\\n\"\n    },\n    \"serial\": {\n      \"type\": \"string\",\n      \"description\": \"Serial number of the Palo Alto Networks device that generated this URL log entry.\\n\"\n    },\n    \"type\": {\n      \"type\": \"string\"\
  ,\n      \"enum\": [\n        \"URL\"\n      ],\n      \"description\": \"Log type identifier, always URL for URL filtering log entries.\"\n    },\n    \"src\": {\n      \"type\": \"string\",\n      \"description\": \"Source IP address of the client making the web request.\"\n    },\n    \"dst\": {\n      \"type\": \"string\",\n      \"description\": \"Destination IP address of the web server being accessed.\"\n    },\n    \"sport\": {\n      \"type\": \"integer\",\n      \"description\": \"Source port number of the HTTP/HTTPS session.\"\n    },\n    \"dport\": {\n      \"type\": \"integer\",\n      \"description\": \"Destination port number of the HTTP/HTTPS session.\"\n    },\n    \"app\": {\n      \"type\": \"string\",\n      \"description\": \"Application identified by App-ID for the web session (e.g., web-browsing, ssl, google-base).\\n\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The full URL that was requested, including protocol, hostname, path,\
  \ and query parameters if present.\\n\"\n    },\n    \"url_category\": {\n      \"type\": \"string\",\n      \"description\": \"URL category classification assigned by PAN-DB URL filtering database (e.g., business-and-economy, malware, social-networking, command-and-control).\\n\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"allow\",\n        \"block\",\n        \"continue\",\n        \"override\",\n        \"alert\"\n      ],\n      \"description\": \"Action applied to the URL request by the URL Filtering security profile configured on the matching security policy rule.\\n\"\n    },\n    \"http_method\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"GET\",\n        \"POST\",\n        \"PUT\",\n        \"DELETE\",\n        \"HEAD\",\n        \"OPTIONS\",\n        \"PATCH\",\n        \"CONNECT\"\n      ],\n      \"description\": \"HTTP method of the web request.\"\n    },\n    \"content_type\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"MIME content type of the HTTP response.\"\n    },\n    \"src_user\": {\n      \"type\": \"string\",\n      \"description\": \"Source user identity associated with the web request if User-ID is enabled.\\n\"\n    },\n    \"rule_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the security policy rule that matched the session containing this URL request.\\n\"\n    },\n    \"device_name\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname of the firewall that generated this URL log entry.\"\n    },\n    \"vsys\": {\n      \"type\": \"string\",\n      \"description\": \"Virtual system name or identifier on the firewall.\"\n    },\n    \"log_forwarding_profile\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the log forwarding profile that forwarded this log entry.\\n\"\n    },\n    \"output_format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CSV\",\n        \"LEEF\",\n        \"CEF\",\n    \
  \    \"JSON\",\n        \"PARQUET\"\n      ],\n      \"description\": \"Output format in which this log entry was forwarded.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-logging-forwarding-url-log-payload-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: UrlLogPayload
---
