<div class="section" id="module-pulumi_gcp.cloudbuild">
<span id="cloudbuild"></span><h1>cloudbuild<a class="headerlink" href="#module-pulumi_gcp.cloudbuild" title="Permalink to this headline">¶</a></h1>
<dl class="class">
<dt id="pulumi_gcp.cloudbuild.Trigger">
<em class="property">class </em><code class="descclassname">pulumi_gcp.cloudbuild.</code><code class="descname">Trigger</code><span class="sig-paren">(</span><em>__name__</em>, <em>__opts__=None</em>, <em>build=None</em>, <em>description=None</em>, <em>filename=None</em>, <em>project=None</em>, <em>substitutions=None</em>, <em>trigger_template=None</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.cloudbuild.Trigger" title="Permalink to this definition">¶</a></dt>
<dd><p>Creates a new build trigger within GCR. For more information, see
[the official documentation](<a class="reference external" href="https://cloud.google.com/container-builder/docs/running-builds/automate-builds">https://cloud.google.com/container-builder/docs/running-builds/automate-builds</a>)
and
[API](<a class="reference external" href="https://godoc.org/google.golang.org/api/cloudbuild/v1#BuildTrigger">https://godoc.org/google.golang.org/api/cloudbuild/v1#BuildTrigger</a>).</p>
<table class="docutils field-list" frame="void" rules="none">
<col class="field-name" />
<col class="field-body" />
<tbody valign="top">
<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
<li><strong>__name__</strong> (<em>str</em>) – The name of the resource.</li>
<li><strong>__opts__</strong> (<em>pulumi.ResourceOptions</em>) – Options for the resource.</li>
<li><strong>build</strong> (<em>pulumi.Input</em><em>[</em><em>dict</em><em>]</em>) – A build resource in the Container Builder API.
Structure is documented below. At a high
level, a <cite>build</cite> describes where to find source code, how to build it (for
example, the builder image to run on the source), and where to store
the built artifacts. Fields can include the following variables, which
will be expanded when the build is created:
* <cite>$PROJECT_ID</cite>: the project ID of the build.
* <cite>$BUILD_ID</cite>: the autogenerated ID of the build.
* <cite>$REPO_NAME</cite>: the source repository name specified by RepoSource.
* <cite>$BRANCH_NAME</cite>: the branch name specified by RepoSource.
* <cite>$TAG_NAME</cite>: the tag name specified by RepoSource.
* <cite>$REVISION_ID</cite> or <cite>$COMMIT_SHA</cite>: the commit SHA specified by RepoSource
or resolved from the specified branch or tag.
* <cite>$SHORT_SHA</cite>: first 7 characters of <cite>$REVISION_ID</cite> or <cite>$COMMIT_SHA</cite>.</li>
<li><strong>description</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – A brief description of this resource.</li>
<li><strong>filename</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Specify the path to a Cloud Build configuration file
in the Git repo. This is mutually exclusive with <cite>build</cite>. This is typically
<cite>cloudbuild.yaml</cite> however it can be specified by the user.</li>
<li><strong>project</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the project that the trigger will be created in.
Defaults to the provider project configuration.</li>
</ul>
</td>
</tr>
</tbody>
</table>
<p>:param pulumi.Input[dict] substitutions
:param pulumi.Input[dict] trigger_template: Location of the source in a Google</p>
<blockquote>
<div>Cloud Source Repository. Structure is documented below.</div></blockquote>
<dl class="attribute">
<dt id="pulumi_gcp.cloudbuild.Trigger.build">
<code class="descname">build</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.cloudbuild.Trigger.build" title="Permalink to this definition">¶</a></dt>
<dd><p>A build resource in the Container Builder API.
Structure is documented below. At a high
level, a <cite>build</cite> describes where to find source code, how to build it (for
example, the builder image to run on the source), and where to store
the built artifacts. Fields can include the following variables, which
will be expanded when the build is created:
* <cite>$PROJECT_ID</cite>: the project ID of the build.
* <cite>$BUILD_ID</cite>: the autogenerated ID of the build.
* <cite>$REPO_NAME</cite>: the source repository name specified by RepoSource.
* <cite>$BRANCH_NAME</cite>: the branch name specified by RepoSource.
* <cite>$TAG_NAME</cite>: the tag name specified by RepoSource.
* <cite>$REVISION_ID</cite> or <cite>$COMMIT_SHA</cite>: the commit SHA specified by RepoSource
or resolved from the specified branch or tag.
* <cite>$SHORT_SHA</cite>: first 7 characters of <cite>$REVISION_ID</cite> or <cite>$COMMIT_SHA</cite>.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.cloudbuild.Trigger.description">
<code class="descname">description</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.cloudbuild.Trigger.description" title="Permalink to this definition">¶</a></dt>
<dd><p>A brief description of this resource.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.cloudbuild.Trigger.filename">
<code class="descname">filename</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.cloudbuild.Trigger.filename" title="Permalink to this definition">¶</a></dt>
<dd><p>Specify the path to a Cloud Build configuration file
in the Git repo. This is mutually exclusive with <cite>build</cite>. This is typically
<cite>cloudbuild.yaml</cite> however it can be specified by the user.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.cloudbuild.Trigger.project">
<code class="descname">project</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.cloudbuild.Trigger.project" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the project that the trigger will be created in.
Defaults to the provider project configuration.</p>
</dd></dl>

<dl class="attribute">
<dt id="pulumi_gcp.cloudbuild.Trigger.trigger_template">
<code class="descname">trigger_template</code><em class="property"> = None</em><a class="headerlink" href="#pulumi_gcp.cloudbuild.Trigger.trigger_template" title="Permalink to this definition">¶</a></dt>
<dd><p>Location of the source in a Google
Cloud Source Repository. Structure is documented below.</p>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.cloudbuild.Trigger.translate_output_property">
<code class="descname">translate_output_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.cloudbuild.Trigger.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
</dd></dl>

<dl class="method">
<dt id="pulumi_gcp.cloudbuild.Trigger.translate_input_property">
<code class="descname">translate_input_property</code><span class="sig-paren">(</span><em>prop</em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_gcp.cloudbuild.Trigger.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
</dd></dl>

</dd></dl>

</div>