Instructions to create a CSR(Certificate Signing Request)

#### 
$ openssl req -new -sha256 -days 730 -newkey rsa:2048 -keyout privatekey.txt -out snteks-cert.csr
Generating a 2048 bit RSA private key
.....+++
.....................................+++
writing new private key to 'privatekey.txt'
Enter PEM pass phrase: ()  **Very important to save the passphrase here**
Verifying - Enter PEM pass phrase:
Verify failure
Enter PEM pass phrase:
Verifying - Enter PEM pass phrase:
-----
You are about to be asked to enter information that will be incorporated
into your certificate request.
What you are about to enter is what is called a Distinguished Name or a DN.
There are quite a few fields but you can leave some blank
For some fields there will be a default value,
If you enter '.', the field will be left blank.
-----