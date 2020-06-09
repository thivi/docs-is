# Enable Login for a Custom Web Application

WSO2 Identity Server provides a way to decouple authentication functionality from the standard authentication
protocols such as OAuth 2.0, OpenID Connect, SAML 2.0 and WS-Federation, etc. 

In this approach, the logic for processing an inbound authentication request will be written as an OSGi component (pluggable Java artifacts) called an inbound authenticator.
When you need to integrate an application which is not written based on a standard protocol, you can write a custom inbound authenticator and plug with WSO2 Identity Server.

---

This guide assumes you have your own web application and a custom inbound authenticator. If you wish to try out this flow with a sample application, click the button below. 

<a class="samplebtn_a" href="../../../quick-starts/webapp-custom-sample" rel="nofollow noopener">Try it with the sample</a>

----
{!fragments/deploying-sample-apps.md!}

----

## Deploy the inbound authenticator

- Copy the authenticator to dropins directory (i.e. /repository/components/dropins)

----

{!fragments/register-a-service-provider.md!}
4. Expand 'Inbound Authentication Configuration' and select relevant configurations based on the sample authenticator deployed.

----

!!! info "Related Topics"
    - [Enable Login for a Sample Custom Web Application](../../../quick-starts/webapp-custom-sample)
    - [Write a Custom Inbound Protocol](inserlink)