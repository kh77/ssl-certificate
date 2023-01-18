# SSL Certificate


### Check JKS certificate expiry time
	
	
	keytool -list -v -keystore keystore.jks -storepass "pass" | grep until


### Check the PKCS#12 expiry time


	openssl pkcs12 -in certicate.p12 -nokeys | openssl x509 -noout -enddate
