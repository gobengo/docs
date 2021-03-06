---
title: Module config
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->

<a href="../index.html">@pulumi/azure</a> &gt; config

<div class="toggleVisible" markdown="1">
<div class="collapsed" markdown="1">
<h2 class="pdoc-module-header toggleButton" title="Click to show Index">Index ▹</h2>
</div>
<div class="expanded" markdown="1">
<h2 class="pdoc-module-header toggleButton" title="Click to hide Index">Index ▾</h2>
<div class="pdoc-module-contents" markdown="1">
* <a href="#clientCertificatePassword">let clientCertificatePassword</a>
* <a href="#clientCertificatePath">let clientCertificatePath</a>
* <a href="#clientId">let clientId</a>
* <a href="#clientSecret">let clientSecret</a>
* <a href="#environment">let environment</a>
* <a href="#msiEndpoint">let msiEndpoint</a>
* <a href="#partnerId">let partnerId</a>
* <a href="#skipCredentialsValidation">let skipCredentialsValidation</a>
* <a href="#skipProviderRegistration">let skipProviderRegistration</a>
* <a href="#subscriptionId">let subscriptionId</a>
* <a href="#tenantId">let tenantId</a>
* <a href="#useMsi">let useMsi</a>

<a href="https://github.com/pulumi/pulumi-azure/blob/33be347f8eaeea8b472b3347d9d7f334b07275a4/sdk/nodejs/config/vars.ts">config/vars.ts</a> 
</div>
</div>
</div>


<h2 class="pdoc-module-header" id="clientCertificatePassword">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-azure/blob/33be347f8eaeea8b472b3347d9d7f334b07275a4/sdk/nodejs/config/vars.ts#L9">let <b>clientCertificatePassword</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">
<pre class="highlight"><span class='kd'>let</span> clientCertificatePassword: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.get(&#34;clientCertificatePassword&#34;)</span>;</pre>
</div>
<h2 class="pdoc-module-header" id="clientCertificatePath">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-azure/blob/33be347f8eaeea8b472b3347d9d7f334b07275a4/sdk/nodejs/config/vars.ts#L10">let <b>clientCertificatePath</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">
<pre class="highlight"><span class='kd'>let</span> clientCertificatePath: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.get(&#34;clientCertificatePath&#34;)</span>;</pre>
</div>
<h2 class="pdoc-module-header" id="clientId">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-azure/blob/33be347f8eaeea8b472b3347d9d7f334b07275a4/sdk/nodejs/config/vars.ts#L11">let <b>clientId</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">
<pre class="highlight"><span class='kd'>let</span> clientId: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.get(&#34;clientId&#34;) || (utilities.getEnv(&#34;ARM_CLIENT_ID&#34;) || &#34;&#34;)</span>;</pre>
</div>
<h2 class="pdoc-module-header" id="clientSecret">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-azure/blob/33be347f8eaeea8b472b3347d9d7f334b07275a4/sdk/nodejs/config/vars.ts#L12">let <b>clientSecret</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">
<pre class="highlight"><span class='kd'>let</span> clientSecret: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.get(&#34;clientSecret&#34;) || (utilities.getEnv(&#34;ARM_CLIENT_SECRET&#34;) || &#34;&#34;)</span>;</pre>
</div>
<h2 class="pdoc-module-header" id="environment">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-azure/blob/33be347f8eaeea8b472b3347d9d7f334b07275a4/sdk/nodejs/config/vars.ts#L13">let <b>environment</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">
<pre class="highlight"><span class='kd'>let</span> environment: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> = <span class='s2'> utilities.requireWithDefault(() =&gt; __config.require(&#34;environment&#34;), (utilities.getEnv(&#34;ARM_ENVIRONMENT&#34;) || &#34;public&#34;))</span>;</pre>
</div>
<h2 class="pdoc-module-header" id="msiEndpoint">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-azure/blob/33be347f8eaeea8b472b3347d9d7f334b07275a4/sdk/nodejs/config/vars.ts#L14">let <b>msiEndpoint</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">
<pre class="highlight"><span class='kd'>let</span> msiEndpoint: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.get(&#34;msiEndpoint&#34;) || (utilities.getEnv(&#34;ARM_MSI_ENDPOINT&#34;) || &#34;&#34;)</span>;</pre>
</div>
<h2 class="pdoc-module-header" id="partnerId">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-azure/blob/33be347f8eaeea8b472b3347d9d7f334b07275a4/sdk/nodejs/config/vars.ts#L15">let <b>partnerId</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">
<pre class="highlight"><span class='kd'>let</span> partnerId: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.get(&#34;partnerId&#34;)</span>;</pre>
</div>
<h2 class="pdoc-module-header" id="skipCredentialsValidation">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-azure/blob/33be347f8eaeea8b472b3347d9d7f334b07275a4/sdk/nodejs/config/vars.ts#L16">let <b>skipCredentialsValidation</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">
<pre class="highlight"><span class='kd'>let</span> skipCredentialsValidation: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.getObject&lt;boolean&gt;(&#34;skipCredentialsValidation&#34;) || (utilities.getEnvBoolean(&#34;ARM_SKIP_CREDENTIALS_VALIDATION&#34;) || false)</span>;</pre>
</div>
<h2 class="pdoc-module-header" id="skipProviderRegistration">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-azure/blob/33be347f8eaeea8b472b3347d9d7f334b07275a4/sdk/nodejs/config/vars.ts#L17">let <b>skipProviderRegistration</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">
<pre class="highlight"><span class='kd'>let</span> skipProviderRegistration: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.getObject&lt;boolean&gt;(&#34;skipProviderRegistration&#34;) || (utilities.getEnvBoolean(&#34;ARM_SKIP_PROVIDER_REGISTRATION&#34;) || false)</span>;</pre>
</div>
<h2 class="pdoc-module-header" id="subscriptionId">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-azure/blob/33be347f8eaeea8b472b3347d9d7f334b07275a4/sdk/nodejs/config/vars.ts#L18">let <b>subscriptionId</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">
<pre class="highlight"><span class='kd'>let</span> subscriptionId: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.get(&#34;subscriptionId&#34;) || (utilities.getEnv(&#34;ARM_SUBSCRIPTION_ID&#34;) || &#34;&#34;)</span>;</pre>
</div>
<h2 class="pdoc-module-header" id="tenantId">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-azure/blob/33be347f8eaeea8b472b3347d9d7f334b07275a4/sdk/nodejs/config/vars.ts#L19">let <b>tenantId</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">
<pre class="highlight"><span class='kd'>let</span> tenantId: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.get(&#34;tenantId&#34;) || (utilities.getEnv(&#34;ARM_TENANT_ID&#34;) || &#34;&#34;)</span>;</pre>
</div>
<h2 class="pdoc-module-header" id="useMsi">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-azure/blob/33be347f8eaeea8b472b3347d9d7f334b07275a4/sdk/nodejs/config/vars.ts#L20">let <b>useMsi</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">
<pre class="highlight"><span class='kd'>let</span> useMsi: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span> = <span class='s2'> __config.getObject&lt;boolean&gt;(&#34;useMsi&#34;) || (utilities.getEnvBoolean(&#34;ARM_USE_MSI&#34;) || false)</span>;</pre>
</div>
