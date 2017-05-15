# wp-sss
Wordpress Stacks with fine tune for Speed/Secure/Scale with HA

# Measures
## Speed
- Max request/sec
- Min drop request
- Min CPU
- Min RAM

## Secure
- Pass https://github.com/wpscanteam/wpscan

## Scale
- Pass > 1 failed over

## Extras
- Min price

## How to test
- use Apache2 Bench (ab)

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

