#syslog_purge_setting_details



Configuration for Syslog Purge Setting Details resource.

<span>(click to see [Operations](#operations))</span>



##Properties 

<span>(click to see [Operations](#operations))</span>





<table><thead><tr><th>Name</th><th>Data Type</th><th>Permissions</th><th>Description</th></tr></thead><tbody><tr><td>syslog_detail_type_desc</td><td>&lt;String></td><td>Read-write</td><td>syslog groups.<br>Maximum length = 255</td></tr><tr><td>parent_name</td><td>&lt;String></td><td>Read-write</td><td>.</td></tr><tr><td>syslog_type</td><td>&lt;String></td><td>Read-write</td><td>syslog groups.<br>Maximum length = 255</td></tr><tr><td>syslog_module</td><td>&lt;String></td><td>Read-write</td><td>syslog modulename.<br>Maximum length = 255</td></tr><tr><td>id</td><td>&lt;String></td><td>Read-write</td><td>Id is system generated key for all the events.</td></tr><tr><td>syslog_detail_purge_interval</td><td>&lt;Integer></td><td>Read-write</td><td>Purge interval for syslog groups..</td></tr><tr><td>parent_id</td><td>&lt;String></td><td>Read-write</td><td>ID of syslog_purge_setting_details.</td></tr></tbody></table>

##Operations 

<span>(click to see [Properties](#properties))</span>





Some options that you can use for each operations:

<ul><li><p><b>Getting warnings in response:</b>NITRO allows you to get warnings in an operation by specifying the "warning" query parameter as "yes". For example, to get warnings while connecting to the NetScaler appliance, the URL is as follows:</p><p>http://<span style="color:green;font-style:italic;">&lt;netscaler-ip-address&gt;</span>/nitro/v1/config/login?warning=yes</p><p>If any, the warnings are displayed in the response payload with the HTTP code "209 X-NITRO-WARNING".</p></li><li><p><b>Authenticated access for individual NITRO operations:</b>NITRO allows you to logon to the NetScaler appliance to perform individual operations. You can use this option instead of creating a NITRO session (using the login object) and then using that session to perform all operations,</p><p>To do this, you must specify the username and password in the request header of the NITRO request as follows:</p><p>X-NITRO-USER:<span style="color:green;font-style:italic;">&lt;username&gt;</span></p><p>X-NITRO-PASS:<span style="color:green;font-style:italic;">&lt;password&gt;</span></p><p><b>Note: </b>In such cases, make sure that the request header DOES not include the following:</p><p>Cookie:NITRO_AUTH_TOKEN=<span style="color:green;font-style:italic;">&lt;tokenvalue&gt;</span></p></li></ul>







***Note: *** 

Mandatory parameters are marked in <span style="color:#FF0000;">red</span> and placeholder content is marked in <span style="color:green;font-style:italic">&lt;green&gt;</span>.



