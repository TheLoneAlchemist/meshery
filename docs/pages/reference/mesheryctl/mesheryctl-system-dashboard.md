---
layout: default
title: mesheryctl-system-dashboard
permalink: reference/mesheryctl/system/dashboard
redirect_from: reference/mesheryctl/system/dashboard/
type: reference
display-title: "false"
language: en
command: system
subcommand: dashboard
---

# mesheryctl system dashboard

Open Meshery UI in browser.

<pre class='codeblock-pre'>
<div class='codeblock'>
mesheryctl system dashboard [flags]

</div>
</pre> 

## Examples

Open Meshery UI in browser
<pre class='codeblock-pre'>
<div class='codeblock'>
mesheryctl system dashboard

</div>
</pre> 

Open Meshery UI in browser and use port-forwarding (if default port is taken already)
<pre class='codeblock-pre'>
<div class='codeblock'>
mesheryctl system dashboard --port-forward

</div>
</pre> 

Open Meshery UI in browser and use port-forwarding, listen on port 9081 locally, forwarding traffic to meshery server in the pod
<pre class='codeblock-pre'>
<div class='codeblock'>
mesheryctl system dashboard --port-forward -p 9081

</div>
</pre> 

(optional) skip opening of MesheryUI in browser.
<pre class='codeblock-pre'>
<div class='codeblock'>
mesheryctl system dashboard --skip-browser

</div>
</pre> 

<pre class='codeblock-pre'>
<div class='codeblock'>
Note: Meshery's web-based user interface is embedded in Meshery Server and is available as soon as Meshery starts. The location and port that Meshery UI is exposed varies depending upon your mode of deployment. See accessing \"Meshery UI\" for additional deployment-specific options: https://docs.meshery.io/installation/accessing-meshery-ui.

</div>
</pre> 

## Options

<pre class='codeblock-pre'>
<div class='codeblock'>
  -h, --help           help for dashboard
  -p, --port int       (optional) Local port that is not in use from which traffic is to be forwarded to the server running inside the Pod. (default 9081)
      --port-forward   (optional) Use port forwarding to access Meshery UI
      --skip-browser   (optional) skip opening of MesheryUI in browser.

</div>
</pre>

## Options inherited from parent commands

<pre class='codeblock-pre'>
<div class='codeblock'>
      --config string    path to config file (default "/home/runner/.meshery/config.yaml")
  -c, --context string   (optional) temporarily change the current context.
  -v, --verbose          verbose output
  -y, --yes              (optional) assume yes for user interactive prompts.

</div>
</pre>


{% include mesheryctl/system-dashboard.md %}
## See Also

Go back to [command reference index](/reference/mesheryctl/), if you want to add content manually to the CLI documentation, please refer to the [instruction](/project/contributing/contributing-cli#preserving-manually-added-documentation) for guidance.
