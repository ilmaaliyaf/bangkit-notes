create private key
` openssl genrsa -out private_key.pem 2048 `

create public key
`openssl rsa -in private_key.pem -outform PEM -pubout -out public_key.pem`

encrypt
`openssl rsautl -encrypt -pubin -inkey public_key.pem -in secret.txt -out secret.enc`

decrypt
`openssl rsautl -decrypt -inkey private_key.pem -in secret.enc`

---
Creating hash digest
`openssl dgst -sha256 -sign private_key.pem -out secret.txt.sha256 secret.txt`

verify
`openssl dgst -sha256 -verify public_key.pem -signature secret.txt.sha256 secret.txt`

---
create md5 hash digest
`md5sum file.txt > file.txt.md5`

check the validity
`md5sum -c file.txt.md5`