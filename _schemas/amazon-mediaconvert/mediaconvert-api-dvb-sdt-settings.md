---
description: Use these settings to insert a DVB Service Description Table (SDT) in the transport stream of this output. When you work directly in your JSON job specification, include this object only when your job has a transport stream output and the container settings contain the object M2tsSettings.
layout: schema
name: DvbSdtSettings
properties_list:
- description: ''
  name: OutputSdt
  type: object
- description: ''
  name: SdtInterval
  type: object
- description: ''
  name: ServiceName
  type: object
- description: ''
  name: ServiceProviderName
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-dvb-sdt-settings-schema.json
slug: mediaconvert-api-dvb-sdt-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dvb-sdt-settings-schema.json\",\n  \"title\": \"DvbSdtSettings\",\n  \"description\": \"Use these settings to insert a DVB Service Description Table (SDT) in the transport stream of this output. When you work directly in your JSON job specification, include this object only when your job has a transport stream output and the container settings contain the object M2tsSettings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OutputSdt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputSdt\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputSdt\"\n          },\n          \"description\": \"Selects method of inserting SDT information into output stream. \\\"Follow input SDT\\\" copies SDT information from input stream\
  \ to output stream. \\\"Follow input SDT if present\\\" copies SDT information from input stream to output stream if SDT information is present in the input, otherwise it will fall back on the user-defined values. Enter \\\"SDT Manually\\\" means user will enter the SDT information. \\\"No SDT\\\" means output stream will not contain SDT information.\"\n        }\n      ]\n    },\n    \"SdtInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin25Max2000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sdtInterval\"\n          },\n          \"description\": \"The number of milliseconds between instances of this table in the output transport stream.\"\n        }\n      ]\n    },\n    \"ServiceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max256\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"serviceName\"\n          },\n          \"description\"\
  : \"The service name placed in the service_descriptor in the Service Description Table. Maximum length is 256 characters.\"\n        }\n      ]\n    },\n    \"ServiceProviderName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max256\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"serviceProviderName\"\n          },\n          \"description\": \"The service provider name placed in the service_descriptor in the Service Description Table. Maximum length is 256 characters.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dvb-sdt-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DvbSdtSettings
---
