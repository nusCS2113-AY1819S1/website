{% macro show_main_text() %}
<div id="main">

<div id="title">

</div>
<div id="body">

<tip-box>

Overview: <include src="project-timeline.md#v13-overview" inline />
</tip-box>

**v1.3 Summary of Milestone**

Milestone | Minimum acceptable performance to consider as 'reached'
--------- | -------------------------------------------------------
{{ icon_individual }} Contributed code to v1.3 | code merged
{{ icon_team }} v1.3 jar file released properly on GitHub | as stated
{{ icon_team }} v1.3 milestone properly wrapped up on GitHub | as stated
{{ icon_team }} Documentation updated to match v1.3 | at least the User Guide and the `README.adoc` is updated

### v1.3 Project Management

<tip-box>

**Updated Instructions**

{{ icon_important_big_red }} We will depend on Reposense for identifying your code contribution. ==At the moment, you are **NOT** required to collate your code==. However, the teaching team will monitor Reposense for another week and confirm via an announcement.

</tip-box>

### v1.3 Product

* As before, move the product towards v2.0.

  **Submission**: Push the code to GitHub.

### v1.3 Documentation

<tip-box>

{{ icon_important_big_red }} v1.3 user guide should be updated to match the current version of the product. %%&nbsp;Reason: v1.3 will be subjected to a trial _acceptance testing_ session%%
  
</tip-box>

* **README page**: Update to look like a real product (rather than a project for learning SE) if you haven't done so already. In particular,
  * ==Describe the profile of the target user==
  * Remove irrelevant content such as _Learning Outcomes_
  * ==Update the `Ui.png` to match the current product==
  
* **User Guide**: ==This document will be used by acceptance testers==. Update to match the current version. In particular,
  * Clearly indicate which features are not implemented yet %%&nbsp;e.g. tag those features with a `Coming in v2.0`%%. 
  * For those features already implemented, ensure their descriptions match the exact behavior of the product %%&nbsp;e.g. replace mockups with actual screenshots%% 
 
* **Developer Guide**: As before, update if necessary.
  
* **AboutUs page**: Update to reflect current state of roles and responsibilities.  

**Submission**: Must be included in the version tagged `v1.3`.


### v1.3 Demo

* Optional. If you want feedback on your features, you can demo the feature and get feedback from the tutor.


### v1.3 Testing (PE-1)

=={{ icon_important_big_red }} See info in the panel below==

{{ embed_topic("project-deliverables.md#project-deliverables-practicalexam-dry-run", "Admin " + icon_embedding + " Project Deliverables → **Practical Exam - Round 1**", "v13-peDryRun", "1") }}
  
</div>
</div>
{% endmacro %}

{% from "common/macros.njk" import embed_topic with context %}
{% from "common/admin.njk" import show_admin_page with context %}
{{ show_admin_page("project-w11-v13", show_main_text) }}