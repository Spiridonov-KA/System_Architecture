### Без кэширования
```
Running 5m test @ http://localhost:8080
  1 threads and 10 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency   284.94ms  457.74ms   2.00s    83.95%
    Req/Sec    15.98      9.54    80.00     83.00%
  Latency Distribution
     50%   80.08ms
     75%  282.74ms
     90%    1.04s 
     99%    1.86s 
  4677 requests in 5.00m, 0.95MB read
  Socket errors: connect 0, read 1390, write 0, timeout 531
  Non-2xx or 3xx responses: 2283
Requests/sec:     15.59
Transfer/sec:      3.25KB
```

### С кэшированием
```
Running 5m test @ http://localhost:8080
  1 threads and 10 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency   224.90ms  388.60ms   2.00s    85.93%
    Req/Sec    44.63     28.29   272.00     76.97%
  Latency Distribution
     50%   81.59ms
     75%  238.28ms
     90%  820.97ms
     99%    1.67s 
  13170 requests in 5.00m, 2.60MB read
  Socket errors: connect 0, read 3887, write 0, timeout 446
  Non-2xx or 3xx responses: 5609
Requests/sec:     43.89
Transfer/sec:      8.89KB
```
