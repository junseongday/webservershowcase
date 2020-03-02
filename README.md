# webservershowcase
로컬 https 설정방법

application.properties<br />
server.ssl.key-store: keystore.p12<br />
server.ssl.key-store-password: 123456<br />
server.ssl.keyStoreType: PKCS12<br />
server.ssl.keyAlias: tomcat<br />


터미널에 <br />
keytool -genkey 
  -alias tomcat 
  -storetype PKCS12 
  -keyalg RSA 
  -keysize 2048 
  -keystore keystore.p12 
  -validity 4000
<br />
