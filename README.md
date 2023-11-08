## Summary

This project was to present skills that were learned in using Microsoft Azure. I made a separate cybersecurity blog with the "added" feature of an SSL certificate and Azure's security features.  

## Requirements


+ Hosting the web application using Azure’s Cloud Services
+ Using Azure’s App Service resource to create the web application
+ Choosing a domain with “godaddy or Azure” (choose what you selected)
+ Deploying a Docker container which had a framework for a blog webpage
+ SSHing  into the container to customize the webpage
+ Creating a Self-signed certificate with OpenSSL 
+ Storing the certificate in Azure’s Key vault
+ ~~Binding the certificate to the website~~ (*this line is crossed out as the self-signed cert could not be applied to the free website created on azure*)
+ After determining the security issues with a self-signed certificate, creating and binding a managed CA approved certificate to the web application
+ Deploying Azure’s Front Door, and configuring a WAF rule to restrict traffic from certain countries
+ Analyzing the Azure’s Security Center recommendations and applying the recommended fix

## Key Notes

+ self-signed certificates will never be trusted as it's not as secure compared to a Certificate Authority (CA)
+ TLS is a better and improved version of an SSL
+ Azure's Front Door was used to apply a Web Application Firewall (WAF) so that US, Australia, and Canada can access the site
+ Azure Security Center provides mitigation recommendations and best practices
  1. change FTP to its encrypted version FTPS
 
