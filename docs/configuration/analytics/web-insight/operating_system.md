#operating_system



Configuration for AF URL Report table resource.

<span>(click to see [Operations](#operations))</span>



##Properties 

<span>(click to see [Operations](#operations))</span>





<table><thead><tr><th>Name</th><th>Data Type</th><th>Permissions</th><th>Description</th></tr></thead><tbody><tr><td>__count</td><td>&lt;Double></td><td>Read-write</td><td>count..</td></tr><tr><td>cache_hits</td><td>&lt;Double></td><td>Read-write</td><td>Total requests to this APP for cache hits in given sampled timeframe..</td></tr><tr><td>http_content_type_name</td><td>&lt;String></td><td>Read-write</td><td>HTTP Content TYPE Name..<br>Maximum length = 256</td></tr><tr><td>total_bytes_cache_bypass</td><td>&lt;Double></td><td>Read-write</td><td>Cache Bypass total bytes accounted by this URL in sampled timeframe..</td></tr><tr><td>render_time</td><td>&lt;Double></td><td>Read-write</td><td>Render time..</td></tr><tr><td>ic_non_cache_hits</td><td>&lt;Double></td><td>Read-write</td><td>Total requests to this APP for cache bypass in given sampled timeframe..</td></tr><tr><td>id</td><td>&lt;String></td><td>Read-write</td><td>Id is HTTP Req URL..<br>Maximum length = 2000</td></tr><tr><td>total_bytes_cache_miss</td><td>&lt;Double></td><td>Read-write</td><td>Cache Miss total bytes accounted by this URL in sampled timeframe..</td></tr><tr><td>ic_miss</td><td>&lt;Double></td><td>Read-write</td><td>Total requests to this APP for cache miss in given sampled timeframe..</td></tr><tr><td>cache_miss</td><td>&lt;Double></td><td>Read-write</td><td>Total requests to this APP for cache miss in given sampled timeframe..</td></tr><tr><td>name</td><td>&lt;String></td><td>Read-write</td><td>Client Operating System Name..<br>Maximum length = 30</td></tr><tr><td>total_bytes</td><td>&lt;Double></td><td>Read-write</td><td>Total bytes accounted by this URL in sampled timeframe..</td></tr><tr><td>percent_bw_saved</td><td>&lt;Double></td><td>Read-write</td><td>Percentage of bw save to this APP in given sampled timeframe..</td></tr><tr><td>total_bytes_ic_hits</td><td>&lt;Double></td><td>Read-write</td><td>IC Cache Hits total bytes accounted by this URL in sampled timeframe..</td></tr><tr><td>total_bytes_cache_hits</td><td>&lt;Double></td><td>Read-write</td><td>Cache Hits total bytes accounted by this URL in sampled timeframe..</td></tr><tr><td>ic_no_store_reason</td><td>&lt;String></td><td>Read-write</td><td>ic_no_store_reason..<br>Maximum length = 256</td></tr><tr><td>max_transaction_time</td><td>&lt;Double></td><td>Read-write</td><td>Last Transaction Time for this URL in the sampled timeframe..</td></tr><tr><td>cache_bypass</td><td>&lt;Double></td><td>Read-write</td><td>Total requests to this APP for cache bypass in given sampled timeframe..</td></tr><tr><td>total_bytes_ic_miss</td><td>&lt;Double></td><td>Read-write</td><td>Cache Miss total bytes accounted by this URL in sampled timeframe..</td></tr><tr><td>ic_hits</td><td>&lt;Double></td><td>Read-write</td><td>Total requests to this APP for cache hits in given sampled timeframe..</td></tr><tr><td>total_bytes_ic_reval</td><td>&lt;Double></td><td>Read-write</td><td>Cache Reval total bytes accounted by this URL in sampled timeframe..</td></tr><tr><td>rpt_sample_time</td><td>&lt;Double></td><td>Read-write</td><td>Report Sample time..</td></tr><tr><td>ic_utilization</td><td>&lt;Double></td><td>Read-write</td><td>Total IC utilization in given sampled timeframe..</td></tr><tr><td>ic_reval</td><td>&lt;Double></td><td>Read-write</td><td>Total requests to this APP for cache bypass in given sampled timeframe..</td></tr><tr><td>total_requests</td><td>&lt;Double></td><td>Read-write</td><td>Count of this URL in given sampled timeframe..</td></tr><tr><td>http_media_type_name</td><td>&lt;String></td><td>Read-write</td><td>HTTP MEDIA TYPE Name..<br>Maximum length = 30</td></tr></tbody></table>

##Operations 

<span>(click to see [Properties](#properties))</span>





[GET (ALL)](#get-all)





Some options that you can use for each operations:

<ul><li><p><b>Getting warnings in response:</b>NITRO allows you to get warnings in an operation by specifying the "warning" query parameter as "yes". For example, to get warnings while connecting to the NetScaler appliance, the URL is as follows:</p><p>http://<span style="color:green;font-style:italic;">&lt;netscaler-ip-address&gt;</span>/nitro/v1/config/login?warning=yes</p><p>If any, the warnings are displayed in the response payload with the HTTP code "209 X-NITRO-WARNING".</p></li><li><p><b>Authenticated access for individual NITRO operations:</b>NITRO allows you to logon to the NetScaler appliance to perform individual operations. You can use this option instead of creating a NITRO session (using the login object) and then using that session to perform all operations,</p><p>To do this, you must specify the username and password in the request header of the NITRO request as follows:</p><p>X-NITRO-USER:<span style="color:green;font-style:italic;">&lt;username&gt;</span></p><p>X-NITRO-PASS:<span style="color:green;font-style:italic;">&lt;password&gt;</span></p><p><b>Note: </b>In such cases, make sure that the request header DOES not include the following:</p><p>Cookie:NITRO_AUTH_TOKEN=<span style="color:green;font-style:italic;">&lt;tokenvalue&gt;</span></p></li></ul>







***Note: *** 

Mandatory parameters are marked in <span style="color:#FF0000;">red</span> and placeholder content is marked in <span style="color:green;font-style:italic">&lt;green&gt;</span>.



###get (all)







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/config/operating_system

<b>HTTP Method: </b>null

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done", "severity": ;ltString_value>, "operating_system":[{
"__count":<Double_value>,
"cache_hits":<Double_value>,
"http_content_type_name":<String_value>,
"total_bytes_cache_bypass":<Double_value>,
"render_time":<Double_value>,
"ic_non_cache_hits":<Double_value>,
"id":<String_value>,
"total_bytes_cache_miss":<Double_value>,
"ic_miss":<Double_value>,
"vpn_user_name":<String_value>,
"cache_miss":<Double_value>,
"http_req_method_name":<String_value>,
"name":<String_value>,
"total_bytes":<Double_value>,
"user_agent_name":<String_value>,
"percent_bw_saved":<Double_value>,
"client_ip_address":<String_value>,
"total_bytes_ic_hits":<Double_value>,
"app_unit_ip_address":<String_value>,
"total_bytes_cache_hits":<Double_value>,
"ic_no_store_reason":<String_value>,
"http_resp_status_name":<String_value>,
"max_transaction_time":<Double_value>,
"uri_url":<String_value>,
"cache_bypass":<Double_value>,
"total_bytes_ic_miss":<Double_value>,
"app_unit_name":<String_value>,
"ic_hits":<Double_value>,
"server_ip_address":<String_value>,
"total_bytes_ic_reval":<Double_value>,
"rpt_sample_time":<Double_value>,
"device_ip_address":<String_value>,
"domain_name":<String_value>,
"ic_utilization":<Double_value>,
"ic_reval":<Double_value>,
"total_requests":<Double_value>,
"http_media_type_name":<String_value>}]}
```







