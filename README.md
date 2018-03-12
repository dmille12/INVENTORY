# INVENTORY
SC INVENTORY
While the Wiki has decent instructions for Inventory, do not worry about setting up the dojo environment–perform the basic perl stuff but do not include Dojo Environment:

https://wiki.servercentral.com/o/index.php/Inventory_Development#Development_Instance_Dependencies

Note: The new hire must run the cpan.sh twice. If the install gets stuck in a loop, ^C and rerun.

create client cert: 

https://wiki.servercentral.com/o/index.php/SSL_Client_Cert_For_REST_API 

change all the mysql database config in the reflected.cfg file to match the new hire’s setup 

search for ‘dsn’ in the file 

change the connect strings and user/pass to what the new hire’s setup is in the first step (except for kayako_dsn—should be correct) 

change the instances of ‘nobody@servercentral.com’ to the new hire’s assigned email

update the portal_rest api_url, ui_url, cert_file, and key_file to the information that the new hire recently created 

update the netsuite_cache api_url, and the proxy_ip_addr 

set the ssl_cert_file and ssl_key_file to the ones that the new hire opened with the IT ticket. 

The new hire should be able to navigate to https://<server hostname> in any browser and log into the new hire’s instance.
