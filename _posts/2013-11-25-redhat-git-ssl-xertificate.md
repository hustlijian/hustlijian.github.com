---
layout: post
categories: problems 
title: "redhat 下处理git ssl certificate 问题"
tags : [git, ssl, ca]
---

问题：
------
	error: SSL certificate problem, verify that the CA cert is OK. Details:
	error:14090086:SSL routines:SSL3_GET_SERVER_CERTIFICATE:certificate verify failed while accessing https://github.com/.../***.git/info/refs?service=git-upload-pack
	fatal: HTTP request failed

解决(下载新的ca证书)：
------
	curl http://curl.haxx.se/ca/cacert.pem -o /etc/pki/tls/certs/ca-bundle.crt

参考：http://serverfault.com/questions/394815/how-to-update-curl-ca-bundle-on-redhat 

Curl is using the system-default CA bundle is stored in /etc/pki/tls/certs/ca-bundle.crt . Before you change it, make a copy of that file so that you can restore the system default if you need to. You can simply append new CA certificates to that file, or you can replace the entire bundle.

Are you also wondering where to get the certificates? I (and others) recommend curl.haxx.se/ca . In one line:

	curl http://curl.haxx.se/ca/cacert.pem -o /etc/pki/tls/certs/ca-bundle.crt
Alternately, you can follow instructions in this article: https://gist.github.com/996292 to request the certs over https.

