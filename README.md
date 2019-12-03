# opencadc-awscli
AWS Command line client

Installs the `awscli` Python module for 3.5, 3.6, 3.7, and 3.8 (latest) running on Alpine Linux.  

Available on Docker Hub:
```bash
docker pull opencadc/awscli
```

Can be run by mounting the `~/.aws` directory:
```bash
docker run --rm --name awscli -ti -v /home/user/.aws:/root/.aws opencadc/awscli aws s3 ls
```

Or start a shell and do a mass upload:
```bash
docker run --rm --name awscli -ti -v /usr/src/data:/usr/src/data -v /home/user/.aws:/root/.aws opencadc/awscli sh

>$ cd /usr/src/data
>$ aws s3 cp 2019-files/* s3://mybucket/
```
