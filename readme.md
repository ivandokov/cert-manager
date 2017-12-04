# Cert Manager
Setup SSL certificates easily.
Usually when you purchase SSL certificate you receive multiple files and it is always a hustle to find in Google the correct information how to setup the certificate for your Apache or nginx server.
This script is helping to automate the process.

## Installation
```bash
git clone https://github.com/ivandokov/cert-manager.git
cd cert-manager
./install
```

## Usage

### Create
Create new certificate signing request. This file is required from the company which issues your certificate. Optionally you can use your hosting provider to generate one for you, but not all providers have this option.
```bash
cert-manager request
```

### Create
Create new certificate and private key files. When you run this command you will have to answer to a few questions and copy-paste some information that you have received from the company that issues your certificate.
```bash
cert-manager create
```

### Server configuration
The script does not provide server configuration out-of-the-box because this is not its purpose. You can get some basic configuration for nginx and Apache by running the command below.
```bash
cert-manager serverconfig
```
