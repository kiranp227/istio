curl -s -I -HHost:httpbin.example.com "http://$INGRESS_HOST:$INGRESS_PORT/"
curl -s -I -HHost:httpbin.example.com "http://$INGRESS_HOST:$INGRESS_PORT/delay/200"
curl -s -I -HHost:httpbin.example.com "http://$INGRESS_HOST:$INGRESS_PORT/status/200"


we should see 200 ok response if the service is accessible
