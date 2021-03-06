#perf_content_switching_report



Configuration for Content Switching resource.

<span>(click to see [Operations](#operations))</span>



##Properties 

<span>(click to see [Operations](#operations))</span>





<table><thead><tr><th>Name</th><th>Data Type</th><th>Permissions</th><th>Description</th></tr></thead><tbody><tr><td>establishedconn</td><td>&lt;Double></td><td>Read-write</td><td>establishedconn Value.</td></tr><tr><td>curclntconnections</td><td>&lt;Double></td><td>Read-write</td><td>curclntconnections Value.</td></tr><tr><td>totspillovers</td><td>&lt;Double></td><td>Read-write</td><td>totspillovers Value .</td></tr><tr><td>cursrvrconnections</td><td>&lt;Double></td><td>Read-write</td><td>cursrvrconnections Value .</td></tr><tr><td>device_ip_address</td><td>&lt;String></td><td>Read-write</td><td>Device IP Address.<br>Minimum length = 1<br>Maximum length = 64</td></tr><tr><td>vsvrName</td><td>&lt;String></td><td>Read-write</td><td>vsvrName Value .</td></tr><tr><td>timestamp</td><td>&lt;Double></td><td>Read-write</td><td>timestamp in milliseconds.</td></tr><tr><td>id</td><td>&lt;String></td><td>Read-write</td><td>Id is system generated key for all the entries in this perf table configuration.<br>Maximum length = 256</td></tr><tr><td>responsesrate</td><td>&lt;Double></td><td>Read-write</td><td>responsesrate Value.</td></tr><tr><td>requestsrate</td><td>&lt;Double></td><td>Read-write</td><td>requestsrate Value .</td></tr><tr><td>hitsrate</td><td>&lt;Double></td><td>Read-write</td><td>hitsrate Value.</td></tr><tr><td>report_start_time</td><td>&lt;Double></td><td>Read-write</td><td>report_start_time in seconds.</td></tr><tr><td>report_end_time</td><td>&lt;Double></td><td>Read-write</td><td>report_end_time in seconds.</td></tr></tbody></table>

##Operations 

<span>(click to see [Properties](#properties))</span>





[GET](#get)





Some options that you can use for each operations:

<ul><li><p><b>Getting warnings in response:</b>NITRO allows you to get warnings in an operation by specifying the "warning" query parameter as "yes". For example, to get warnings while connecting to the NetScaler appliance, the URL is as follows:</p><p>http://<span style="color:green;font-style:italic;">&lt;netscaler-ip-address&gt;</span>/nitro/v1/config/login?warning=yes</p><p>If any, the warnings are displayed in the response payload with the HTTP code "209 X-NITRO-WARNING".</p></li><li><p><b>Authenticated access for individual NITRO operations:</b>NITRO allows you to logon to the NetScaler appliance to perform individual operations. You can use this option instead of creating a NITRO session (using the login object) and then using that session to perform all operations,</p><p>To do this, you must specify the username and password in the request header of the NITRO request as follows:</p><p>X-NITRO-USER:<span style="color:green;font-style:italic;">&lt;username&gt;</span></p><p>X-NITRO-PASS:<span style="color:green;font-style:italic;">&lt;password&gt;</span></p><p><b>Note: </b>In such cases, make sure that the request header DOES not include the following:</p><p>Cookie:NITRO_AUTH_TOKEN=<span style="color:green;font-style:italic;">&lt;tokenvalue&gt;</span></p></li></ul>







***Note: *** 

Mandatory parameters are marked in <span style="color:#FF0000;">red</span> and placeholder content is marked in <span style="color:green;font-style:italic">&lt;green&gt;</span>.



###get







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/config/perf_content_switching_report

<b>HTTP Method: </b>null

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done", "severity": ;ltString_value>, "perf_content_switching_report":[{
"establishedconn":<Double_value>,
"curclntconnections":<Double_value>,
"totspillovers":<Double_value>,
"cursrvrconnections":<Double_value>,
"device_ip_address":<String_value>,
"vsvrName":<String_value>,
"timestamp":<Double_value>,
"id":<String_value>,
"responsesrate":<Double_value>,
"requestsrate":<Double_value>,
"hitsrate":<Double_value>,
"report_start_time":<Double_value>,
"report_end_time":<Double_value>}]}
```







