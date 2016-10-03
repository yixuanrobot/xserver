# xserver
<Highperformence Gameserver><br /><br /><br />
How to build it?<br />
install boost version >=1.42<br />
mkdir build<br />
cd build<br />
cmake ..<br />
make<br /><br /><br /><br />
This is the test!<br />
$ ab -n100000 -c6000 localhost:8000/index.html<br /><br />

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
Server Port:            8000<br />

Document Path:          /index.html<br />
Document Length:        93 bytes<br /><br />

Concurrency Level:      6000<br />
Time taken for tests:   2.587 seconds<br />
Complete requests:      100000<br />
Failed requests:        0<br />
Total transferred:      13700000 bytes<br />
HTML transferred:       9300000 bytes<br />
Requests per second:    38657.62 [#/sec] (mean)<br />
Time per request:       155.209 [ms] (mean)<br />
Time per request:       0.026 [ms] (mean, across all concurrent requests)<br />
Transfer rate:          5171.97 [Kbytes/sec] received<br /><br />

Connection Times (ms)<br />
              min  mean[+/-sd] median   max<br />
Connect:        6   67 221.4     15    1030<br />
Processing:     7   21  35.4     17     820<br />
Waiting:        2   13  35.3      8     819<br />
Total:         17   88 241.1     31    1847<br />

Percentage of the requests served within a certain time (ms)<br />
  50%     31<br />
  66%     32<br />
  75%     34<br />
  80%     35<br />
  90%     46<br />
  95%   1028<br />
  98%   1056<br />
  99%   1250<br />
 100%   1847 (longest request)<br /><br />

