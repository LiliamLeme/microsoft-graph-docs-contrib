---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)

request_body = ExternalUsersSelfServiceSignUpEventsFlow(
	odata_type = "#microsoft.graph.externalUsersSelfServiceSignUpEventsFlow",
	display_name = "Woodgrove User Flow 2",
	on_authentication_method_load_start = OnAuthenticationMethodLoadStartExternalUsersSelfServiceSignUp(
		odata_type = "#microsoft.graph.onAuthenticationMethodLoadStartExternalUsersSelfServiceSignUp",
		identity_providers = [
			IdentityProviderBase(
				id = "EmailPassword-OAUTH",
			),
			IdentityProviderBase(
				id = "Google-OAUTH",
			),
			IdentityProviderBase(
				id = "Facebook-OAUTH",
			),
		],
	),
	on_interactive_auth_flow_start = OnInteractiveAuthFlowStartExternalUsersSelfServiceSignUp(
		odata_type = "#microsoft.graph.onInteractiveAuthFlowStartExternalUsersSelfServiceSignUp",
		is_sign_up_allowed = True,
	),
	on_attribute_collection = OnAttributeCollectionExternalUsersSelfServiceSignUp(
		odata_type = "#microsoft.graph.onAttributeCollectionExternalUsersSelfServiceSignUp",
		attributes = [
			IdentityUserFlowAttribute(
				id = "email",
				display_name = "Email Address",
				description = "Email address of the user",
				user_flow_attribute_type = IdentityUserFlowAttributeType.BuiltIn,
				data_type = IdentityUserFlowAttributeDataType.String,
			),
			IdentityUserFlowAttribute(
				id = "displayName",
				display_name = "Display Name",
				description = "Display Name of the User.",
				user_flow_attribute_type = IdentityUserFlowAttributeType.BuiltIn,
				data_type = IdentityUserFlowAttributeDataType.String,
			),
			IdentityUserFlowAttribute(
				id = "extension_6ea3bc85aec24b1c92ff4a117afb6621_Favoritecolor",
				display_name = "Favorite color",
				description = "what is your favorite color",
				user_flow_attribute_type = IdentityUserFlowAttributeType.Custom,
				data_type = IdentityUserFlowAttributeDataType.String,
			),
		],
		attribute_collection_page = AuthenticationAttributeCollectionPage(
			views = [
				AuthenticationAttributeCollectionPageViewConfiguration(
					inputs = [
						AuthenticationAttributeCollectionInputConfiguration(
							attribute = "email",
							label = "Email Address",
							input_type = AuthenticationAttributeCollectionInputType.Text,
							hidden = True,
							editable = False,
							write_to_directory = True,
							required = True,
							validation_reg_ex = "^[a-zA-Z0-9.!#$%&amp;&#8217;'*+/=?^_`{|}~-]+@[a-zA-Z0-9-]+(?:.[a-zA-Z0-9-]+)*$",
						),
						AuthenticationAttributeCollectionInputConfiguration(
							attribute = "displayName",
							label = "Display Name",
							input_type = AuthenticationAttributeCollectionInputType.Text,
							hidden = False,
							editable = True,
							write_to_directory = True,
							required = False,
							validation_reg_ex = "^[a-zA-Z_][0-9a-zA-Z_ ]*[0-9a-zA-Z_]+$",
						),
						AuthenticationAttributeCollectionInputConfiguration(
							attribute = "extension_6ea3bc85aec24b1c92ff4a117afb6621_Favoritecolor",
							label = "Favorite color",
							input_type = AuthenticationAttributeCollectionInputType.Text,
							hidden = False,
							editable = True,
							write_to_directory = True,
							required = False,
							validation_reg_ex = "^[a-zA-Z_][0-9a-zA-Z_ ]*[0-9a-zA-Z_]+$",
						),
					],
				),
			],
		),
	),
)

result = await graph_client.identity.authentication_events_flows.post(request_body)


```