# curl basics

# Simple curl call
```
curl https://github.com/dilipkumar2k6/curl-basics
```
# Rest API for json
```
curl https://api.github.com/users
```
# To print header (-i)
```
curl -i https://api.github.com/users
```
# Post update/delete operation (-d)
```
curl -d "repo:test&user:dilipkumar2k6"  https://api.github.com/repository
```

# Explicitly define the HTTP Verb (-x)
```
curl -x POST -d "repo:test&user:dilipkumar2k6"  https://api.github.com/repository
```

# Basic Authenticate API (-u)
``` 
curl -u username:password https://api.github.com/users 
```
# Download binary (-o)
``` 
curl -o test.png https://api.github.com/profile/2-2.png 
curl -o users.json https://api.github.com/users
```
# Follow redirection (-l)
``` 
curl -l users.json https://api.github.com/users
```
# Set headers (-H)
```
curl -X GET \
  'https://username.carto.com/endpoint/' \
  -H 'authorization: Basic dXNlcm5hbWU6MTIzNDU2Nzg5MDEyMzQ1Njc4OTAxMjM0NTY3ODkwMTIzNDU2Nzg5MA==' 
```
# TLS communication (--key, --cert, --cacert)
```
curl --cacert ca.crt \
     --key client.key \
     --cert client.crt \
     https://cloud-controller-ng.service.cf.internal:9023/internal/v4/syslog_drain_urls
```
# Verbose output (-v)
```
curl -v  https://api.github.com/users 
```
# Insecure TLS communications (-k)
```
curl -k https://api.github.com/users 
```
# Only prints headers (-I)
```
curl -I https://api.github.com/users 
```




