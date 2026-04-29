---
description: 'It is the relation of the add-on client with the primary client. <BR/> **Conditional Mandatory**<font color=''red''>* </font> field - Add-on ''client code'' and relation fields are mutually exclusive while creating the client. If both present, then relation value will be ignored. <br/> Valid values are configured on ''Card Management > Institution Parameter Setup > System Codes [ISSS15]'' screen for "Type Id=RELATION". <br/> **Few sample values: ** `Brother`, `Business card`, `Daughter`, `Father`, `Father-in-Law`, `Mother`, `Mother in Law`, `Others`, `Sister`, `Son`, `Spouse`'
layout: schema
name: Relation
properties_list: []
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-relation-schema.json
slug: mastercard-card-issuance-relation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Relation\",\n  \"type\": \"string\",\n  \"description\": \"It is the relation of the add-on client with the primary client. <BR/> **Conditional Mandatory**<font color='red'>* </font> field - Add-on 'client code' and relation fields are mutually exclusive while creating the client. If both present, then relation value will be ignored. <br/> Valid values are configured on 'Card Management > Institution Parameter Setup > System Codes [ISSS15]'     screen for \\\"Type Id=RELATION\\\". <br/> **Few sample values: ** `Brother`, `Business card`, `Daughter`, `Father`, `Father-in-Law`, `Mother`, `Mother in Law`, `Others`, `Sister`, `Son`, `Spouse`\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-relation-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Relation
---
