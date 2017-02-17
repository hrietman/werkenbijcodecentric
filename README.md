werken bij codecentric landing page
=============================

This is a single web page and used at <a href="http://www.werkenbijcodecentric.nl">werkenbijcodecentric</a>

To build:

<pre>mvn clean install</pre>

To test locally

<pre>mvn appengine:devserver</pre>

Your application is running at http://localhost:8080

To deploy into the cloud

<pre>mvn appengine:update</pre>

If you do this the first time you need to authorize yourself; you will be prompted for this. 

For more details see <a href="https://cloud.google.com/appengine/docs/java/tools/maven">Google App Engine Maven Project</a>

When running mvn appengine:update and you get this:

"Either the access code is invalid or the OAuth token is revoked.Details: invalid_grant"

and then nothing, you need to delete

~/.appcfg_oauth2_tokens_java