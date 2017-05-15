# wp-sss
Wordpress Stacks with fine tune for Speed/Secure/Scale with HA

# Prerequsites
- One command/click to deploy

# Measures
## Speed
- Max request/sec
- Min drop request
- Time per request (mean)
- Transfer rate
- Min CPU
- Min RAM
- Transfer rate

## Secure
- Pass https://github.com/wpscanteam/wpscan

## Scale
- Pass > 1 failed over

## Extras
- Min price $5

## How to test
- Use Apache2 Bench (ab)
- Google Page Speed https://developers.google.com/speed/pagespeed/insights/

### Install apache-bench
- https://github.com/radiospiel/ApacheBench-Lion

or

- http://sudheeraedama.blogspot.com/2013/05/install-apachebench-on-mac-osx-1075.html


#### Fast Test
```
ab -c 40 -n 5000 http://128.199.238.199/
```

#### High concurrent test
```
ab -c 1000 -n 50000 http://128.199.238.199/
```

## How result is measured?

We will measure these 4 values from `ab` result 
```
Failed requests:        0 less is better
Requests per second:    33.91 [#/sec] (mean) more is better
Time per request:       1179.563 [ms] (mean) less is better
Transfer rate:          1719.75 [Kbytes/sec] received more is better
```
