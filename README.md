beet-amazon
===========

plugin for beets that lets you search amazon for album-details

adds Amazon album search support to the autotagger.
Needs an AmazonAccess Key ID and a Secret access key see:

http://aws-portal.amazon.com/gp/aws/developer/account/index.html

Also needs bottlenose

https://github.com/lionheart/bottlenose

in your pluginfolder
you must set Access_Key_ID, Secret_Key_ID and asso_tag in the config of beets
like this...


    amazon:
      Access_Key_ID: youracceskeyID
      Secret_Access_Key: yoursecretaccesskey
      asso_tag: yourassotag(can be anything, I just set it to beets)

