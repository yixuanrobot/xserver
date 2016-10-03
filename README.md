# xserver
<Highperformence Gameserver><br /><br /><br />
How to build it?<br />
install boost version >=1.42<br />
mkdir build<br />
cd build<br />
cmake ..<br />
make<br /><br /><br /><br />
This is the test!<br /><br />
yixuan@yixuan-All-Series:~$ ab -n100000 -c8000 localhost:8000/index.html<br />
This is ApacheBench, Version 2.3 <$Revision: 1706008 $><br />
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/<br />
Licensed to The Apache Software Foundation, http://www.apache.org/<br /><br />

Benchmarking localhost (be patient)<br />
Completed 10000 requests<br />
Completed 20000 requests<br />
Completed 30000 requests<br />
Completed 40000 requests<br />
Completed 50000 requests<br />
Completed 60000 requests<br />
Completed 70000 requests<br />
Completed 80000 requests<br />
Completed 90000 requests<br />
Completed 100000 requests<br />
Finished 100000 requests<br /><br /><br />


Server Software:        <br />
Server Hostname:        localhost<br />
Server Port:            8000<br /><br />

Document Path:          /index.html<br />
Document Length:        93 bytes<br /><br />

Concurrency Level:      8000<br />
Time taken for tests:   2.578 seconds<br />
Complete requests:      100000<br />
Failed requests:        0<br />
Total transferred:      13700000 bytes<br />
HTML transferred:       9300000 bytes<br />
Requests per second:    38786.03 [#/sec] (mean)<br />
Time per request:       206.260 [ms] (mean)<br />
Time per request:       0.026 [ms] (mean, across all concurrent requests)<br />
Transfer rate:          5189.15 [Kbytes/sec] received<br /><br />

Connection Times (ms)<br />
              min  mean[+/-sd] median   max<br />
Connect:        4   84 250.8     17    1039<br />
Processing:     6   22  33.5     18     817<br />
Waiting:        2   16  33.2     12     814<br />
Total:         18  107 269.1     40    1834<br /><br />

Percentage of the requests served within a certain time (ms)<br />
  50%     40<br />
  66%     41<br />
  75%     45<br />
  80%     48<br />
  90%     60<br />
  95%   1047<br />
  98%   1068<br />
  99%   1249<br />
 100%   1834 (longest request)<br />


