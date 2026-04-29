---
description: Snowflake account object.
layout: schema
name: Account
properties_list:
- description: Name of the organization.
  name: organization_name
  type: string
- description: Region group where the account is located. Note - This column is only displayed for organizations that span multiple region groups.
  name: region_group
  type: string
- description: 'Snowflake Region where the account is located. A Snowflake Region is a distinct location within a cloud platform region that is isolated from other Snowflake Regions. A Snowflake Region can be either '
  name: region
  type: string
- description: Snowflake Edition of the account.
  name: edition
  type: string
- description: Date and time the account was created.
  name: created_on
  type: string
- description: Preferred Snowflake account URL that includes the values of organization_name and account_name.
  name: account_url
  type: string
- description: System-assigned identifier of the acccount.
  name: account_locator
  type: string
- description: Legacy Snowflake account URL syntax that includes the region_name and account_locator.
  name: account_locator_url
  type: string
- description: Indicates how many managed accounts have been created by the account.
  name: managed_accounts
  type: integer
- description: Name of the consumption billing entity.
  name: consumption_billing_entity_name
  type: string
- description: Name of the marketplace consumer billing entity.
  name: marketplace_consumer_billing_entity_name
  type: string
- description: Name of the marketplace provider billing entity.
  name: marketplace_provider_billing_entity_name
  type: string
- description: If the original account URL was saved when the account was renamed, provides the original URL. If the original account URL was dropped, the value is NULL even if the account was renamed
  name: old_account_url
  type: string
- description: Optional comment in which to store information related to the account.
  name: comment
  type: string
- description: Indicates whether the ORGADMIN role is enabled in an account. If TRUE, the role is enabled.
  name: is_org_admin
  type: boolean
- description: Number of days that historical data is retained for Time Travel.
  name: retention_time
  type: integer
- description: Date and time the account was dropped.
  name: dropped_on
  type: string
- description: Date and time when the account is scheduled to be permanently deleted. Accounts are deleted within one hour after the scheduled time.
  name: scheduled_deletion_time
  type: string
- description: Date and time when the account was last restored.
  name: restored_on
  type: string
- description: If the original account URL was saved when the account was renamed, provides the date and time when the original account URL was saved.
  name: account_old_url_saved_on
  type: string
- description: If the original account URL was saved when the account was renamed, indicates the last time the account was accessed using the original URL.
  name: account_old_url_last_used
  type: string
- description: If the account’s organization was changed in a way that created a new account URL and the original account URL was saved, provides the original account URL. If the original account URL was dropped, th
  name: organization_old_url
  type: string
- description: If the account’s organization was changed in a way that created a new account URL and the original account URL was saved, provides the date and time when the original account URL was saved.
  name: organization_old_url_saved_on
  type: string
- description: If the account’s organization was changed in a way that created a new account URL and the original account URL was saved, indicates the last time the account was accessed using the original account UR
  name: organization_old_url_last_used
  type: string
- description: If the account’s organization was changed in a way that created a new account URL and the original account URL was saved, provides the date and time when the original account URL will be dropped. Drop
  name: organization_URL_expiration_on
  type: string
- description: Date and time when the account was moved to a different organization.
  name: moved_on
  type: string
- description: Indicates whether an account is an events account. For more information, see Set up logging and event sharing for an application.
  name: is_events_account
  type: boolean
- description: If the account was moved to a different organization, provides the name of that organization.
  name: moved_to_organization
  type: string
- description: Name of the account administrator.
  name: admin_name
  type: string
- description: Password for the account administrator.
  name: admin_password
  type: string
- description: RSA public key for the account administrator.
  name: admin_rsa_public_key
  type: string
- description: User type of the account administrator.
  name: admin_user_type
  type: string
- description: First name of the account administrator.
  name: first_name
  type: string
- description: Last name of the account administrator.
  name: last_name
  type: string
- description: Email address of the account administrator.
  name: email
  type: string
- description: Indicates whether the account administrator must change the password at the next login.
  name: must_change_password
  type: boolean
- description: Indicates whether the account is a Polaris account.
  name: polaris
  type: boolean
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/account-account-schema.json
slug: account-account
source_filename: account-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Account\",\n  \"type\": \"object\",\n  \"description\": \"Snowflake account object.\",\n  \"properties\": {\n    \"organization_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the organization.\"\n    },\n    \"region_group\": {\n      \"type\": \"string\",\n      \"description\": \"Region group where the account is located. Note - This column is only displayed for organizations that span multiple region groups.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Snowflake Region where the account is located. A Snowflake Region is a distinct location within a cloud platform region that is isolated from other Snowflake Regions. A Snowflake Region can be either multi-tenant or single-tenant (for a Virtual Private Snowflake account).\"\n    },\n    \"edition\": {\n      \"type\": \"string\",\n      \"description\": \"Snowflake Edition of\
  \ the account.\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time the account was created.\"\n    },\n    \"account_url\": {\n      \"type\": \"string\",\n      \"description\": \"Preferred Snowflake account URL that includes the values of organization_name and account_name.\"\n    },\n    \"account_locator\": {\n      \"type\": \"string\",\n      \"description\": \"System-assigned identifier of the acccount.\"\n    },\n    \"account_locator_url\": {\n      \"type\": \"string\",\n      \"description\": \"Legacy Snowflake account URL syntax that includes the region_name and account_locator.\"\n    },\n    \"managed_accounts\": {\n      \"type\": \"integer\",\n      \"description\": \"Indicates how many managed accounts have been created by the account.\"\n    },\n    \"consumption_billing_entity_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the consumption billing entity.\"\n    },\n    \"marketplace_consumer_billing_entity_name\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Name of the marketplace consumer billing entity.\"\n    },\n    \"marketplace_provider_billing_entity_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the marketplace provider billing entity.\"\n    },\n    \"old_account_url\": {\n      \"type\": \"string\",\n      \"description\": \"If the original account URL was saved when the account was renamed, provides the original URL. If the original account URL was dropped, the value is NULL even if the account was renamed\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Optional comment in which to store information related to the account.\"\n    },\n    \"is_org_admin\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the ORGADMIN role is enabled in an account. If TRUE, the role is enabled.\"\n    },\n    \"retention_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of days\
  \ that historical data is retained for Time Travel.\"\n    },\n    \"dropped_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time the account was dropped.\"\n    },\n    \"scheduled_deletion_time\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the account is scheduled to be permanently deleted. Accounts are deleted within one hour after the scheduled time.\"\n    },\n    \"restored_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the account was last restored.\"\n    },\n    \"account_old_url_saved_on\": {\n      \"type\": \"string\",\n      \"description\": \"If the original account URL was saved when the account was renamed, provides the date and time when the original account URL was saved.\"\n    },\n    \"account_old_url_last_used\": {\n      \"type\": \"string\",\n      \"description\": \"If the original account URL was saved when the account was renamed, indicates the last time the account was\
  \ accessed using the original URL.\"\n    },\n    \"organization_old_url\": {\n      \"type\": \"string\",\n      \"description\": \"If the account\\u2019s organization was changed in a way that created a new account URL and the original account URL was saved, provides the original account URL. If the original account URL was dropped, the value is NULL even if the organization changed.\"\n    },\n    \"organization_old_url_saved_on\": {\n      \"type\": \"string\",\n      \"description\": \"If the account\\u2019s organization was changed in a way that created a new account URL and the original account URL was saved, provides the date and time when the original account URL was saved.\"\n    },\n    \"organization_old_url_last_used\": {\n      \"type\": \"string\",\n      \"description\": \"If the account\\u2019s organization was changed in a way that created a new account URL and the original account URL was saved, indicates the last time the account was accessed using the original account\
  \ URL.\"\n    },\n    \"organization_URL_expiration_on\": {\n      \"type\": \"string\",\n      \"description\": \"If the account\\u2019s organization was changed in a way that created a new account URL and the original account URL was saved, provides the date and time when the original account URL will be dropped. Dropped URLs cannot be used to access the account.\"\n    },\n    \"moved_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the account was moved to a different organization.\"\n    },\n    \"is_events_account\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether an account is an events account. For more information, see Set up logging and event sharing for an application.\"\n    },\n    \"moved_to_organization\": {\n      \"type\": \"string\",\n      \"description\": \"If the account was moved to a different organization, provides the name of that organization.\"\n    },\n    \"admin_name\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Name of the account administrator.\"\n    },\n    \"admin_password\": {\n      \"type\": \"string\",\n      \"description\": \"Password for the account administrator.\"\n    },\n    \"admin_rsa_public_key\": {\n      \"type\": \"string\",\n      \"description\": \"RSA public key for the account administrator.\"\n    },\n    \"admin_user_type\": {\n      \"type\": \"string\",\n      \"description\": \"User type of the account administrator.\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"First name of the account administrator.\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the account administrator.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Email address of the account administrator.\"\n    },\n    \"must_change_password\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the account administrator must\
  \ change the password at the next login.\"\n    },\n    \"polaris\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the account is a Polaris account.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/account-account-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Account
---
