# \<aes-256-cbc-pbkdf2-30k\>

some description

## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.

## Viewing Your Application

```
$ polymer serve
```

## Building Your Application

```
$ polymer build
```

This will create a `build/` folder with `bundled/` and `unbundled/` sub-folders
containing a bundled (Vulcanized) and unbundled builds, both run through HTML,
CSS, and JS optimizers.

You can serve the built versions by giving `polymer serve` a folder to serve
from:

```
$ polymer serve build/bundled
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.


Detect()
=================
Get hash from local storage
- If we can get the hash, go to Login() else go to Create()

{{action}} none
{{hash}} from storage 


Login()
=================
Enter Password
Get Hash from local storage
Decrypt
- If Decrypt pass go to home 
- If the user forgot the password go to import

{{action}} login
{{password}} from user
{{hash}} from storage
{{mnemonic}} decrypted


Create()
=================
Enter Password
Generate Mnemonic 
Encrypt
Save Hash to local storage
- go to home 
- If the user forgot the password go to import

{{action}} create
{{password}} from user
{{mnemonic}} generated 
{{hash}} generated


Import()
=================
Enter Mnemonic 
Enter Password
Encrypt
Save Hash to local storage
- go to home 

{{action}} import
{{mnemonic}}  from user 
{{password}} from user
{{hash}} generated


Home
=================
