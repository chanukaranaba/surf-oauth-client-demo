# surf-oauth-client-demo
Using WSO2 API Manager store with Surf OAuth as the key manager


Open api-manager.xml located in <APIM_HOME>/repository/conf folder, uncomment <APIKeyManager> element and configure it as explained below.

 ` ` ` 
<APIKeyManager>
  <KeyManagerClientImpl>nl.surfnet.demo.SurfOAuthClient</KeyManagerClientImpl>
  <Configuration>    
    <RegistrationEndpoint>http://localhost:8080/admin/resourceServer/251/client</RegistrationEndpoint>
    <AccessToken>661ee1c7-e134-437e-90e5-ebe741ecd669</AccessToken>
    <IntrospectionURL>http://localhost:8080/v1/tokeninfo</IntrospectionURL>
    <ConsumerKey>aa693e15-3be5-4aae-bc75-2313c48d0860</ConsumerKey>
    <ConsumerSecret>825ba61c-4a4d-42f8-9942-b2dc9fc8a3fd</ConsumerSecret>
    <TokenEndpoint>http://localhost:8080/v1/token</TokenEndpoint>
  </Configuration>
</APIKeyManager>
 ` ` ` 
