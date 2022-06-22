During inference of 60 MB file https://drive.google.com/file/d/1Jv7tbB3TnZqJsaKPs1FygG1BOdBGu8xk/view?usp=sharing

root@localhost:/StratosphereLinuxIPS# ./slips.py -c slips.conf -f conn.log
Slips. Version 0.9.1 (a54d38b0)
https://stratosphereips.org
---------------------------
[Main] Using redis server on port: 34598
Started main program [PID 1391]
Started output thread [PID 1407]
                Starting the module RiskIQ (Module to get different information from RiskIQ) [PID 1412]
                Starting the module arp (Detect arp attacks) [PID 1414]
                Starting the module flowalerts (Alerts about flows: long connection, successful ssh, password guessing, self-signed certificate, data exfiltration, etc.) [PID 1416]
                Starting the module flowmldetection (Train or test a Machine Learning model to detect malicious flows) [PID 1417]
                Starting the module HTTP Analyzer (Analyze HTTP flows) [PID 1419]
                Starting the module ip_info (Get different info about an IP/MAC address) [PID 1420]
                Starting the module portscandetector-1 (Detect Horizonal, Vertical and ICMP scans) [PID 1421]
                Starting the module rnn-cc-detection (Detect C&C channels based on behavioral letters) [PID 1422]
                Starting the module threatintelligence1 (Check if the srcIP or dstIP are in a malicious list of IPs) [PID 1423]
                Starting the module timeline (Creates kalipso timeline of what happened in the network based on flows and available data) [PID 1425]
                Starting the module UpdateManager (Update Threat Intelligence files) [PID 1431]
[virustotal] The file with API key (modules/virustotal/api_key_secret) could not be loaded. VT module is stopping.
                Starting the module virustotal (IP, domain and file hash lookup on Virustotal) [PID 1433]
---------------------------
[Main] Disabled Modules: ['template', 'ensembling', 'exporting_alerts', 'p2ptrust', 'CESNET', 'blocking', 'leak_detector']
[EvidenceProcess-14] Storing Slips logs in output/conn.log_2022-06-22_09:07:23/
Started Evidence Process [PID 1436]
[update_manager] 44 TI files successfully loaded.
Started Profiler Process [PID 1439]
Started input thread [PID 1440]
[Main] Warning: You have 2 redis servers running. Run Slips with --killall to stop them.
[EvidenceProcess-14] 2012/03/16 15:50:51 IP 192.168.202.76  detected as infected in timewindow 1 (start 2012-03-16T15:50:40.650000+00:00, stop 2012-03-16T16:50:40.650000+0000) given the following evidence:
        • Detected Connection to unknown destination port 40028/TCP destination IP 213.199.179.152.
        • Detected Connection to unknown destination port 40046/TCP destination IP 157.56.52.15.
        • Detected Connection to unknown destination port 40024/TCP destination IP 157.55.56.150.
        • Detected Connection to unknown destination port 40020/TCP destination IP 64.4.23.162.
        • Detected Connection to unknown destination port 40003/TCP destination IP 157.55.235.156.
        • Detected Connection to unknown destination port 40028/TCP destination IP 213.199.179.152. AS: MICROSOFT-CORP-MSN-AS-BLOCK
        • Detected Connection to unknown destination port 40017/TCP destination IP 111.221.74.23.
        • Detected Connection to unknown destination port 40020/TCP destination IP 157.56.52.24.

[EvidenceProcess-14] 2012/03/16 15:51:02 IP 192.168.202.102  detected as infected in timewindow 1 (start 2012-03-16T15:50:40+00:00, stop 2012-03-16T16:50:40.000000+0000) given the following evidence:
        • Detected Connection to unknown destination port 6505/TCP destination IP 192.168.28.100.
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1246 to 192.168.28.100:6505
        • Detected Connection to unknown destination port 6513/TCP destination IP 192.168.28.103.
        • Detected Connection to unknown destination port 58448/TCP destination IP 192.168.24.152.
        • Detected Connection to unknown destination port 6513/TCP destination IP 192.168.26.152.
        • Detected Connection to unknown destination port 6558/TCP destination IP 192.168.21.103.
        • Detected Connection to unknown destination port 6512/TCP destination IP 192.168.28.103.
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1245 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1248 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1247 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1249 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1250 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1252 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1251 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1253 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1254 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1256 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1255 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1258 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1257 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1259 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1260 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1261 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1262 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1263 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1264 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1266 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1265 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1369 to 192.168.28.103:6513
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1268 to 192.168.24.202:80
        • Detected Connection to unknown destination port 6504/TCP destination IP 192.168.28.152.
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1267 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1269 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1270 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1271 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1272 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1273 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1274 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1275 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1276 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1277 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1278 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1280 to 192.168.24.152:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1281 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1279 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1283 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1282 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1284 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1285 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1286 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1287 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1288 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1289 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1290 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1291 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1293 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1292 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1296 to 192.168.24.152:58448
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1295 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1297 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1298 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1299 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1301 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1300 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1302 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1303 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1305 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1304 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1306 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1307 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1308 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1309 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1310 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1311 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1312 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1313 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1314 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1315 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1316 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1317 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1318 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1319 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1320 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1321 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1323 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1322 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:4397 to 192.168.26.152:6513
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1325 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1324 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:4401 to 192.168.21.103:6558
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1328 to 192.168.21.103:6558
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1327 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1326 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1329 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1330 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1332 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1331 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1333 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1334 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1336 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1335 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1338 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1337 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1339 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1340 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1341 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1342 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1343 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1344 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1345 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1346 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1348 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1347 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1349 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1350 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1351 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1352 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1353 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1354 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1355 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1356 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1358 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1357 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1360 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1359 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1363 to 192.168.24.152:58448
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1362 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1361 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1364 to 192.168.26.152:6513
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1365 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1366 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:4439 to 192.168.28.103:6512
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1367 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1368 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1370 to 192.168.24.202:80
        • Detected Malicious flow by ML. Src IP 192.168.202.102:1371 to 192.168.24.202:80
        • Detected Connection to unknown destination port 6528/TCP destination IP 192.168.28.152.

[EvidenceProcess-14] 2012/03/16 15:51:02 IP 192.168.202.83  detected as infected in timewindow 1 (start 2012-03-16T15:50:49.990000+00:00, stop 2012-03-16T16:50:49.990000+0000) given the following evidence:
        • Detected new vertical port scan to IP 192.168.206.44 from 192.168.202.83. Total 6 dst ports of protocol TCP. Not Established. Tot pkts sent all ports: 6. Confidence: 0.6
        • Detected new vertical port scan to IP 192.168.206.44 from 192.168.202.83. Total 12 dst ports of protocol TCP. Not Established. Tot pkts sent all ports: 12. Confidence: 1
        • Detected new vertical port scan to IP 192.168.206.44 from 192.168.202.83. Total 18 dst ports of protocol TCP. Not Established. Tot pkts sent all ports: 18. Confidence: 1
        • Detected new vertical port scan to IP 192.168.206.44 from 192.168.202.83. Total 24 dst ports of protocol TCP. Not Established. Tot pkts sent all ports: 25. Confidence: 1
        • Detected new vertical port scan to IP 192.168.206.44 from 192.168.202.83. Total 30 dst ports of protocol TCP. Not Established. Tot pkts sent all ports: 31. Confidence: 1
        • Detected new vertical port scan to IP 192.168.206.44 from 192.168.202.83. Total 36 dst ports of protocol TCP. Not Established. Tot pkts sent all ports: 37. Confidence: 1
        • Detected new vertical port scan to IP 192.168.206.44 from 192.168.202.83. Total 42 dst ports of protocol TCP. Not Established. Tot pkts sent all ports: 43. Confidence: 1
        • Detected new vertical port scan to IP 192.168.206.44 from 192.168.202.83. Total 48 dst ports of protocol TCP. Not Established. Tot pkts sent all ports: 49. Confidence: 1
        • Detected new vertical port scan to IP 192.168.206.44 from 192.168.202.83. Total 54 dst ports of protocol TCP. Not Established. Tot pkts sent all ports: 55. Confidence: 1
        • Detected new vertical port scan to IP 192.168.206.44 from 192.168.202.83. Total 60 dst ports of protocol TCP. Not Established. Tot pkts sent all ports: 61. Confidence: 1
        • Detected new vertical port scan to IP 192.168.206.44 from 192.168.202.83. Total 66 dst ports of protocol TCP. Not Established. Tot pkts sent all ports: 67. Confidence: 1
        • Detected new vertical port scan to IP 192.168.206.44 from 192.168.202.83. Total 72 dst ports of protocol TCP. Not Established. Tot pkts sent all ports: 73. Confidence: 1
        • Detected new vertical port scan to IP 192.168.206.44 from 192.168.202.83. Total 78 dst ports of protocol TCP. Not Established. Tot pkts sent all ports: 79. Confidence: 1
        • Detected new vertical port scan to IP 192.168.206.44 from 192.168.202.83. Total 84 dst ports of protocol TCP. Not Established. Tot pkts sent all ports: 85. Confidence: 1
        • Detected new vertical port scan to IP 192.168.206.44 from 192.168.202.83. Total 90 dst ports of protocol TCP. Not Established. Tot pkts sent all ports: 91. Confidence: 1
        • Detected new vertical port scan to IP 192.168.206.44 from 192.168.202.83. Total 96 dst ports of protocol TCP. Not Established. Tot pkts sent all ports: 97. Confidence: 1
        • Detected new vertical port scan to IP 192.168.206.44 from 192.168.202.83. Total 102 dst ports of protocol TCP. Not Established. Tot pkts sent all ports: 103. Confidence: 1
        • Detected new vertical port scan to IP 192.168.206.44 from 192.168.202.83. Total 114 dst ports of protocol TCP. Not Established. Tot pkts sent all ports: 115. Confidence: 1
        • Detected Multiple reconnection attempts to Destination IP: 192.168.206.44  from IP: 192.168.202.83 reconnections: 5
        • Detected Multiple reconnection attempts to Destination IP: 192.168.206.44  from IP: 192.168.202.83 reconnections: 6
        • Detected Connection to unknown destination port 199/TCP destination IP 192.168.206.44.
        • Detected Multiple reconnection attempts to Destination IP: 192.168.206.44  from IP: 192.168.202.83 reconnections: 7
        • Detected Multiple reconnection attempts to Destination IP: 192.168.206.44  from IP: 192.168.202.83 reconnections: 8
        • Detected Connection to unknown destination port 256/TCP destination IP 192.168.206.44.
        • Detected Multiple reconnection attempts to Destination IP: 192.168.206.44  from IP: 192.168.202.83 reconnections: 9
        • Detected Multiple reconnection attempts to Destination IP: 192.168.206.44  from IP: 192.168.202.83 reconnections: 10
        • Detected new vertical port scan to IP 192.168.206.44 from 192.168.202.83. Total 126 dst ports of protocol TCP. Not Established. Tot pkts sent all ports: 127. Confidence: 1
        • Detected Multiple reconnection attempts to Destination IP: 192.168.206.44  from IP: 192.168.202.83 reconnections: 12
        • Detected Multiple reconnection attempts to Destination IP: 192.168.206.44  from IP: 192.168.202.83 reconnections: 13
        • Detected Connection to unknown destination port 8888/TCP destination IP 192.168.206.44.
        • Detected Multiple reconnection attempts to Destination IP: 192.168.206.44  from IP: 192.168.202.83 reconnections: 14
        • Detected Connection to unknown destination port 1025/TCP destination IP 192.168.206.44.
        • Detected Multiple reconnection attempts to Destination IP: 192.168.206.44  from IP: 192.168.202.83 reconnections: 15
        • Detected Multiple reconnection attempts to Destination IP: 192.168.206.44  from IP: 192.168.202.83 reconnections: 16
        • Detected Multiple reconnection attempts to Destination IP: 192.168.206.44  from IP: 192.168.202.83 reconnections: 17

Total Number of Profiles in DB so far: 37. Modified Profiles in the last TW: 1. (2022-06-22--09:17:23)
Total Number of Profiles in DB so far: 37. Modified Profiles in the last TW: 6. (2022-06-22--09:26:09)
 otal Number of Profiles in DB so far: 42. Modified Profiles in the last TW: 1. (2022-06-22--09:33:21)
^Ctal Number of Profiles in DB so far: 50. Modified Profiles in the last TW: 1. (2022-06-22--09:45:08)
---------------------------
Stopping Slips
Process InputProcess:
Traceback (most recent call last):
  File "/usr/lib/python3.8/multiprocessing/process.py", line 318, in _bootstrap
    util._exit_function()
  File "/usr/lib/python3.8/multiprocessing/util.py", line 360, in _exit_function
    _run_finalizers()
  File "/usr/lib/python3.8/multiprocessing/util.py", line 300, in _run_finalizers
    finalizer()
        timeline                Stopped. 15 left.
Process EvidenceProcess-14:
        ip_info                 Stopped. 14 left.
        EvidenceProcess         Stopped. 13 left.
Traceback (most recent call last):
Process ProfilerProcess-15:
Exception ignored in: <function Connection.__del__ at 0x7f1a4ee6a5e0>
Traceback (most recent call last):
  File "/usr/local/lib/python3.8/dist-packages/redis/connection.py", line 544, in __del__
        ProfilerProcess         Stopped. 12 left.
Traceback (most recent call last):
        portscandetector-1      Stopped. 11 left.
        arp                     Stopped. 10 left.
        UpdateManager           Stopped. 9 left.
        flowmldetection         Stopped. 8 left.
  File "/usr/lib/python3.8/multiprocessing/process.py", line 318, in _bootstrap
    util._exit_function()
  File "/usr/lib/python3.8/multiprocessing/util.py", line 360, in _exit_function
    _run_finalizers()
        threatintelligence1     Stopped. 7 left.
  File "/usr/lib/python3.8/multiprocessing/util.py", line 300, in _run_finalizers
    finalizer()
  File "/usr/lib/python3.8/multiprocessing/util.py", line 224, in __call__
    res = self._callback(*self._args, **self._kwargs)
  File "/usr/lib/python3.8/multiprocessing/queues.py", line 195, in _finalize_join
    thread.join()
  File "/usr/lib/python3.8/threading.py", line 1011, in join
    self._wait_for_tstate_lock()
  File "/usr/lib/python3.8/threading.py", line 1027, in _wait_for_tstate_lock
    elif lock.acquire(block, timeout):
KeyboardInterrupt
    self.disconnect()
  File "/usr/local/lib/python3.8/dist-packages/redis/connection.py", line 675, in disconnect
    self._sock.close()
  File "/usr/lib/python3.8/multiprocessing/process.py", line 318, in _bootstrap
    util._exit_function()
  File "/usr/lib/python3.8/multiprocessing/util.py", line 360, in _exit_function
    _run_finalizers()
  File "/usr/lib/python3.8/multiprocessing/util.py", line 300, in _run_finalizers
    finalizer()
  File "/usr/lib/python3.8/multiprocessing/util.py", line 224, in __call__
    res = self._callback(*self._args, **self._kwargs)
  File "/usr/lib/python3.8/multiprocessing/queues.py", line 195, in _finalize_join
    thread.join()
  File "/usr/lib/python3.8/threading.py", line 1011, in join
    self._wait_for_tstate_lock()
  File "/usr/lib/python3.8/threading.py", line 1027, in _wait_for_tstate_lock
    elif lock.acquire(block, timeout):
KeyboardInterrupt
KeyboardInterrupt:
        rnn-cc-detection        Stopped. 6 left.
        HTTP Analyzer           Stopped. 5 left.
        OutputProcess           Stopped. 4 left.
        flowalerts              Stopped. 3 left.
^C      RiskIQ                  Already stopped.
        virustotal              Already stopped.
        InputProcess            Killed.
Process flowmldetection:
Traceback (most recent call last):
  File "/usr/lib/python3.8/multiprocessing/process.py", line 318, in _bootstrap
    util._exit_function()
  File "/usr/lib/python3.8/multiprocessing/util.py", line 360, in _exit_function
    _run_finalizers()
  File "/usr/lib/python3.8/multiprocessing/util.py", line 300, in _run_finalizers
    finalizer()
  File "/usr/lib/python3.8/multiprocessing/util.py", line 224, in __call__
    res = self._callback(*self._args, **self._kwargs)
  File "/usr/lib/python3.8/multiprocessing/queues.py", line 195, in _finalize_join
    thread.join()
  File "/usr/lib/python3.8/threading.py", line 1011, in join
    self._wait_for_tstate_lock()
  File "/usr/lib/python3.8/threading.py", line 1027, in _wait_for_tstate_lock
    elif lock.acquire(block, timeout):
KeyboardInterrupt
root@localhost:/StratosphereLinuxIPS#
