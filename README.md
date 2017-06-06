# Shibboleth example

## How to use?

1.Place your certifcate (name: "sp-cert.pem") and key (name: "sp-key.pem") inside the shibboleth folder. 

2.Build the docker image with

~~~BASH
docker build -t shibboleth-example .
~~~

3.Run the docker image with

~~~BASH
docker run -itd  --network host  shibboleth-example httpd-shibd-foreground
~~~

4.Append to your /etc/hosts file the line

~~~
127.0.0.1 sp26.example.org
~~~
