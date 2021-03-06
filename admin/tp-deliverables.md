{% from "common/macros.njk" import embed_topic with context %}
{% from "common/admin.njk" import show_admin_page with context %}

{% call show_admin_page("tp-deliverables") %}
<div id="main">

Here is a list of main deliverables of the project; their details are given in the subsequent sections.
* Product
  * [Executable](#deliverable-executable)
  * [Source code](#deliverable-source-code)
* Documentation
  * [User Guide](#deliverable-user-guide-ug)
  * [Developer Guide](#deliverable-developer-guide-dg)
  * [Product Website](#deliverable-product-website)
  * [Project Portfolio Page (PPP)](#deliverable-project-portfolio-page-ppp)
* [Product Demo](#deliverable-demo)


### <div class="text-white bg-info p-1">Deliverable: Executable</div>
<span id="tp-deliverables-executable">
<include src="tp-deliverables-executable-fragment.md" />
</span>

### <div class="text-white bg-info p-1">Deliverable: Source code</div>
<span id="tp-deliverables-sourcecode">
<include src="tp-deliverables-sourcecode-fragment.md" />
</span>

### <div class="text-white bg-info p-1">Deliverable: User Guide (UG)</div>
<span id="tp-deliverables-ug">
<include src="tp-deliverables-ug-fragment.md" />
</span>

### <div class="text-white bg-info p-1">Deliverable: Developer Guide (DG)</div>
<span id="tp-deliverables-dg">
<include src="tp-deliverables-dg-fragment.md" />
</span>

### <div class="text-white bg-info p-1">Deliverable: Product Website</div>
<span id="tp-deliverables-website">
<include src="tp-deliverables-website-fragment.md" />
</span>

### <div class="text-white bg-info p-1">Deliverable: Project Portfolio Page (PPP)</div>
<span id="tp-deliverables-ppp">
<include src="tp-deliverables-ppp-fragment.md" />
</span>

### <div class="text-white bg-info p-1">Deliverable: Demo</div>
<span id="tp-deliverables-demo">
<include src="tp-deliverables-demo-fragment.md" />
</span>

</div>

{% endcall %}
