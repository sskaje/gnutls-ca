# gnutls-ca
GnuTLS CA scripts

Author: sskaje

Basic CA related commands

## Usage
```

GnuTLS CA Script
Author: sskaje http://sskaje.me/
Usage:
    /path/to/ca.sh 
        genca   NAME            generate self signed 
        genkey  NAME [KEYBITS]  generate private key, NAME-key.pem, default KEYBITS=2048
        genreq  NAME            generate certification request, NAME.tmpl required, NAME-cert.csr
        signreq NAME CA_NAME    create certificate from NAME-cert.csr, NAME-cert.pem
        to_p12  NAME [CA_NAME]  export to pkcs#12 NAME.p12, ca cert included if CA_NAME is valid
        p7sign  NAME CA_NAME    sign NAME.mobileconfig to NAME.signed.mobileconfig, gnutls 3.4.x+ required
        gencrl  NAME CA_NAME    create CRL, NAME-crl.pem

```

## CA Certificates
Locates like 
```
~/Documents/CA/APP CA
~/Documents/CA/APP CA/app_ca.key
~/Documents/CA/APP CA/app_ca.pem
~/Documents/CA/USER CA
~/Documents/CA/USER CA/user_ca.key
~/Documents/CA/USER CA/user_ca.pem

```

