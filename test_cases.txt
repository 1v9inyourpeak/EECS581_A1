-------------- Test Case --------------  | ----- Expected result (valid/invalid) -----  | ----- Result -----  |
connecting to 192.168.1.1 now            |                    Valid                     |        Valid        |
server=10.0.0.255:8080end                |                    Valid                     |        Valid        |
192a168.1.1.1                            |                    Valid                     |        Valid        |
192.168.1.1.                             |                   Invalid                    |       Invalid       |
Connection from 192.168.1.1 refused      |                    Valid                     |        Valid        |
192.168.01.1                             |                   Invalid                    |       Invalid       |
1.2.3.4:99999                            |                   Invalid                    |       Invalid       |
12.34.56                                 |                   Invalid                    |       Invalid       |
no number here                           |                   Invalid                    |       Invalid       |
0.0.0.0                                  |                    Valid                     |        Valid        |
255.255.255.255                          |                    Valid                     |        Valid        |
256.0.0.0                                |                   Invalid                    |       Invalid       |
0.256.0.0                                |                   Invalid                    |       Invalid       |
0.0.256.0                                |                   Invalid                    |       Invalid       |
0.0.0.256                                |                   Invalid                    |       Invalid       |
1.2.3.4                                  |                    Valid                     |        Valid        |
12.34.56.78                              |                    Valid                     |        Valid        |
123.234.245.255                          |                    Valid                     |        Valid        |
000.0.0.0                                |                   Invalid                    |       Invalid       |
00.0.0.0                                 |                   Invalid                    |       Invalid       |
01.2.3.4                                 |                   Invalid                    |       Invalid       |
10.02.3.4                                |                   Invalid                    |       Invalid       |
10.20.003.4                              |                   Invalid                    |       Invalid       |
10.20.30.04                              |                   Invalid                    |       Invalid       |
0000.0.0.0                               |                   Invalid                    |       Invalid       |
1000.0.0.0                               |                   Invalid                    |       Invalid       |
0.1000.0.0                               |                   Invalid                    |       Invalid       |
0.0.0.1000                               |                   Invalid                    |       Invalid       |
1.2.3.4:0                                |                    Valid                     |        Valid        |
1.2.3.4:1                                |                    Valid                     |        Valid        |
1.2.3.4:9                                |                    Valid                     |        Valid        |
1.2.3.4:10                               |                    Valid                     |        Valid        |
1.2.3.4:999                              |                    Valid                     |        Valid        |
1.2.3.4:9999                             |                    Valid                     |        Valid        |
1.2.3.4:65534                            |                    Valid                     |        Valid        |
1.2.3.4:65535                            |                    Valid                     |        Valid        |
1.2.3.4:65536                            |                   Invalid                    |       Invalid       |
1.2.3.4:99999                            |                   Invalid                    |       Invalid       |
1.2.3.4:00                               |                   Invalid                    |       Invalid       |
1.2.3.4:01                               |                   Invalid                    |       Invalid       |
1.2.3.4:001                              |                   Invalid                    |       Invalid       |
1.2.3.4:0001                             |                   Invalid                    |       Invalid       |
1.2.3.4:00000                            |                   Invalid                    |       Invalid       |
1.2.3.4:0                                |                    Valid                     |        Valid        |
x:1.2.3.4                                |                   Invalid                    |       Invalid       |
1.2.3.4:x                                |                   Invalid                    |       Invalid       |
x1.2.3.4:80y                             |                    Valid                     |        Valid        |
x1.2.3.4:80                              |                    Valid                     |        Valid        |
x.1.2.3.4.y                              |                   Invalid                    |       Invalid       |
1.2.3.4 hello 5.6.7.8                    |                    Valid                     |        Valid        |
