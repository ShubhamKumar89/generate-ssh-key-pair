# Generate an SSH Key Pair

This repository will generate an SSH key pair for UNIX and LINUX systems.

## Create RSA Key Pair

**RSA**(*Rivest–Shamir–Adleman*) is a public-key cryptosystem or an algorithm that is widely used for secure data transmission. An RSA key pair includes a private and a public key. The RSA private key is used to generate digital signatures, and the RSA public key is used to verify digital signatures. RSA uses public key to encrypt messages which can only decrypted by using private key.

```bash
ssh-keygen -t rsa
# -t specifies the type of key we want to create 

# you can also specify the length of the key(bit-size) by using -b option
# e.g. ssh-keygen -b 1024 -t rsa
```

* The command prompts ask you to enter the path to the file in which you want to save the key. By default, a path and file-name is suggested inside the parenthesis.

![image](https://user-images.githubusercontent.com/97805339/180519794-ca077c89-7cba-4e91-8765-de07891bd362.png)

* To accept the default values, press `ENTER`. 

* Now, the command prompt ask you to enter a `passphrase` to protect the private key from unauthorised access. This is an optional part. So, leave it empty, by pressing `ENTER`. After this you will again asked to enter the passphrase, press `ENTER` to continue.

![image](https://user-images.githubusercontent.com/97805339/180558237-423c42f5-ab3f-43a9-a13e-905b8e7cdc3f.png)

* Now the keys have been saved in default directory. The file name of the **SSH private key** is **id_rsa**,and the file name of the **SSH public key** would be **id_rsa.pub**.
