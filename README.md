beet-amazon
===========

plugin for beets that lets you search amazon for album-details

adds Amazon album search support to the autotagger.
Needs an AmazonAccess Key ID and a Secret access key see:

http://aws-portal.amazon.com/gp/aws/developer/account/index.html

Also needs bottlenose

https://github.com/lionheart/bottlenose

Copy the api.py file to your pluginfolder, rename it bottlenose.py.


You must set Access_Key_ID, Secret_Key_ID and asso_tag in the config of beets
like this...


    amazon:
      Access_Key_ID: youracceskeyID
      Secret_Access_Key: yoursecretaccesskey
      preferred_regions: ["US", "FR"] # try to get tracks from amazon.com and amazon.fr if first failed, default to ["US"]
      asso_tag: yourassotag #can be anything, I just set it to beets)

Basically an [Amazon Web service AWS](http://console.aws.amazon.com) account and an [Amazon Associates](https://affiliate-program.amazon.com/) account on [https://affiliate-program.amazon.com/](https://affiliate-program.amazon.com/) are needed to request tracks from [http://amazon.com](http://amazon.com)

To request
* [http://amazon.fr](http://amazon.fr) (FR): [Amazon Associates](https://partenaires.amazon.fr) on [https://partenaires.amazon.fr](https://partenaires.amazon.fr) is needed
* [http://amazon.ca](http://amazon.ca) (CA): [Amazon Associates](https://associates.amazon.ca) on [https://associates.amazon.ca](https://associates.amazon.ca) is needed
* [http://amazon.cn](http://amazon.cn) (CN): [Amazon Associates](https://associates.amazon.cn) on [https://associates.amazon.cn](https://associates.amazon.cn) is needed
* [http://amazon.de](http://amazon.de) (DE): [Amazon Associates](https://partnernet.amazon.de) on [https://partenaires.amazon.de](https://partenaires.amazon.de) is needed
* [http://amazon.es](http://amazon.es) (ES): [Amazon Associates](https://afiliados.amazon.es) on [https://partenaires.amazon.es](https://partenaires.amazon.es) is needed
* [http://amazon.in](http://amazon.in) (IN): [Amazon Associates](https://affiliate-program.amazon.in) on [https://partenaires.amazon.in](https://partenaires.amazon.in) is needed
* [http://amazon.it](http://amazon.it) (IT): [Amazon Associates](https://programma-affiliazione.amazon.it) on [https://partenaires.amazon.it](https://partenaires.amazon.it) is needed
* [http://amazon.co.jp](http://amazon.co.jp) (JP): [Amazon Associates](https://affiliate.amazon.co.jp) on [https://partenaires.amazon.co.jp](https://partenaires.amazon.co.jp) is needed
* [http://amazon.co.uk](http://amazon.co.uk) (UK): [Amazon Associates](https://affiliate-program.amazon.co.uk) on [https://partenaires.amazon.co.uk](https://partenaires.amazon.co.uk) is needed
* [http://amazon.com.br](http://amazon.com.br) (BR): [Amazon Associates](https://associados.amazon.com.br) on [https://partenaires.amazon.com.br](https://partenaires.amazon.com.br) is needed
* [http://amazon.com.mx](http://amazon.com.mx) (MX): [Amazon Associates](https://afiliados.amazon.com.mx) on [https://partenaires.amazon.com.mx](https://partenaires.amazon.com.mx) is needed
