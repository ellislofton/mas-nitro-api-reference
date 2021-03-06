#ace_conf_file



Configuration for Ace Configuration File resource.

<span>(click to see [Operations](#operations))</span>



##Properties 

<span>(click to see [Operations](#operations))</span>





<table><thead><tr><th>Name</th><th>Data Type</th><th>Permissions</th><th>Description</th></tr></thead><tbody><tr><td>file_location_path</td><td>&lt;String></td><td>Read-write</td><td>File Location on Client for upload/download.<br>Minimum length = 1</td></tr><tr><td>file_name</td><td>&lt;String></td><td>Read-write</td><td>File Name.<br>Minimum length = 1<br>Maximum length = 256</td></tr><tr><td>is_main</td><td>&lt;Boolean></td><td>Read-write</td><td>File Location on Client for upload/download.</td></tr><tr><td>file_size</td><td>&lt;Integer></td><td>Read-only</td><td>File Size.</td></tr><tr><td>file_last_modified</td><td>&lt;String></td><td>Read-only</td><td>Last Modified.</td></tr></tbody></table>

##Operations 

<span>(click to see [Properties](#properties))</span>





[DELETE](#delete)| [GET (ALL)](#get-all)| [GET](#get)| [UPLOAD](#upload)| [DOWNLOAD](#download)





Some options that you can use for each operations:

<ul><li><p><b>Getting warnings in response:</b>NITRO allows you to get warnings in an operation by specifying the "warning" query parameter as "yes". For example, to get warnings while connecting to the NetScaler appliance, the URL is as follows:</p><p>http://<span style="color:green;font-style:italic;">&lt;netscaler-ip-address&gt;</span>/nitro/v1/config/login?warning=yes</p><p>If any, the warnings are displayed in the response payload with the HTTP code "209 X-NITRO-WARNING".</p></li><li><p><b>Authenticated access for individual NITRO operations:</b>NITRO allows you to logon to the NetScaler appliance to perform individual operations. You can use this option instead of creating a NITRO session (using the login object) and then using that session to perform all operations,</p><p>To do this, you must specify the username and password in the request header of the NITRO request as follows:</p><p>X-NITRO-USER:<span style="color:green;font-style:italic;">&lt;username&gt;</span></p><p>X-NITRO-PASS:<span style="color:green;font-style:italic;">&lt;password&gt;</span></p><p><b>Note: </b>In such cases, make sure that the request header DOES not include the following:</p><p>Cookie:NITRO_AUTH_TOKEN=<span style="color:green;font-style:italic;">&lt;tokenvalue&gt;</span></p></li></ul>







***Note: *** 

Mandatory parameters are marked in <span style="color:#FF0000;">red</span> and placeholder content is marked in <span style="color:green;font-style:italic">&lt;green&gt;</span>.



###delete







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/config/ace_conf_file/file_name_value&lt;String&gt;

<b>HTTP Method: </b>null

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done", "severity": ;ltString_value> }
```







###get (all)







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/config/ace_conf_file

<b>HTTP Method: </b>null

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done", "severity": ;ltString_value>, "ace_conf_file":[{
"file_location_path":<String_value>,
"file_size":<Integer_value>,
"file_name":<String_value>,
"file_last_modified":<String_value>,
"is_main":<Boolean_value>}]}
```







###get







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/config/ace_conf_file/file_name_value&lt;String&gt;

<b>HTTP Method: </b>null

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done", "severity": ;ltString_value>, "ace_conf_file":[{
"file_location_path":<String_value>,
"file_size":<Integer_value>,
"file_name":<String_value>,
"file_last_modified":<String_value>,
"is_main":<Boolean_value>}]}
```







###upload







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/upload/ace_conf_file

<b>HTTP Method: </b>null

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done }
```







###download







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/download/ace_conf_file/file_name_value&lt;String&gt;

<b>HTTP Method: </b>null







