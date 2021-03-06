---
title: Package @pulumi/kubernetes
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->


{% include langchoose.html nodeonly=true %}

```javascript
var kubernetes = require("@pulumi/kubernetes");
```

```typescript
import * as kubernetes from "@pulumi/kubernetes";
```


<div class="toggleVisible" markdown="1">
<div class="collapsed" markdown="1">
<h2 class="pdoc-module-header toggleButton" title="Click to show Index">Index ▹</h2>
</div>
<div class="expanded" markdown="1">
<h2 class="pdoc-module-header toggleButton" title="Click to hide Index">Index ▾</h2>
<div class="pdoc-module-contents" markdown="1">
* <a href="#Provider">class Provider</a>
* <a href="#ProviderArgs">interface ProviderArgs</a>

<a href="https://github.com/pulumi/pulumi-kubernetes/blob/a33e855465c06a2921aead18ba9f84519baacfd7/sdk/nodejs/provider.ts">provider.ts</a> 
</div>
</div>
</div>

<div class="toggleVisible" markdown="1">
<div class="collapsed" markdown="1">
<h2 class="pdoc-module-header toggleButton" title="Click to show Modules">Modules ▹</h2>
</div>
<div class="expanded" markdown="1">
<h2 class="pdoc-module-header toggleButton" title="Click to hide Modules">Modules ▾</h2>
<div class="pdoc-module-contents" markdown="1">
* <a href="admissionregistration">admissionregistration</a>
* <a href="apiextensions">apiextensions</a>
* <a href="apiregistration">apiregistration</a>
* <a href="apps">apps</a>
* <a href="auditregistration">auditregistration</a>
* <a href="authentication">authentication</a>
* <a href="authorization">authorization</a>
* <a href="autoscaling">autoscaling</a>
* <a href="batch">batch</a>
* <a href="certificates">certificates</a>
* <a href="coordination">coordination</a>
* <a href="core">core</a>
* <a href="events">events</a>
* <a href="extensions">extensions</a>
* <a href="helm">helm</a>
* <a href="meta">meta</a>
* <a href="networking">networking</a>
* <a href="node">node</a>
* <a href="policy">policy</a>
* <a href="rbac">rbac</a>
* <a href="scheduling">scheduling</a>
* <a href="settings">settings</a>
* <a href="storage">storage</a>
* <a href="yaml">yaml</a>
</div>
</div>
</div>

<h2 class="pdoc-module-header" id="Provider">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/a33e855465c06a2921aead18ba9f84519baacfd7/sdk/nodejs/provider.ts#L6">class <b>Provider</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">
<pre class="highlight"><span class='kd'>extends</span> ProviderResource</pre>

The provider type for the kubernetes package.

<h3 class="pdoc-member-header" id="Provider-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/a33e855465c06a2921aead18ba9f84519baacfd7/sdk/nodejs/provider.ts#L6"> <b>constructor</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">

<pre class="highlight"><span class='kd'></span><span class='kd'>new</span> Provider(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, args: <a href='#ProviderArgs'>ProviderArgs</a>, opts?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#ResourceOptions'>pulumi.ResourceOptions</a>)</pre>


Create a Provider resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

</div>
<h3 class="pdoc-member-header" id="Provider-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/a33e855465c06a2921aead18ba9f84519baacfd7/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L14">method <b>getProvider</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">

<pre class="highlight"><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): ProviderResource | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></pre>

</div>
<h3 class="pdoc-member-header" id="Provider-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/a33e855465c06a2921aead18ba9f84519baacfd7/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L101">method <b>isInstance</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">

<pre class="highlight"><span class='kd'>static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span></pre>


Returns true if the given object is an instance of CustomResource.  This is designed to work even when
multiple copies of the Pulumi SDK have been loaded into the same process.

</div>
<h3 class="pdoc-member-header" id="Provider-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/a33e855465c06a2921aead18ba9f84519baacfd7/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L96">property <b>id</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>id: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Output'>Output</a>&lt;<a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#ID'>ID</a>&gt;;</pre>

id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

</div>
<h3 class="pdoc-member-header" id="Provider-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/a33e855465c06a2921aead18ba9f84519baacfd7/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L12">property <b>urn</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>urn: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Output'>Output</a>&lt;<a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#URN'>URN</a>&gt;;</pre>

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

</div>
</div>
<h2 class="pdoc-module-header" id="ProviderArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/a33e855465c06a2921aead18ba9f84519baacfd7/sdk/nodejs/provider.ts#L28">interface <b>ProviderArgs</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">

The set of arguments for constructing a Provider.

<h3 class="pdoc-member-header" id="ProviderArgs-cluster">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/a33e855465c06a2921aead18ba9f84519baacfd7/sdk/nodejs/provider.ts#L32">property <b>cluster</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>cluster?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>

If present, the name of the kubeconfig cluster to use.

</div>
<h3 class="pdoc-member-header" id="ProviderArgs-context">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/a33e855465c06a2921aead18ba9f84519baacfd7/sdk/nodejs/provider.ts#L36">property <b>context</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>context?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>

If present, the name of the kubeconfig context to use.

</div>
<h3 class="pdoc-member-header" id="ProviderArgs-kubeconfig">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/a33e855465c06a2921aead18ba9f84519baacfd7/sdk/nodejs/provider.ts#L40">property <b>kubeconfig</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>kubeconfig?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>

The contents of a kubeconfig file. If this is set, this config will be used instead of $KUBECONFIG.

</div>
<h3 class="pdoc-member-header" id="ProviderArgs-namespace">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-kubernetes/blob/a33e855465c06a2921aead18ba9f84519baacfd7/sdk/nodejs/provider.ts#L44">property <b>namespace</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>namespace?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>

If present, the namespace scope to use.

</div>
</div>
