---
description: "Automatically generated file. DO NOT MODIFY"
---

```python



graph_client = GraphServiceClient(credentials, scopes)


await graph_client.identity.authentication_events_flows.by_authentication_events_flow_id('authenticationEventsFlow-id').graph_external_users_self_service_sign_up_events_flow.on_authentication_method_load_start.graph_on_authentication_method_load_start_external_users_self_service_sign_up.identity_providers.by_identity_provider_base_id('identityProviderBase-id').ref.delete()


```