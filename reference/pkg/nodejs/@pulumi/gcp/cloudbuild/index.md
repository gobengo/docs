---
title: Module cloudbuild
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->

<a href="../index.html">@pulumi/gcp</a> &gt; cloudbuild

<div class="toggleVisible" markdown="1">
<div class="collapsed" markdown="1">
<h2 class="pdoc-module-header toggleButton" title="Click to show Index">Index ▹</h2>
</div>
<div class="expanded" markdown="1">
<h2 class="pdoc-module-header toggleButton" title="Click to hide Index">Index ▾</h2>
<div class="pdoc-module-contents" markdown="1">
* <a href="#Trigger">class Trigger</a>
* <a href="#TriggerArgs">interface TriggerArgs</a>
* <a href="#TriggerState">interface TriggerState</a>

<a href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts">cloudbuild/trigger.ts</a> 
</div>
</div>
</div>


<h2 class="pdoc-module-header" id="Trigger">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L37">class <b>Trigger</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">
<pre class="highlight"><span class='kd'>extends</span> <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#CustomResource'>CustomResource</a></pre>

Configuration for an automated build in response to source repository changes.

To get more information about Trigger, see:

* [API documentation](https://cloud.google.com/cloud-build/docs/api/reference/rest/)
* How-to Guides
    * [Automating builds using build triggers](https://cloud.google.com/cloud-build/docs/running-builds/automate-builds)

## Example Usage - Cloudbuild Trigger Filename


```typescript
import * as pulumi from "@pulumi/pulumi";
import * as gcp from "@pulumi/gcp";

const filename_trigger = new gcp.cloudbuild.Trigger("filename-trigger", {
    filename: "cloudbuild.yaml",
    substitutions: {
        _BAZ: "qux",
        _FOO: "bar",
    },
    triggerTemplate: {
        branchName: "master",
        repoName: "my-repo",
    },
});
```

<h3 class="pdoc-member-header" id="Trigger-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L64"> <b>constructor</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">

<pre class="highlight"><span class='kd'></span><span class='kd'>new</span> Trigger(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, args?: <a href='#TriggerArgs'>TriggerArgs</a>, opts?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>)</pre>


Create a Trigger resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

</div>
<h3 class="pdoc-member-header" id="Trigger-get">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L46">method <b>get</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">

<pre class="highlight"><span class='kd'>public static </span>get(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, id: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#ID'>pulumi.ID</a>&gt;, state?: <a href='#TriggerState'>TriggerState</a>, opts?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>): <a href='#Trigger'>Trigger</a></pre>


Get an existing Trigger resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

</div>
<h3 class="pdoc-member-header" id="Trigger-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L14">method <b>getProvider</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">

<pre class="highlight"><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): ProviderResource | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></pre>

</div>
<h3 class="pdoc-member-header" id="Trigger-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L101">method <b>isInstance</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">

<pre class="highlight"><span class='kd'>static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span></pre>


Returns true if the given object is an instance of CustomResource.  This is designed to work even when
multiple copies of the Pulumi SDK have been loaded into the same process.

</div>
<h3 class="pdoc-member-header" id="Trigger-build">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L50">property <b>build</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'>public </span>build: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Output'>pulumi.Output</a>&lt;{
    images: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>[];
    steps: {
        args: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>[];
        name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;
    }[];
    tags: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>[];
} | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="Trigger-createTime">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L51">property <b>createTime</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'>public </span>createTime: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="Trigger-description">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L52">property <b>description</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'>public </span>description: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="Trigger-disabled">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L53">property <b>disabled</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'>public </span>disabled: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="Trigger-filename">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L54">property <b>filename</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'>public </span>filename: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="Trigger-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L96">property <b>id</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>id: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Output'>Output</a>&lt;<a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#ID'>ID</a>&gt;;</pre>

id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

</div>
<h3 class="pdoc-member-header" id="Trigger-ignoredFiles">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L55">property <b>ignoredFiles</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'>public </span>ignoredFiles: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>[] | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="Trigger-includedFiles">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L56">property <b>includedFiles</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'>public </span>includedFiles: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>[] | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="Trigger-project">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L61">property <b>project</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'>public </span>project: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>

The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.

</div>
<h3 class="pdoc-member-header" id="Trigger-substitutions">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L62">property <b>substitutions</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'>public </span>substitutions: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Output'>pulumi.Output</a>&lt;{[key: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>]: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>} | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="Trigger-triggerId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L63">property <b>triggerId</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'>public </span>triggerId: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="Trigger-triggerTemplate">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L64">property <b>triggerTemplate</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'>public </span>triggerTemplate: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Output'>pulumi.Output</a>&lt;{
    branchName: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;
    commitSha: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;
    dir: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;
    projectId: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;
    repoName: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;
    tagName: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>;
} | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="Trigger-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L12">property <b>urn</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>urn: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Output'>Output</a>&lt;<a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#URN'>URN</a>&gt;;</pre>

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

</div>
</div>
<h2 class="pdoc-module-header" id="TriggerArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L131">interface <b>TriggerArgs</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">

The set of arguments for constructing a Trigger resource.

<h3 class="pdoc-member-header" id="TriggerArgs-build">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L132">property <b>build</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>build?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{
    images: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;
    steps: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{
        args: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;
        name: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
    }&gt;[]&gt;;
    tags: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;
}&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="TriggerArgs-description">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L133">property <b>description</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>description?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="TriggerArgs-disabled">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L134">property <b>disabled</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>disabled?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="TriggerArgs-filename">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L135">property <b>filename</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>filename?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="TriggerArgs-ignoredFiles">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L136">property <b>ignoredFiles</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>ignoredFiles?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="TriggerArgs-includedFiles">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L137">property <b>includedFiles</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>includedFiles?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="TriggerArgs-project">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L142">property <b>project</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>project?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>

The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.

</div>
<h3 class="pdoc-member-header" id="TriggerArgs-substitutions">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L143">property <b>substitutions</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>substitutions?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{[key: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>]: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;}&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="TriggerArgs-triggerTemplate">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L144">property <b>triggerTemplate</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>triggerTemplate?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{
    branchName: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
    commitSha: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
    dir: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
    projectId: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
    repoName: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
    tagName: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
}&gt;;</pre>
</div>
</div>
<h2 class="pdoc-module-header" id="TriggerState">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L110">interface <b>TriggerState</b></a>
</h2>
<div class="pdoc-module-contents" markdown="1">

Input properties used for looking up and filtering Trigger resources.

<h3 class="pdoc-member-header" id="TriggerState-build">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L111">property <b>build</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>build?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{
    images: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;
    steps: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{
        args: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;
        name: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
    }&gt;[]&gt;;
    tags: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;
}&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="TriggerState-createTime">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L112">property <b>createTime</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>createTime?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="TriggerState-description">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L113">property <b>description</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>description?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="TriggerState-disabled">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L114">property <b>disabled</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>disabled?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="TriggerState-filename">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L115">property <b>filename</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>filename?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="TriggerState-ignoredFiles">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L116">property <b>ignoredFiles</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>ignoredFiles?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="TriggerState-includedFiles">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L117">property <b>includedFiles</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>includedFiles?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="TriggerState-project">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L122">property <b>project</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>project?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>

The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.

</div>
<h3 class="pdoc-member-header" id="TriggerState-substitutions">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L123">property <b>substitutions</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>substitutions?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{[key: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>]: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;}&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="TriggerState-triggerId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L124">property <b>triggerId</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>triggerId?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
</div>
<h3 class="pdoc-member-header" id="TriggerState-triggerTemplate">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-gcp/blob/65c7a44d62f0ea5edd3833c6f7b1f0c253503f0f/sdk/nodejs/cloudbuild/trigger.ts#L125">property <b>triggerTemplate</b></a>
</h3>
<div class="pdoc-member-contents" markdown="1">
<pre class="highlight"><span class='kd'></span>triggerTemplate?: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{
    branchName: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
    commitSha: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
    dir: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
    projectId: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
    repoName: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
    tagName: <a href='https://pulumi.io/reference/pkg/nodejs/@pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;
}&gt;;</pre>
</div>
</div>
