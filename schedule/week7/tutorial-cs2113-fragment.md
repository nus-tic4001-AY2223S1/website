{% from "common/macros.njk" import embed_topic, step, thumb, show_as_tab, timing_badge with context %}
{% from "common/topics.njk" import panopto, slugify, topic_followup, topic_preamble with context %}

{% call topic_preamble(reuse=false) %}
By the end of this tutorial, we want to confirm that you are able to apply Git and GitHub techniques you learned so far to **follow a systematic workflow when updating the code**.
{% endcall %}
<p/>

#### {{ thumb(1) }} Set up tP org/repo

<include src="../../admin/common-tutorials-fragment.md#setup-tp-org-repo" />

#### {{ thumb(2) }} Update the code using the forking workflow

<include src="../../admin/common-tutorials-fragment.md#update-code-using-forking-workflow" />

{% call topic_followup(reuse=false) %}
The workflow you followed above is very safe but has a high-overhead. You may simplify your workflow (at your own risk) after following the above workflow for a while.
{% endcall %}
<p/>
