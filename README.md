# nodeutils

## csv conversion

[link](https://github.com/ShaneCarr/node-csvtojson)

- npm install convert-csv-to-json --save 
- npm install -g csvtojson 
- sudo apt-get install npm jq 
- csvtojson production_yammertestone_25k_load_test.csv > parsedusers.json
 
## jwt io decode

[link](https://www.npmjs.com/package/jwt-cli)
- jwt <token here> 
 
 ## getting a goken
 
```bash
 curl -X POST https://login.microsoftonline.com/{tenant}/oauth2/token -F grant_type=client_credentials -F resource={resource} -F client_id={client_id} -F client_secret={client_secret}

 curl -X POST https://login.microsoftonline.com/423f054d-16c2-4fcf-a4eb-21fc069010d1/oauth2/token -F grant_type=client_credentials -F resource=https://graph.microsoft.com/
 -F client_id=bd25e636-21e7-4464-8d4f-101435950dec -F client_secret=<secret here>

 curl -X POST https://login.microsoftonline.com/423f054d-16c2-4fcf-a4eb-21fc069010d1/oauth2/token -F grant_type=client_credentials -F resource=https://graph.microsoft.com -F client_id=bd25e636-21e7-4464-8d4f-101435950dec -F client_secret=<secret> -F scope=https://graph.microsoft.com/.default
```

## decode encode

[link](https://www.npmjs.com/package/url-decode-encode-cli)
 
 ```bash
echo -n '{"foo": "bar"}' | url-encode # %7B%22foo%22%3A%20%22bar%22%7D
echo -n '%7B%22foo%22%3A%20%22bar%22%7D' | url-decode # {"foo": "bar"}

echo -n '{"foo": "bar"}' >some-file
url-encode some-file # %7B%22foo%22%3A%20%22bar%22%7D
```
