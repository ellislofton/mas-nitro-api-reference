#si_safety_security_check



Configuration for AF Safety Data Report table resource.

<span>(click to see [Operations](#operations))</span>



##Properties 

<span>(click to see [Operations](#operations))</span>





<table><thead><tr><th>Name</th><th>Data Type</th><th>Permissions</th><th>Description</th></tr></thead><tbody><tr><td>profile_stat</td><td>&lt;Double></td><td>Read-write</td><td>profile_stat..</td></tr><tr><td>profile_check_safety_index</td><td>&lt;Double></td><td>Read-write</td><td>profile_check_safety_index..</td></tr><tr><td>__count</td><td>&lt;Double></td><td>Read-write</td><td>count..</td></tr><tr><td>profile_log</td><td>&lt;Double></td><td>Read-write</td><td>profile_log..</td></tr><tr><td>profile_none</td><td>&lt;Double></td><td>Read-write</td><td>profile_none..</td></tr><tr><td>profile_block</td><td>&lt;Double></td><td>Read-write</td><td>profile_block..</td></tr><tr><td>configuration</td><td>&lt;String></td><td>Read-write</td><td>Profile Security configuration.<br>Maximum length = 255</td></tr><tr><td>id</td><td>&lt;String></td><td>Read-write</td><td>Id is safety profile.<br>Maximum length = 255</td></tr><tr><td>si_safety_profile_name</td><td>&lt;String></td><td>Read-write</td><td>Profile Name.<br>Maximum length = 255</td></tr><tr><td>profile_block_count</td><td>&lt;Double></td><td>Read-write</td><td>profile_block_count..</td></tr><tr><td>name</td><td>&lt;String></td><td>Read-write</td><td>Profile Security Check Type Name.<br>Maximum length = 255</td></tr><tr><td>profile_not_block_count</td><td>&lt;Double></td><td>Read-write</td><td>profile_not_block_count..</td></tr><tr><td>profile_learn</td><td>&lt;Double></td><td>Read-write</td><td>profile_learn..</td></tr><tr><td>profile_none_count</td><td>&lt;Double></td><td>Read-write</td><td>profile_none_count..</td></tr><tr><td>si_app_unit_name</td><td>&lt;String></td><td>Read-write</td><td>AppName.<br>Maximum length = 255</td></tr><tr><td>profile_safety_index</td><td>&lt;Double></td><td>Read-write</td><td>profile_safety_index..</td></tr></tbody></table>

##Operations 

<span>(click to see [Properties](#properties))</span>





[GET (ALL)](#get-all)





Some options that you can use for each operations:

<ul><li><p><b>Getting warnings in response:</b>NITRO allows you to get warnings in an operation by specifying the "warning" query parameter as "yes". For example, to get warnings while connecting to the NetScaler appliance, the URL is as follows:</p><p>http://<span style="color:green;font-style:italic;">&lt;netscaler-ip-address&gt;</span>/nitro/v1/config/login?warning=yes</p><p>If any, the warnings are displayed in the response payload with the HTTP code "209 X-NITRO-WARNING".</p></li><li><p><b>Authenticated access for individual NITRO operations:</b>NITRO allows you to logon to the NetScaler appliance to perform individual operations. You can use this option instead of creating a NITRO session (using the login object) and then using that session to perform all operations,</p><p>To do this, you must specify the username and password in the request header of the NITRO request as follows:</p><p>X-NITRO-USER:<span style="color:green;font-style:italic;">&lt;username&gt;</span></p><p>X-NITRO-PASS:<span style="color:green;font-style:italic;">&lt;password&gt;</span></p><p><b>Note: </b>In such cases, make sure that the request header DOES not include the following:</p><p>Cookie:NITRO_AUTH_TOKEN=<span style="color:green;font-style:italic;">&lt;tokenvalue&gt;</span></p></li></ul>







***Note: *** 

Mandatory parameters are marked in <span style="color:#FF0000;">red</span> and placeholder content is marked in <span style="color:green;font-style:italic">&lt;green&gt;</span>.



###get (all)







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/config/si_safety_security_check

<b>HTTP Method: </b>null

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done", "severity": ;ltString_value>, "si_safety_security_check":[{
"profile_stat":<Double_value>,
"profile_check_safety_index":<Double_value>,
"__count":<Double_value>,
"profile_log":<Double_value>,
"profile_none":<Double_value>,
"profile_block":<Double_value>,
"configuration":<String_value>,
"id":<String_value>,
"si_safety_profile_name":<String_value>,
"profile_block_count":<Double_value>,
"name":<String_value>,
"profile_not_block_count":<Double_value>,
"profile_learn":<Double_value>,
"profile_none_count":<Double_value>,
"si_device_ip_address":<String_value>,
"si_app_unit_name":<String_value>,
"profile_safety_index":<Double_value>}]}
```







