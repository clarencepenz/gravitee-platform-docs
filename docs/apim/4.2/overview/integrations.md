---
description: >-
  Learn more about how Gravitee integrates with your larger enterprise tech
  ecosystem
---

# Integrations

The below sections and tables outline major integrations that Gravitee API Management (APIM) offers with other enterprise tooling.

## Event brokers

<table><thead><tr><th width="144">Event broker</th><th>Integration description</th><th>Plugin or add-on required</th></tr></thead><tbody><tr><td>Kafka</td><td>Gravitee can expose backend Kafka data sources as <a href="../guides/create-apis/how-to/">supported client-side APIs.</a></td><td>Gateway Kafka Endpoint connector</td></tr><tr><td>Confluent</td><td>Gravitee can expose backend Confluent data sources as <a href="../guides/create-apis/how-to/">supported client-side APIs.</a> Gravitee also supports Confluent Schema registry as schema validation resource.</td><td>Gateway Kafka Endpoint connector<br><br>Various serialization and deserialization policies</td></tr><tr><td>Solace</td><td>Gravitee can expose backend Solace event APIs as <a href="../guides/create-apis/how-to/">supported client-side APIs.</a> Gravitee can also auto-import Solace event APIs.</td><td>Management Solace Sync Service plugin<br><br>Gateway Solace Endpoint Connector</td></tr><tr><td>HiveMQ</td><td>Gravitee can expose backend MQTT data sources as <a href="../guides/create-apis/how-to/">supported client-side APIs.</a></td><td>Gateway MQTT Endpoint Connector</td></tr><tr><td>Mosquito</td><td>Gravitee can expose backend MQTT data sources as <a href="../guides/create-apis/how-to/">supported client-side APIs.</a></td><td>Gateway MQTT Endpoint Connector</td></tr><tr><td>(Other MQTT broker running MQTT 5)</td><td>Gravitee can expose backend MQTT data sources as <a href="../guides/create-apis/how-to/">supported client-side APIs.</a></td><td>Gateway MQTT Endpoint Connector</td></tr></tbody></table>

## APM and Observability

<table><thead><tr><th width="144">Monitoring solution</th><th>Integration description</th><th>Plugin or add-on required</th></tr></thead><tbody><tr><td>Splunk</td><td>Gravitee can push API metrics and monitoring data to Splunk for visualization in Splunk dashboards.</td><td>File reporter plugin</td></tr><tr><td>Datadog</td><td>Gravitee can push API metrics and monitoring data to Datadog for visualization in Datadog dashboards.</td><td>Datadog reporter plugin<br><br>File reporter plugin (less advanced version)</td></tr><tr><td>Dynatrace</td><td>Gravitee can push API metrics and monitoring data to Dynatrace for visualization in Dynatrace dashboards.</td><td>File reporter plugin</td></tr></tbody></table>

## Service Discovery

<table><thead><tr><th width="144">Solution</th><th>Integration description</th><th>Plugin or add-on required</th></tr></thead><tbody><tr><td><a href="../guides/api-configuration/v2-api-configuration/configure-service-discovery.md">HashiCorp Consul</a></td><td>Bind the backend endpoints of your API to a service managed by HashiCorp Consul so that API requests are always routed to the proper, healthy backend service dynamically managed by HashiCorp Consul.</td><td>Gravitee service discovery consul plugin</td></tr></tbody></table>

## API documentation

<table><thead><tr><th width="144">Solution</th><th>Integration description</th><th>Plugin or add-on required</th></tr></thead><tbody><tr><td>Bitbucket</td><td>Fetch content from a Bitbucket repository. It’s primarily used to fetch documentation.</td><td>Bitbucket fetcher plugin</td></tr><tr><td>Git</td><td>Fetch content from a Git repository. It’s primarily used to fetch documentation.</td><td>GIT fetcher plugin</td></tr><tr><td>GitHub</td><td>Fetch content from a GitHub repository. It’s primarily used to fetch documentation.</td><td>GitHub fetcher plugin</td></tr><tr><td>GitLab</td><td>Fetch content from a GitLab repository. It’s primarily used to fetch documentation.</td><td>GitLab fetcher plugin</td></tr></tbody></table>

## Authentication and Authorization

<table><thead><tr><th width="222">Solution</th><th>Integration description</th><th>Plugin or add-on required</th></tr></thead><tbody><tr><td>Gravitee Access Management</td><td>A Gravitee Access Management resource is defined to introspect an access_token generated by a Gravitee Access Management instance.</td><td>Gravitee.io Access Management Resource plugin</td></tr><tr><td>Keycloak</td><td>A Keycloak adapter resource is defined to introspect an access token provided by Keycloak.</td><td>keycloak Adapter Resource plugin</td></tr><tr><td>OAuth2 authorization servers</td><td>A Generic OAuth2 Authorization Server resource is defined to introspect an access_token generated by a generic OAuth2 authorization server.</td><td>Generic OAuth2 Authorization Server Resource</td></tr><tr><td>LDAP authentication provider</td><td>A Gravitee LDAP Authentication Provider resource is used to validate a user’s credentials against an LDAP server.</td><td>LDAP Authentication Provider plugin</td></tr><tr><td>HTTP Authentication provider</td><td>You can set up an HTTP authentication provider resource.</td><td>HTTP Authentication Provider plugin</td></tr><tr><td>Inline authentication</td><td>You can set up an inline authentication provider resource (i.e. you can bring your own users)</td><td>Inline Authentication Provider plugin</td></tr></tbody></table>

## Cache

<table><thead><tr><th width="144">Solution</th><th>Integration description</th><th>Plugin or add-on required</th></tr></thead><tbody><tr><td>Redis</td><td>The Redis cache resource is used to maintain a cache and link it to the API lifecycle. It means that the cache is initialized when the API is starting and released when API is stopped.</td><td>Redis Cache Resource plugin</td></tr><tr><td>In-memory cache solution</td><td>The cache resource is used to maintain a cache and link it to the API lifecycle. The cache will be initialized when the API is starting and released when API is stopped. This cache is responsible for storing HTTP responses from the backend to avoid subsequent calls.</td><td>Cache resource</td></tr></tbody></table>

## Custom backend integrations

Gravitee's flexible API and protocol support enables you to integrate Gravitee with any backend system that can communicate over:

* SOAP
* REST
* WebSocket
* gRPC

{% hint style="info" %}
**For example: Salesforce**

Gravitee can be used for some custom Salesforce integration use cases, as Salesforce provides streaming APIs. For more information on how to use Gravitee for these use cases, we recommend [booking a demo with one of our Solutions Engineers](https://www.gravitee.io/demo).
{% endhint %}
