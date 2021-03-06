#servicepackage



Configuration for NetScaler Control Center allocates NetScaler instances according to the SLA that is defined as part this service package. resource.

<span>(click to see [Operations](#operations))</span>



##Properties 

<span>(click to see [Operations](#operations))</span>





<table><thead><tr><th>Name</th><th>Data Type</th><th>Permissions</th><th>Description</th></tr></thead><tbody><tr><td>name</td><td>&lt;String></td><td>Read-write</td><td>Name of service package..</td></tr><tr><td>cloudplatform_type</td><td>&lt;String></td><td>Read-write</td><td>Cloudplatform registered on MAS.</td></tr><tr><td>max_devices_to_autoprovision</td><td>&lt;String></td><td>Read-write</td><td>Maximum number of devices to autoprovision.</td></tr><tr><td>description</td><td>&lt;String></td><td>Read-write</td><td>Description for the service package.</td></tr><tr><td>isdefault</td><td>&lt;String></td><td>Read-write</td><td>Is this a default service package. Only one service package can be set as default service package. The default service package is used for allotment in any lb configuration that is not associated with any service package. Possible values - 'true', 'false'.</td></tr><tr><td>id</td><td>&lt;String></td><td>Read-write</td><td>Id is system generated key for service package.</td></tr><tr><td>allocationgroups</td><td>&lt;allocationgroup[]></td><td>Read-write</td><td>Device allocation policy for each device type.</td></tr><tr><td>tenantgroup</td><td>&lt;groupmember></td><td>Read-write</td><td>Tenant group of the tenants which are part of the service package.</td></tr></tbody></table>

##Operations 

<span>(click to see [Properties](#properties))</span>





[ADD](#add)| [DELETE](#delete)| [GET (ALL)](#get-all)| [GET](#get)| [UPDATE](#update)





Some options that you can use for each operations:

<ul><li><p><b>Getting warnings in response:</b>NITRO allows you to get warnings in an operation by specifying the "warning" query parameter as "yes". For example, to get warnings while connecting to the NetScaler appliance, the URL is as follows:</p><p>http://<span style="color:green;font-style:italic;">&lt;netscaler-ip-address&gt;</span>/nitro/v1/config/login?warning=yes</p><p>If any, the warnings are displayed in the response payload with the HTTP code "209 X-NITRO-WARNING".</p></li><li><p><b>Authenticated access for individual NITRO operations:</b>NITRO allows you to logon to the NetScaler appliance to perform individual operations. You can use this option instead of creating a NITRO session (using the login object) and then using that session to perform all operations,</p><p>To do this, you must specify the username and password in the request header of the NITRO request as follows:</p><p>X-NITRO-USER:<span style="color:green;font-style:italic;">&lt;username&gt;</span></p><p>X-NITRO-PASS:<span style="color:green;font-style:italic;">&lt;password&gt;</span></p><p><b>Note: </b>In such cases, make sure that the request header DOES not include the following:</p><p>Cookie:NITRO_AUTH_TOKEN=<span style="color:green;font-style:italic;">&lt;tokenvalue&gt;</span></p></li></ul>







***Note: *** 

Mandatory parameters are marked in <span style="color:#FF0000;">red</span> and placeholder content is marked in <span style="color:green;font-style:italic">&lt;green&gt;</span>.



###add







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/config/servicepackage?onerror=&lt;String_value&gt;

<b>HTTP Method: </b>null

<b>Request Payload: </b>
```
{servicepackage: {
"name":<String_value>,
"description":<String_value>,
"max_devices_to_autoprovision":<String_value>,
"cloudplatform_type":<String_value>,
"isdefault":<String_value>,
"id":<String_value>,
"allocationgroups":[{
"device_type":<String_value>,
"devicespec":<groupmember_value>,
"partitionspec":<groupmember_value>,
"placement_scheme":<String_value>,
"devicegroup":<groupmember_value>,
"device_allocation_type":<String_value>,
"allocationpolicy":<String_value>}],
"tenantgroup":<groupmember_value>}}
```

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done", "severity": ;ltString_value>, "servicepackage":[{
"name":<String_value>,
"cloudplatform_type":<String_value>,
"max_devices_to_autoprovision":<String_value>,
"description":<String_value>,
"isdefault":<String_value>,
"id":<String_value>,
"allocationgroups":[{
"partitionspec":<groupmember_value>,
"devicespec":<groupmember_value>,
"device_type":<String_value>,
"placement_scheme":<String_value>,
"devicegroup":<groupmember_value>,
"allocationpolicy":<String_value>,
"device_allocation_type":<String_value>}],
"tenantgroup":<groupmember_value>}]}
```







###delete







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/config/servicepackage/id_value&lt;String&gt;

<b>HTTP Method: </b>null

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done", "severity": ;ltString_value> }
```







###get (all)







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/config/servicepackage

<b>HTTP Method: </b>null

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done", "severity": ;ltString_value>, "servicepackage":[{
"name":<String_value>,
"cloudplatform_type":<String_value>,
"max_devices_to_autoprovision":<String_value>,
"description":<String_value>,
"isdefault":<String_value>,
"id":<String_value>,
"allocationgroups":[{
"partitionspec":<groupmember_value>,
"devicespec":<groupmember_value>,
"device_type":<String_value>,
"placement_scheme":<String_value>,
"devicegroup":<groupmember_value>,
"allocationpolicy":<String_value>,
"device_allocation_type":<String_value>}],
"tenantgroup":<groupmember_value>}]}
```







###get







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/config/servicepackage/id_value&lt;String&gt;

<b>HTTP Method: </b>null

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done", "severity": ;ltString_value>, "servicepackage":[{
"name":<String_value>,
"cloudplatform_type":<String_value>,
"max_devices_to_autoprovision":<String_value>,
"description":<String_value>,
"isdefault":<String_value>,
"id":<String_value>,
"allocationgroups":[{
"partitionspec":<groupmember_value>,
"devicespec":<groupmember_value>,
"device_type":<String_value>,
"placement_scheme":<String_value>,
"devicegroup":<groupmember_value>,
"allocationpolicy":<String_value>,
"device_allocation_type":<String_value>}],
"tenantgroup":<groupmember_value>}]}
```







###update







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/config/servicepackage/id_value&lt;String&gt;

<b>HTTP Method: </b>null

<b>Request Payload: </b>
```
{servicepackage:{
"name":<String_value>,
"description":<String_value>,
"max_devices_to_autoprovision":<String_value>,
"cloudplatform_type":<String_value>,
"isdefault":<String_value>,
"id":<String_value>,
"allocationgroups":[{
"device_type":<String_value>,
"devicespec":<groupmember_value>,
"partitionspec":<groupmember_value>,
"placement_scheme":<String_value>,
"devicegroup":<groupmember_value>,
"device_allocation_type":<String_value>,
"allocationpolicy":<String_value>}],
"tenantgroup":<groupmember_value>}}
```

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done", "severity": ;ltString_value>, "servicepackage":[{
"name":<String_value>,
"cloudplatform_type":<String_value>,
"max_devices_to_autoprovision":<String_value>,
"description":<String_value>,
"isdefault":<String_value>,
"id":<String_value>,
"allocationgroups":[{
"partitionspec":<groupmember_value>,
"devicespec":<groupmember_value>,
"device_type":<String_value>,
"placement_scheme":<String_value>,
"devicegroup":<groupmember_value>,
"allocationpolicy":<String_value>,
"device_allocation_type":<String_value>}],
"tenantgroup":<groupmember_value>}]}
```







