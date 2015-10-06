Tool for scan PLC devices over s7comm or modbus protocols.

## Usage examples ##

  * `plcscan.py 192.168.0.1`

  * `plcscan.py --timeout 2 192.168.0.1:102 10.0.0.0/24`

  * `plcscan.py --hosts-list hosts.txt`

where file hosts.txt looks like:
<pre>
192.168.1.15<br>
192.168.1.107:102<br>
example.host:502<br>
</pre>


## Output examples ##
### Siemens PLC ###
<pre>
127.0.0.1:102 S7comm (src_tsap=0x100, dst_tsap=0x102)<br>
Module                   : 6ES7 151-8AB01-0AB0  v.0.2    	(36455337203135312d38414230312d304142302000c000020001)<br>
Basic Hardware           : 6ES7 151-8AB01-0AB0  v.0.2    	(36455337203135312d38414230312d304142302000c000020001)<br>
Basic Firmware           :                      v.3.2.6  	(202020202020202020202020202020202020202000c056030206)<br>
Unknown (129)            : Boot Loader           A       	(426f6f74204c6f61646572202020202020202020000041200909)<br>
Name of the PLC          : SIMATIC 300(xxxxxxxxx)      	(53494d4154494320333030280000000000000000002900000000000000000000)<br>
Name of the module       : IM151-8 PN/DP CPU             	(494d3135312d3820504e2f445020435055000000000000000000000000000000)<br>
Plant identification     :                               	(0000000000000000000000000000000000000000000000000000000000000000)<br>
Copyright                : Original Siemens Equipment    	(4f726967696e616c205369656d656e732045717569706d656e74000000000000)<br>
Serial number of module  : S C-BOUVxxxxxxxx              	(5320432d424f5556xxxxxxxxxx00000000000000000000000000000000000000)<br>
Module type name         : IM151-8 PN/DP CPU             	(494d3135312d3820504e2f445020435055000000000000000000000000000000)<br>
</pre>

### Modbus device ###
<pre>
127.0.0.1:502 Modbus/TCP<br>
Unit ID: 0<br>
Response error: ILLEGAL FUNCTION<br>
Device info error: ILLEGAL FUNCTION<br>
Unit ID: 255<br>
Response error: GATEWAY TARGET DEVICE FAILED TO RESPOND<br>
Device: Lantronix I WiPo V3.2.25<br>
</pre>