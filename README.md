WebIRC on OpenShift
=========================

WebIRC is a free, open, always connected web IRC client. [Check out the project here](https://github.com/pavben/WebIRC)

Running WebIRC on OpenShift
--------------------

The easiest way to deploy WebIRC on OpenShift is with the [Client Tools](https://developers.openshift.com/en/managing-client-tools.html).

Start by creating a Node.js application:

    rhc app create webirc nodejs-0.10 --from-code=https://github.com/nskaggs/openshift-webirc.git

Your application should be up and running. Login with the default credentials in me.json

To Connect to your application remotely using SSH:

    rhc ssh webirc

You will need want to edit the me.json file accordingly.


This template is based on the excellent work of [Kornagan](https://github.com/Kornagan/openshift-shoutirc).