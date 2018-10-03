{% macro show_main_text() %}
<div id="main">

<div id="title">

</div>
<div id="body">

<tip-box>

Overview: <include src="project-timeline.md#mid-v12-overview" inline />
</tip-box>

<div id="product">

**<big>Project Management:</big>**

:bulb: **You are free to adjust _process rigor_ and _project plan_ at any future time in the project**, starting from v1.2. If you are not sure if a certain adjustment is allowed, you can check with the teaching team first.
</box>

* **Switch to AB-3 or AB-2 if AB-4 is not working out for you**.  There is no explicit penalty for switching to a lower level AB. All projects are evaluated based on the same yardstick irrespective of on which AB it is based. As an AB is given to you as a 'free' head-start, a lower level AB gives you a shorter head-start, which means your final product is likely to be less functional than those from teams using AB-4 unless you progress faster than them. Nevertheless, you should switch to AB2/3 if you feel you can learn more from the project that way, as our goal is to maximize learning, not features.<br>
  If your team wants to stay with AB-4 but you want to switch to a lower level AB, let the us know so that we can work something out for you.

<div class="indented-level2">
{{ embed_topic("project-deliverables.md#notes-for-ab23", "Admin " + icon_embedding + " Project Deliverables → Notes for Those Using AB-2 or AB-3 for the Project", "midv12-notesForAb23", "3") }}

</div>

* **Complete the repo set up.**
  * Fix any errors in org/repo set up %%&nbsp;(e.g. wrong repo name)%%.
  * Set up [auto-publishing of docs](https://nus{{ module | lower }}-{{ semester | lower }}.github.io/addressbook-level4/UsingTravis.html#enabling-auto-publishing-of-documentation) if you haven't done so already

* **Adjust project rigor to suit your team's pace**, as explained below. Note that you are free to do similar adjustments at any future time in the project.

  * **Automated tests** have benefits, but they can be a pain to write/maintain; GUI tests are especially hard to maintain because their behavior can sometimes depend on things such as the OS, resolution etc.
  
    It is OK to get rid of some of the troublesome tests and rely more on manual testing instead. The less automated test coverage you have, the higher the risk of regressions; but it may be an acceptable trade-off under the circumstances if tests are slowing you down too much. <br> 
    There is no direct penalty for removing GUI tests.   
    Also note <trigger trigger="click" for="modal:v12-testingExpectations">our expectation on test code</trigger>. 
    
  * **Automated checks**: You can also reduce the rigor of checkstyle checks to expedite PR processing.
  
  * **Workflow**: Though you are _recommended_ to **follow the forking workflow** when evolving the product, you can switch to a simpler workflow if the forking workflow is slowing you down. 

<modal title="Admin {{ icon_embedding }} Project Asessement → Expectation on testing" id="modal:v12-testingExpectations">
  <include src="project-testing.fr#expectations"/>
</modal>


* **Adjust project plan if necessary**, as explained below. Note that you are free to do similar adjustments at any future time in the project.
  * Now that you have a some idea about the code base, revisit the feature release plan and adjust it if necessary. The adjustment can be done using GitHub issue tracker. 
  
* **Set up the issue tracker** as described in <trigger trigger="click" for="modal:v12-issueTracker">[Admin {{ icon_embedding }} Appendix E: GitHub: Issue Tracker Setup]</trigger>, if you haven't done so already. Update it to reflect the current project plan.

* **Start proper milestone management**
  * {{ icon_important_big_red }} Starting from the upcoming milestone, ==there are additional requirements to follow== regarding how you **use GitHub to manage your milestones**, as described in <trigger trigger="click" for="modal:v12-projectTracking">[Admin {{ icon_embedding }} Appendix E: GitHub: Project Schedule Tracking]</trigger>.

<modal large title="Admin {{ icon_embedding }} Appendix E: Github: Setting Up Issue Tracker" id="modal:v12-issueTracker">
  <include src="appendixE-gitHub.md#issue-tracker-setup"/>
</modal>
<modal large title="Admin {{ icon_embedding }} Appendix E: Github: Project Schedule Tracking" id="modal:v12-projectTracking">
  <include src="appendixE-gitHub.md#project-schedule-tracking"/>
</modal>

**<big>Product:</big>**

* **From v1.2 onwards each member is expected to contribute <tooltip content="the amount of code does not matter; even small contributions are acceptable">some</tooltip> code to each <tooltip content="v1.3, v1.4"> milestone</tooltip>, preferably each week; only merged code is considered as contributions** %%<popover content="The ability to deliver code incrementally is an important LO of this module because incremental delivery improves the _visibility_ of your work.">(Reason)</popover>%%. <br>
 If an enhancement is too big to complete in one milestone, try to deliver it in smaller incremental steps e.g. deliver a basic version of the enhancement first. 


</div>

</div>

</div>
{% endmacro %}

{% from "common/macros.njk" import embed_topic with context %}
{% from "common/admin.njk" import show_admin_page with context %}
{{ show_admin_page("project-w08-mid-v12", show_main_text) }}