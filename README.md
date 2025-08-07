# Digital-certification

## What is a Digital Certificate?


### English Definition:
A digital certificate is an electronic document that verifies a person, website, or organization's identity using cryptography.

It contains:

Public key

Owner's identity info

Digital signature of the Certificate Authority

### Urdu Explanation:
Digital Certificate ek online ID card ki tarah hota hai jo verify karta hai ke koi website, server ya person real aur trusted hai.
Is mein public key, naam, expiry date, aur CA ka signature hota hai.

## What’s inside a Digital Certificate?

### Field -------------------------------------	Explanation

Subject ---------------------------------	Name of the owner

Issuer---------------------------------	Certificate Authority (CA) name

Public Key -----------------------------	Owner’s public key

Serial Number -----------------------------	Unique ID

Validity -------------------------------	Start & expiry date

Digital Signature --------------------------------	Signed by the CA

Algorithm ------------------------------	Encryption method used

## Types of Digital Certificates 

### Type ---------------------------------------	Use Case--------------------------------------------------------	Urdu

SSL/TLS Certificate --------------------------------	Secures websites (HTTPS) -------------------------------------	ویب سائٹس کی حفاظت

Code Signing Certificate ----------------------------	Verifies software integrity ------------------------------------	سافٹ ویئر پر اعتماد

Email Certificate (S/MIME)----------------------------	Encrypts emails, signs messages -----------------------------------	ای میل کی حفاظت

Client Certificate----------------------------------	Identifies users or devices	------------------------------------- یوزر یا ڈیوائس کی شناخت

Root Certificate ----------------------------------	Base trust certificate for CAs	-------------------------------------بنیادی اعتماد والا سرٹیفکیٹ

## Self-Signed Certificate 
### Definition (English):
A self-signed certificate is signed by the same entity that created it — not signed by any trusted CA.

### Urdu:
Self-signed certificate wo hota hai jo khud apne aap se sign kiya gaya ho. Yeh trusted CA se verify nahi hota, is liye browsers isay unsafe show karte hain.



Internal testing

Local development

Private networks



## Certificate Authority (CA) 
### English Definition:
A Certificate Authority (CA) is a trusted third-party organization that issues, verifies, and signs digital certificates.

###  Urdu:
CA ek trusted company hoti hai (jaise DigiCert, Let's Encrypt, Sectigo) jo certificates banati hai aur verify karti hai ke koi website ya user legit hai ya nahi.

Examples of CAs:

DigiCert

Let's Encrypt

GlobalSign

Sectigo

Comodo

## Certificate Request Process (CSR Process)
(ڈیجیٹل سرٹیفکیٹ کے لیے درخواست کا عمل
### Step	----------------------------------------- Description

1. Generate Key Pair ---------------------------------	A public/private key is created on the server
(Server per key pair banai jati hai)

3. Create CSR (Certificate Signing Request) ------------------	CSR contains public key + identity info
(Yeh ek file hoti hai jisme name, domain, key waghera hotay hain)

5. Submit to CA	-------------------------------------CSR is sent to the Certificate Authority
6. 
7. CA Verifies Info -----------------------------	CA checks identity of the requester (domain, org)
8. 
9. Issue Certificate -------------------------	CA signs the certificate and sends it back
10. 
11. Install Certificate -------------------------	The certificate is installed on the web server
12. 
13. Renewal / Revoke	------------------------------Expired certificates are renewed or revoked if compromised

## Summary Table

### Term -------------------------------------------	Description

Digital Certificate ----------------------------	Confirms identity using public key cryptography

Types	SSL/TLS,----------------------------------- Code Signing, Email, Client

Self-signed Certificate --------------------	Not trusted by default – made & signed by user

Certificate Authority (CA) -------------------	Trusted organization that issues certificates

CSR	Certificate -------------------------------- Signing Request – request sent to CA
