Red Hat Cloud Suite CloudForms Install Demo
===========================================
Install your very own local instance of the Red Hat CloudForms product, the management tool of choice for Red Hat Cloud Suite infrastructure solutions.

This project requires a docker engine and some patience for the database to be populated after starting up the containerized CloudForms instance. There will be checks during installation and I point you to what is missing. It also checks that you have the right versions running too.


Install on your machine
-----------------------
1. [Download and unzip.](https://github.com/redhatdemocentral/rhcs-cloudforms-demo/archive/master.zip)

2. Run 'init.sh', then sit back.

3. Follow displayed instructions to log in to your brand new Red Hat CloudForms!


Notes
-----
Before the log in interface to CloudForms will be available, it takes around 5-10 minutes to populate the containers database. When
it is done, log in to CloudForms web interface at https://localhost with one of the below users:

```
   Admin user: admin
   Admin pass: smartvm

   Operations user: cloudops
   Operations pass: Redhat1!

   Customer user: clouduser
   Customer pass: Redhat1!
```

This project has an install script that is setup to allow you to re-run it without worrying about previous
installations. To stop and start instead of re-running the install script, use:

```
   $ docker stop cfme4-demo
  
   $ docker start cfme4-demo
```


Supporting Articles
-------------------
- [3 Steps to Cloud Operational Happiness with Red Hat CloudForms](http://www.schabell.org/2016/11/3-steps-to-cloud-happiness-with-ocp.html)


Released versions
-----------------
See the tagged releases for the following versions of the product:

- v1.0 - Red Hat CloudForms 4.2 containerized and running locally.

![CF Login](https://github.com/redhatdemocentral/rhcs-cloudforms-demo/blob/master/docs/demo-images/cf-login.png?raw=true)

![CF Mgmt](https://github.com/redhatdemocentral/rhcs-cloudforms-demo/blob/master/docs/demo-images/cf-cloud-intel.png?raw=true)
