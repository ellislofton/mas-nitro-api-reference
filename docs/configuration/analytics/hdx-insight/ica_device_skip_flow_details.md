#ica_device_skip_flow_details



Configuration for Af report for ICA Device Skip flow details resource.

<span>(click to see [Operations](#operations))</span>



##Properties 

<span>(click to see [Operations](#operations))</span>





<table><thead><tr><th>Name</th><th>Data Type</th><th>Permissions</th><th>Description</th></tr></thead><tbody><tr><td>serverside_packet_retransmits</td><td>&lt;Double></td><td>Read-write</td><td>Server side packet retransmits..</td></tr><tr><td>__count</td><td>&lt;Double></td><td>Read-write</td><td>count..</td></tr><tr><td>state</td><td>&lt;String></td><td>Read-write</td><td>ICA Session state..</td></tr><tr><td>skipflow_reason_id</td><td>&lt;Double></td><td>Read-write</td><td>Skip flow reason id..</td></tr><tr><td>launch_duration</td><td>&lt;Double></td><td>Read-write</td><td>ica session launch duration..</td></tr><tr><td>server_jitter</td><td>&lt;Double></td><td>Read-write</td><td>ICA User server jitter..</td></tr><tr><td>client_jitter</td><td>&lt;Double></td><td>Read-write</td><td>ICA User client jitter..</td></tr><tr><td>id</td><td>&lt;String></td><td>Read-write</td><td>Id is ICA Session ID.<br>Minimum length = 1<br>Maximum length = 64</td></tr><tr><td>serverside_0_win</td><td>&lt;Double></td><td>Read-write</td><td>server side 0 window count..</td></tr><tr><td>server_latency</td><td>&lt;Double></td><td>Read-write</td><td>ica session server latency..</td></tr><tr><td>host_delay</td><td>&lt;Double></td><td>Read-write</td><td>Server induced delay..</td></tr><tr><td>total_bytes</td><td>&lt;Double></td><td>Read-write</td><td>Total bytes accounted by this URL in sampled timeframe..</td></tr><tr><td>pn_agent_version</td><td>&lt;String></td><td>Read-write</td><td>Name of ICA session pn agent version.<br>Minimum length = 1<br>Maximum length = 128</td></tr><tr><td>client_latency</td><td>&lt;Double></td><td>Read-write</td><td>ica session client latency..</td></tr><tr><td>client_srtt</td><td>&lt;Double></td><td>Read-write</td><td>client Smothen RTT..</td></tr><tr><td>client_side_ns_delay</td><td>&lt;Double></td><td>Read-write</td><td>Clinet to Server NS delay..</td></tr><tr><td>server_side_ns_delay</td><td>&lt;Double></td><td>Read-write</td><td>Server to Clinet NS delay..</td></tr><tr><td>group_reason_id</td><td>&lt;Double></td><td>Read-write</td><td>Skip flow group reason id..</td></tr><tr><td>receiver_version</td><td>&lt;String></td><td>Read-write</td><td>Name of ICA session receiver version.<br>Minimum length = 1<br>Maximum length = 128</td></tr><tr><td>application_enumeration_duration</td><td>&lt;Double></td><td>Read-write</td><td>Time taken for app enumeration to launch..</td></tr><tr><td>session_reconnect</td><td>&lt;Double></td><td>Read-write</td><td>Session reconnect..</td></tr><tr><td>serverside_rto</td><td>&lt;Double></td><td>Read-write</td><td>serverside rto..</td></tr><tr><td>skipflow_description</td><td>&lt;String></td><td>Read-write</td><td>Reason for skip flow..<br>Minimum length = 1<br>Maximum length = 128</td></tr><tr><td>up_time</td><td>&lt;Double></td><td>Read-write</td><td>ica session up time..</td></tr><tr><td>client_tx_bytes</td><td>&lt;Double></td><td>Read-write</td><td>Client Side Tx bytes..</td></tr><tr><td>clientside_packet_retransmits</td><td>&lt;Double></td><td>Read-write</td><td>Client side packet retransmits..</td></tr><tr><td>rpt_sample_time</td><td>&lt;Double></td><td>Read-write</td><td>Report Sample time..</td></tr><tr><td>clientside_0_win</td><td>&lt;Double></td><td>Read-write</td><td>Client side 0 window count..</td></tr><tr><td>client_rx_bytes</td><td>&lt;Double></td><td>Read-write</td><td>Client Side Rx bytes..</td></tr><tr><td>session_setup_time</td><td>&lt;Double></td><td>Read-write</td><td>ICA Session setup time..</td></tr><tr><td>bandwidth</td><td>&lt;Double></td><td>Read-write</td><td>Avg Bandwidth..</td></tr><tr><td>clientside_rto</td><td>&lt;Double></td><td>Read-write</td><td>clientside rto..</td></tr><tr><td>server_srtt</td><td>&lt;Double></td><td>Read-write</td><td>server Smothen RTT..</td></tr><tr><td>skipflow_count</td><td>&lt;Double></td><td>Read-write</td><td>Skip flow count...</td></tr><tr><td>session_rtt</td><td>&lt;Double></td><td>Read-write</td><td>ICA Session rtt..</td></tr><tr><td>session_end_time</td><td>&lt;Double></td><td>Read-write</td><td>ICA Session end time..</td></tr></tbody></table>

##Operations 

<span>(click to see [Properties](#properties))</span>





[GET (ALL)](#get-all)





Some options that you can use for each operations:

<ul><li><p><b>Getting warnings in response:</b>NITRO allows you to get warnings in an operation by specifying the "warning" query parameter as "yes". For example, to get warnings while connecting to the NetScaler appliance, the URL is as follows:</p><p>http://<span style="color:green;font-style:italic;">&lt;netscaler-ip-address&gt;</span>/nitro/v1/config/login?warning=yes</p><p>If any, the warnings are displayed in the response payload with the HTTP code "209 X-NITRO-WARNING".</p></li><li><p><b>Authenticated access for individual NITRO operations:</b>NITRO allows you to logon to the NetScaler appliance to perform individual operations. You can use this option instead of creating a NITRO session (using the login object) and then using that session to perform all operations,</p><p>To do this, you must specify the username and password in the request header of the NITRO request as follows:</p><p>X-NITRO-USER:<span style="color:green;font-style:italic;">&lt;username&gt;</span></p><p>X-NITRO-PASS:<span style="color:green;font-style:italic;">&lt;password&gt;</span></p><p><b>Note: </b>In such cases, make sure that the request header DOES not include the following:</p><p>Cookie:NITRO_AUTH_TOKEN=<span style="color:green;font-style:italic;">&lt;tokenvalue&gt;</span></p></li></ul>







***Note: *** 

Mandatory parameters are marked in <span style="color:#FF0000;">red</span> and placeholder content is marked in <span style="color:green;font-style:italic">&lt;green&gt;</span>.



###get (all)







<b>URL: </b>https://&lt;MGMT-IP&gt;/nitro/v1/config/ica_device_skip_flow_details

<b>HTTP Method: </b>null

<b>Response Payload: </b>
```
{ "errorcode": 0, "message": "Done", "severity": ;ltString_value>, "ica_device_skip_flow_details":[{
"serverside_packet_retransmits":<Double_value>,
"ica_user_name":<String_value>,
"__count":<Double_value>,
"state":<String_value>,
"skipflow_reason_id":<Double_value>,
"launch_duration":<Double_value>,
"server_jitter":<Double_value>,
"client_jitter":<Double_value>,
"id":<String_value>,
"serverside_0_win":<Double_value>,
"server_latency":<Double_value>,
"host_delay":<Double_value>,
"total_bytes":<Double_value>,
"client_ip_address":<String_value>,
"pn_agent_version":<String_value>,
"client_latency":<Double_value>,
"client_srtt":<Double_value>,
"client_side_ns_delay":<Double_value>,
"server_side_ns_delay":<Double_value>,
"ica_device_ip_address":<String_value>,
"group_reason_id":<Double_value>,
"receiver_version":<String_value>,
"application_enumeration_duration":<Double_value>,
"session_reconnect":<Double_value>,
"serverside_rto":<Double_value>,
"skipflow_description":<String_value>,
"up_time":<Double_value>,
"client_tx_bytes":<Double_value>,
"clientside_packet_retransmits":<Double_value>,
"server_ip_address":<String_value>,
"rpt_sample_time":<Double_value>,
"clientside_0_win":<Double_value>,
"client_rx_bytes":<Double_value>,
"session_setup_time":<Double_value>,
"bandwidth":<Double_value>,
"clientside_rto":<Double_value>,
"ica_app_name":<String_value>,
"server_srtt":<Double_value>,
"skipflow_count":<Double_value>,
"session_rtt":<Double_value>,
"session_end_time":<Double_value>}]}
```







