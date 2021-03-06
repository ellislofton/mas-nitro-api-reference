#trap_forward_profile



Configuration for Trap Forward Profile resource.

<span>(click to see [Operations](#operations))</span>



##Properties 

<span>(click to see [Operations](#operations))</span>





<table><thead><tr><th>Name</th><th>Data Type</th><th>Permissions</th><th>Description</th></tr></thead><tbody><tr><td>trap_destination_port</td><td>&lt;String></td><td>Read-write</td><td>SNMP port to forward trap .<br>Minimum length = 1<br>Maximum length = 128</td></tr><tr><td>trap_community</td><td>&lt;String></td><td>Read-write</td><td>SNMP community..<br>Minimum length = 1<br>Maximum length = 128</td></tr><tr><td>id</td><td>&lt;String></td><td>Read-write</td><td>Id is system generated key for all the mail profile..</td></tr><tr><td>trap_destination</td><td>&lt;String></td><td>Read-write</td><td>SMTP server name.<br>Minimum length = 1<br>Maximum length = 128</td></tr><tr><td>profile_name</td><td>&lt;String></td><td>Read-write</td><td>Profile name for the mail setting..<br>Minimum length = 1<br>Maximum length = 128</td></tr><tr><td>tenant_id</td><td>&lt;String></td><td>Read-only</td><td>Tenant Id .</td></tr></tbody></table>

##Operations 

<span>(click to see [Properties](#properties))</span>





[ADD](#add)| [DELETE](#delete)| [GET (ALL)](#get-all)| [GET](#get)| [UPDATE](#update)





Some options that you can use for each operations:

<ul><li><p><b>Getting warnings in response:</b>NITRO allows you to get warnings in an operation by specifying the "warning" query parameter as "yes". For example, to get warnings while connecting to the NetScaler appliance, the URL is as follows:</p><p>http://<span style="color:green;font-style:italic;">&lt;netscaler-ip-address&gt;</span>/nitro/v1/config/login?warning=yes</p><p>If any, the warnings are displayed in the response payload with the HTTP code "209 X-NITRO-WARNING".</p></li><li><p><b>Authenticated access for individual NITRO operations:</b>NITRO allows you to logon to the NetScaler appliance to perform individual operations. You can use this option instead of creating a NITRO session (using the login object) and then using that session to perform all operations,</p><p>To do this, you must specify the username and password in the request header of the NITRO request as follows:</p><p>X-NITRO-USER:<span style="color:green;font-style:italic;">&lt;username&gt;</span></p><p>X-NITRO-PASS:<span style="color:green;font-style:italic;">&lt;password&gt;</span></p><p><b>Note: </b>In such cases, make sure that the request header DOES not include the following:</p><p>Cookie:NITRO_AUTH_TOKEN=<span style="color:green;font-style:italic;">&lt;tokenvalue&gt;</span></p></li></ul>







***Note: *** 

Mandatory parameters are marked in <span style="color:#FF0000;">red</span> and placeholder content is marked in <span style="color:green;font-style:italic">&lt;green&gt;</span>.



###add







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/config/trap_forward_profile?onerror=&lt;String_value&gt;

<b>HTTP Method: </b>null

<b>Request Payload: </b>
```
{trap_forward_profile: {
<b>"trap_destination_port":<String_value></b>,
<b>"trap_community":<String_value></b>,
<b>"trap_destination":<String_value></b>,
<b>"profile_name":<String_value></b>,
"id":<String_value>}}
```

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done", "severity": ;ltString_value>, "trap_forward_profile":[{
"trap_destination_port":<String_value>,
"tenant_id":<String_value>,
"trap_community":<String_value>,
"id":<String_value>,
"trap_destination":<String_value>,
"profile_name":<String_value>}]}
```







###delete







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/config/trap_forward_profile/id_value&lt;String&gt;

<b>HTTP Method: </b>null

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done", "severity": ;ltString_value> }
```







###get (all)







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/config/trap_forward_profile

<b>HTTP Method: </b>null

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done", "severity": ;ltString_value>, "trap_forward_profile":[{
"trap_destination_port":<String_value>,
"tenant_id":<String_value>,
"trap_community":<String_value>,
"id":<String_value>,
"trap_destination":<String_value>,
"profile_name":<String_value>}]}
```







###get







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/config/trap_forward_profile/id_value&lt;String&gt;

<b>HTTP Method: </b>null

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done", "severity": ;ltString_value>, "trap_forward_profile":[{
"trap_destination_port":<String_value>,
"tenant_id":<String_value>,
"trap_community":<String_value>,
"id":<String_value>,
"trap_destination":<String_value>,
"profile_name":<String_value>}]}
```







###update







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/config/trap_forward_profile/id_value&lt;String&gt;

<b>HTTP Method: </b>null

<b>Request Payload: </b>
```
{trap_forward_profile:{
<b>"id":<String_value></b>,
"trap_destination_port":<String_value>,
"trap_destination":<String_value>,
"trap_community":<String_value>,
"profile_name":<String_value>}}
```

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done", "severity": ;ltString_value>, "trap_forward_profile":[{
"trap_destination_port":<String_value>,
"tenant_id":<String_value>,
"trap_community":<String_value>,
"id":<String_value>,
"trap_destination":<String_value>,
"profile_name":<String_value>}]}
```







