---
description: DVB Service Description Table (SDT)
layout: schema
name: DvbSdtSettings
properties_list:
- description: ''
  name: OutputSdt
  type: object
- description: ''
  name: RepInterval
  type: object
- description: ''
  name: ServiceName
  type: object
- description: ''
  name: ServiceProviderName
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-dvb-sdt-settings-schema.json
slug: medialive-api-dvb-sdt-settings
source_filename: medialive-api-dvb-sdt-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-dvb-sdt-settings-schema.json\",\n  \"title\": \"DvbSdtSettings\",\n  \"description\": \"DVB Service Description Table (SDT)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OutputSdt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DvbSdtOutputSdt\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputSdt\"\n          },\n          \"description\": \"Selects method of inserting SDT information into output stream. The sdtFollow setting copies SDT information from input stream to output stream. The sdtFollowIfPresent setting copies SDT information from input stream to output stream if SDT information is present in the input, otherwise it will fall back on the user-defined values. The sdtManual setting means user will enter the SDT\
  \ information. The sdtNone setting means output stream will not contain SDT information.\"\n        }\n      ]\n    },\n    \"RepInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin25Max2000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"repInterval\"\n          },\n          \"description\": \"The number of milliseconds between instances of this table in the output transport stream.\"\n        }\n      ]\n    },\n    \"ServiceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max256\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"serviceName\"\n          },\n          \"description\": \"The service name placed in the serviceDescriptor in the Service Description Table. Maximum length is 256 characters.\"\n        }\n      ]\n    },\n    \"ServiceProviderName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max256\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"serviceProviderName\"\n          },\n          \"description\": \"The service provider name placed in the serviceDescriptor in the Service Description Table. Maximum length is 256 characters.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-dvb-sdt-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DvbSdtSettings
---
