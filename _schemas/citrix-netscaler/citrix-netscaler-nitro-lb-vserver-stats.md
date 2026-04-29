---
description: Performance and health statistics for a load balancing virtual server, including connection metrics, throughput, error rates, and APDEX scores.
layout: schema
name: LbVserverStats
properties_list:
- description: Name of the load balancing virtual server.
  name: name
  type: string
- description: IP address of the virtual server.
  name: primaryipaddress
  type: string
- description: Port number of the virtual server.
  name: primaryport
  type: integer
- description: Protocol type of the virtual server.
  name: type
  type: string
- description: Current operational state.
  name: state
  type: string
- description: Number of current client connections.
  name: curclntconnections
  type: number
- description: Number of current server connections.
  name: cursrvrconnections
  type: number
- description: Number of connections in ESTABLISHED state.
  name: establishedconn
  type: number
- description: Number of active persistence sessions.
  name: curpersistencesessions
  type: number
- description: Percentage of UP services bound to this virtual server.
  name: vslbhealth
  type: number
- description: Number of active (UP) services.
  name: actsvcs
  type: number
- description: Number of inactive (DOWN) services.
  name: inactsvcs
  type: number
- description: Total number of virtual server hits since last restart.
  name: tothits
  type: number
- description: Rate of hits per second.
  name: hitsrate
  type: number
- description: Total number of requests received.
  name: totalrequests
  type: number
- description: Rate of requests per second.
  name: requestsrate
  type: number
- description: Total number of responses sent.
  name: totalresponses
  type: number
- description: Rate of responses per second.
  name: responsesrate
  type: number
- description: Total number of request bytes received.
  name: totalrequestbytes
  type: number
- description: Rate of request bytes per second.
  name: requestbytesrate
  type: number
- description: Total number of response bytes sent.
  name: totalresponsebytes
  type: number
- description: Rate of response bytes per second.
  name: responsebytesrate
  type: number
- description: Total packets received.
  name: totalpktsrecvd
  type: number
- description: Rate of packets received per second.
  name: pktsrecvdrate
  type: number
- description: Total packets sent.
  name: totalpktssent
  type: number
- description: Rate of packets sent per second.
  name: pktssentrate
  type: number
- description: Total server busy errors.
  name: totalsvrbusyerr
  type: number
- description: Rate of server busy errors per second.
  name: svrbusyerrrate
  type: number
- description: Number of requests in the surge queue.
  name: surgecount
  type: number
- description: Total number of spillover events.
  name: totspillovers
  type: number
- description: Total diversions to the backup virtual server.
  name: totvserverdownbackuphits
  type: number
- description: Average client time-to-last-byte in microseconds.
  name: avgcltttlb
  type: number
- description: APDEX score based on client response times (0.0-1.0).
  name: cltresponsetimeapdex
  type: number
- description: CPU utilization in parts per million.
  name: cpuusagepm
  type: number
- description: Total HTTP/2 requests received.
  name: totalh2requests
  type: number
- description: Rate of HTTP/2 requests per second.
  name: h2requestsrate
  type: number
- description: Total HTTP/2 responses sent.
  name: totalh2responses
  type: number
- description: Rate of HTTP/2 responses per second.
  name: h2responsesrate
  type: number
- description: Total invalid request/response count.
  name: invalidrequestresponse
  type: number
- description: Total dropped invalid request/response count.
  name: invalidrequestresponsedropped
  type: number
- description: Configured spillover threshold.
  name: sothreshold
  type: number
- description: Total request retry count.
  name: reqretrycount
  type: number
- description: Times retry count was exceeded.
  name: reqretrycountexceeded
  type: number
- description: Number of deferred requests.
  name: deferredreq
  type: number
- description: Rate of deferred requests per second.
  name: deferredreqrate
  type: number
provider_name: Citrix NetScaler
provider_slug: citrix-netscaler
schema_file: json-schema/citrix-netscaler-nitro-lb-vserver-stats-schema.json
slug: citrix-netscaler-nitro-lb-vserver-stats
source_filename: citrix-netscaler-nitro-lb-vserver-stats-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LbVserverStats\",\n  \"type\": \"object\",\n  \"description\": \"Performance and health statistics for a load balancing virtual server, including connection metrics, throughput, error rates, and APDEX scores.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the load balancing virtual server.\"\n    },\n    \"primaryipaddress\": {\n      \"type\": \"string\",\n      \"description\": \"IP address of the virtual server.\"\n    },\n    \"primaryport\": {\n      \"type\": \"integer\",\n      \"description\": \"Port number of the virtual server.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Protocol type of the virtual server.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational state.\"\n    },\n    \"curclntconnections\": {\n      \"type\": \"number\",\n  \
  \    \"description\": \"Number of current client connections.\"\n    },\n    \"cursrvrconnections\": {\n      \"type\": \"number\",\n      \"description\": \"Number of current server connections.\"\n    },\n    \"establishedconn\": {\n      \"type\": \"number\",\n      \"description\": \"Number of connections in ESTABLISHED state.\"\n    },\n    \"curpersistencesessions\": {\n      \"type\": \"number\",\n      \"description\": \"Number of active persistence sessions.\"\n    },\n    \"vslbhealth\": {\n      \"type\": \"number\",\n      \"description\": \"Percentage of UP services bound to this virtual server.\"\n    },\n    \"actsvcs\": {\n      \"type\": \"number\",\n      \"description\": \"Number of active (UP) services.\"\n    },\n    \"inactsvcs\": {\n      \"type\": \"number\",\n      \"description\": \"Number of inactive (DOWN) services.\"\n    },\n    \"tothits\": {\n      \"type\": \"number\",\n      \"description\": \"Total number of virtual server hits since last restart.\"\n\
  \    },\n    \"hitsrate\": {\n      \"type\": \"number\",\n      \"description\": \"Rate of hits per second.\"\n    },\n    \"totalrequests\": {\n      \"type\": \"number\",\n      \"description\": \"Total number of requests received.\"\n    },\n    \"requestsrate\": {\n      \"type\": \"number\",\n      \"description\": \"Rate of requests per second.\"\n    },\n    \"totalresponses\": {\n      \"type\": \"number\",\n      \"description\": \"Total number of responses sent.\"\n    },\n    \"responsesrate\": {\n      \"type\": \"number\",\n      \"description\": \"Rate of responses per second.\"\n    },\n    \"totalrequestbytes\": {\n      \"type\": \"number\",\n      \"description\": \"Total number of request bytes received.\"\n    },\n    \"requestbytesrate\": {\n      \"type\": \"number\",\n      \"description\": \"Rate of request bytes per second.\"\n    },\n    \"totalresponsebytes\": {\n      \"type\": \"number\",\n      \"description\": \"Total number of response bytes sent.\"\n \
  \   },\n    \"responsebytesrate\": {\n      \"type\": \"number\",\n      \"description\": \"Rate of response bytes per second.\"\n    },\n    \"totalpktsrecvd\": {\n      \"type\": \"number\",\n      \"description\": \"Total packets received.\"\n    },\n    \"pktsrecvdrate\": {\n      \"type\": \"number\",\n      \"description\": \"Rate of packets received per second.\"\n    },\n    \"totalpktssent\": {\n      \"type\": \"number\",\n      \"description\": \"Total packets sent.\"\n    },\n    \"pktssentrate\": {\n      \"type\": \"number\",\n      \"description\": \"Rate of packets sent per second.\"\n    },\n    \"totalsvrbusyerr\": {\n      \"type\": \"number\",\n      \"description\": \"Total server busy errors.\"\n    },\n    \"svrbusyerrrate\": {\n      \"type\": \"number\",\n      \"description\": \"Rate of server busy errors per second.\"\n    },\n    \"surgecount\": {\n      \"type\": \"number\",\n      \"description\": \"Number of requests in the surge queue.\"\n    },\n    \"\
  totspillovers\": {\n      \"type\": \"number\",\n      \"description\": \"Total number of spillover events.\"\n    },\n    \"totvserverdownbackuphits\": {\n      \"type\": \"number\",\n      \"description\": \"Total diversions to the backup virtual server.\"\n    },\n    \"avgcltttlb\": {\n      \"type\": \"number\",\n      \"description\": \"Average client time-to-last-byte in microseconds.\"\n    },\n    \"cltresponsetimeapdex\": {\n      \"type\": \"number\",\n      \"description\": \"APDEX score based on client response times (0.0-1.0).\"\n    },\n    \"cpuusagepm\": {\n      \"type\": \"number\",\n      \"description\": \"CPU utilization in parts per million.\"\n    },\n    \"totalh2requests\": {\n      \"type\": \"number\",\n      \"description\": \"Total HTTP/2 requests received.\"\n    },\n    \"h2requestsrate\": {\n      \"type\": \"number\",\n      \"description\": \"Rate of HTTP/2 requests per second.\"\n    },\n    \"totalh2responses\": {\n      \"type\": \"number\",\n    \
  \  \"description\": \"Total HTTP/2 responses sent.\"\n    },\n    \"h2responsesrate\": {\n      \"type\": \"number\",\n      \"description\": \"Rate of HTTP/2 responses per second.\"\n    },\n    \"invalidrequestresponse\": {\n      \"type\": \"number\",\n      \"description\": \"Total invalid request/response count.\"\n    },\n    \"invalidrequestresponsedropped\": {\n      \"type\": \"number\",\n      \"description\": \"Total dropped invalid request/response count.\"\n    },\n    \"sothreshold\": {\n      \"type\": \"number\",\n      \"description\": \"Configured spillover threshold.\"\n    },\n    \"reqretrycount\": {\n      \"type\": \"number\",\n      \"description\": \"Total request retry count.\"\n    },\n    \"reqretrycountexceeded\": {\n      \"type\": \"number\",\n      \"description\": \"Times retry count was exceeded.\"\n    },\n    \"deferredreq\": {\n      \"type\": \"number\",\n      \"description\": \"Number of deferred requests.\"\n    },\n    \"deferredreqrate\": {\n\
  \      \"type\": \"number\",\n      \"description\": \"Rate of deferred requests per second.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/citrix-netscaler/refs/heads/main/json-schema/citrix-netscaler-nitro-lb-vserver-stats-schema.json
tags:
- API Gateway
- Application Delivery Controller
- Application Security
- Load Balancing
- SSL Offloading
- Traffic Management
- Web Application Firewall
title: LbVserverStats
---
