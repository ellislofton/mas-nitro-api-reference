#aaa_server



Configuration for AAA Server configuration resource.

<span>(click to see [Operations](#operations))</span>



##Properties 

<span>(click to see [Operations](#operations))</span>





<table><thead><tr><th>Name</th><th>Data Type</th><th>Permissions</th><th>Description</th></tr></thead><tbody><tr><td>external_servers</td><td>&lt;external_server[]></td><td>Read-write</td><td>List of external servers.</td></tr><tr><td>fallback_local_authentication</td><td>&lt;Boolean></td><td>Read-write</td><td>Enable local fallback authentication.</td></tr><tr><td>primary_server_name</td><td>&lt;String></td><td>Read-write</td><td>Name of primary server name.<br>Minimum length = 1<br>Maximum length = 128</td></tr><tr><td>id</td><td>&lt;String></td><td>Read-write</td><td>Id is system generated key for all the servers.</td></tr><tr><td>primary_server_type</td><td>&lt;String></td><td>Read-write</td><td>Type of primary server. Supported types 1. LOCAL 2.RADIUS 3.LDAP 4.TACACS 5.KEYSTONE.<br>Minimum length = 1<br>Maximum length = 32</td></tr></tbody></table>

##Operations 

<span>(click to see [Properties](#properties))</span>





[GET (ALL)](#get-all)| [GET](#get)| [UPDATE](#update)





Some options that you can use for each operations:

<ul><li><p><b>Getting warnings in response:</b>NITRO allows you to get warnings in an operation by specifying the "warning" query parameter as "yes". For example, to get warnings while connecting to the NetScaler appliance, the URL is as follows:</p><p>http://<span style="color:green;font-style:italic;">&lt;netscaler-ip-address&gt;</span>/nitro/v1/config/login?warning=yes</p><p>If any, the warnings are displayed in the response payload with the HTTP code "209 X-NITRO-WARNING".</p></li><li><p><b>Authenticated access for individual NITRO operations:</b>NITRO allows you to logon to the NetScaler appliance to perform individual operations. You can use this option instead of creating a NITRO session (using the login object) and then using that session to perform all operations,</p><p>To do this, you must specify the username and password in the request header of the NITRO request as follows:</p><p>X-NITRO-USER:<span style="color:green;font-style:italic;">&lt;username&gt;</span></p><p>X-NITRO-PASS:<span style="color:green;font-style:italic;">&lt;password&gt;</span></p><p><b>Note: </b>In such cases, make sure that the request header DOES not include the following:</p><p>Cookie:NITRO_AUTH_TOKEN=<span style="color:green;font-style:italic;">&lt;tokenvalue&gt;</span></p></li></ul>







***Note: *** 

Mandatory parameters are marked in <span style="color:#FF0000;">red</span> and placeholder content is marked in <span style="color:green;font-style:italic">&lt;green&gt;</span>.



###get (all)







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/config/aaa_server

<b>HTTP Method: </b>null

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done", "severity": ;ltString_value>, "aaa_server":[{
"external_servers":[{
"priority":<Integer_value>,
"parent_name":<String_value>,
"external_server_type":<String_value>,
"external_server_name":<String_value>,
"id":<String_value>,
"parent_id":<String_value>}],
"secondary_server_name":<String_value>,
"fallback_local_authentication":<Boolean_value>,
"enable_secondary_server":<Boolean_value>,
"primary_server_name":<String_value>,
"id":<String_value>,
"secondary_server_type":<String_value>,
"primary_server_type":<String_value>}]}
```







###get







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/config/aaa_server/id_value&lt;String&gt;

<b>HTTP Method: </b>null

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done", "severity": ;ltString_value>, "aaa_server":[{
"external_servers":[{
"priority":<Integer_value>,
"parent_name":<String_value>,
"external_server_type":<String_value>,
"external_server_name":<String_value>,
"id":<String_value>,
"parent_id":<String_value>}],
"secondary_server_name":<String_value>,
"fallback_local_authentication":<Boolean_value>,
"enable_secondary_server":<Boolean_value>,
"primary_server_name":<String_value>,
"id":<String_value>,
"secondary_server_type":<String_value>,
"primary_server_type":<String_value>}]}
```







###update







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/config/aaa_server/id_value&lt;String&gt;

<b>HTTP Method: </b>null

<b>Request Payload: </b>
```
{aaa_server:{
<b>"primary_server_type":<String_value></b>,
"external_servers":[{
"priority":<Integer_value>,
"parent_id":<String_value>,
"id":<String_value>,
"parent_name":<String_value>,
"external_server_name":<String_value>,
"external_server_type":<String_value>}],
"id":<String_value>,
"fallback_local_authentication":<Boolean_value>,
"primary_server_name":<String_value>}}
```

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done", "severity": ;ltString_value>, "aaa_server":[{
"external_servers":[{
"priority":<Integer_value>,
"parent_name":<String_value>,
"external_server_type":<String_value>,
"external_server_name":<String_value>,
"id":<String_value>,
"parent_id":<String_value>}],
"secondary_server_name":<String_value>,
"fallback_local_authentication":<Boolean_value>,
"enable_secondary_server":<Boolean_value>,
"primary_server_name":<String_value>,
"id":<String_value>,
"secondary_server_type":<String_value>,
"primary_server_type":<String_value>}]}
```







