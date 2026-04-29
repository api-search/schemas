---
description: InputData schema from Adyen API
layout: schema
name: InputData
properties_list:
- description: ''
  name: Device
  type: object
- description: ''
  name: InfoQualify
  type: object
- description: ''
  name: InputCommand
  type: object
- description: ''
  name: NotifyCardInputFlag
  type: boolean
- description: ''
  name: MaxInputTime
  type: integer
- description: ''
  name: ImmediateResponseFlag
  type: boolean
- description: ''
  name: MinLength
  type: integer
- description: ''
  name: MaxLength
  type: integer
- description: ''
  name: MaxDecimalLength
  type: integer
- description: ''
  name: WaitUserValidationFlag
  type: boolean
- description: ''
  name: DefaultInputString
  type: string
- description: ''
  name: DefaultLayoutString
  type: string
- description: ''
  name: StringMask
  type: string
- description: ''
  name: FromRightToLeftFlag
  type: boolean
- description: ''
  name: MaskCharactersFlag
  type: boolean
- description: ''
  name: BeepKeyFlag
  type: boolean
- description: ''
  name: GlobalCorrectionFlag
  type: boolean
- description: ''
  name: DisableCancelFlag
  type: boolean
- description: ''
  name: DisableCorrectFlag
  type: boolean
- description: ''
  name: DisableValidFlag
  type: boolean
- description: ''
  name: MenuBackFlag
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-input-data-schema.json
slug: terminal-input-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-input-data-schema.json\",\n  \"title\": \"InputData\",\n  \"description\": \"InputData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Device\": {\n      \"$ref\": \"#/components/schemas/Device\"\n    },\n    \"InfoQualify\": {\n      \"$ref\": \"#/components/schemas/InfoQualify\"\n    },\n    \"InputCommand\": {\n      \"$ref\": \"#/components/schemas/InputCommand\"\n    },\n    \"NotifyCardInputFlag\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"MaxInputTime\": {\n      \"type\": \"integer\"\n    },\n    \"ImmediateResponseFlag\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"MinLength\": {\n      \"type\": \"integer\"\n    },\n    \"MaxLength\": {\n      \"type\": \"integer\"\n    },\n    \"MaxDecimalLength\": {\n \
  \     \"type\": \"integer\"\n    },\n    \"WaitUserValidationFlag\": {\n      \"type\": \"boolean\",\n      \"default\": true\n    },\n    \"DefaultInputString\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"DefaultLayoutString\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"StringMask\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"FromRightToLeftFlag\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"MaskCharactersFlag\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"BeepKeyFlag\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"GlobalCorrectionFlag\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"DisableCancelFlag\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"DisableCorrectFlag\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"DisableValidFlag\"\
  : {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"MenuBackFlag\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    }\n  },\n  \"required\": [\n    \"Device\",\n    \"InfoQualify\",\n    \"InputCommand\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-input-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: InputData
---
