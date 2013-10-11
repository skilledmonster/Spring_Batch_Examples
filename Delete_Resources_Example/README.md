<h2>Spring Batch Tasklet Example</h2>

This is a sample project to demonstrate usage of Spring Batch Tasklet.

<b>Scenario:</b>

1. Delete files from a resource directory. This sample project uses "data" directory as resource directory

More details about this project can be found in my blog article <a href="http://www.skilledmonster.com/frameworks/spring/batch/sample-project-integrating-spring-batch-and-spring-integration-modules/">here</a>.

<h2>Author</h2>
<p>Jagadeesh Motamarri [ <a href="http://www.skilledmonster.com">Blog</a> | <a href="http://twitter.com/SkilledMonster">Twitter</a> | <a href="http://www.facebook.com/SkilledMonster">Facebook</a> ]</p>

<h2>Spring Batch</h2>

<p>[ <a href="http://static.springsource.org/spring-batch/">Site</a> | <a href="http://static.springsource.org/spring-batch/reference/index.html">Documentation</a> ]</p>

<h2>Buy me a coffee</h2>
<p>You can do it by PayPal</a>. Thanks! (:</p>
<br/>
<form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top">
<input type="hidden" name="cmd" value="_s-xclick">
<input type="hidden" name="encrypted" value="-----BEGIN PKCS7-----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-----END PKCS7-----
">
<input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif" border="0" name="submit" alt="PayPal - The safer, easier way to pay online!">
<img alt="" border="0" src="https://www.paypalobjects.com/en_US/i/scr/pixel.gif" width="1" height="1">
</form>

