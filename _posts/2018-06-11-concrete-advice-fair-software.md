---
ID: 175
post_title: Concrete Advice for FAIR Software
author: Katrin Leinweber
post_excerpt: ""
layout: post
permalink: >
  http://genr-updraft.consortium.io/concrete-advice-fair-software/
published: true
post_date: 2018-06-11 09:00:10
---
<!-- wp:image {"id":398,"align":"center"} -->
<figure class="wp-block-image aligncenter"><img src="http://genr.eu/wp/wp-content/uploads/2018/06/mms01.jpg" alt="" class="wp-image-398" />
	<figcaption>Video screen grab from <a href="https://av.tib.eu/series/415/the+leibniz+mathematical+modeling+and+simulation+mms+days+2018" rel="noopener">The Leibniz "Mathematical Modeling and Simulation" (MMS) Days 2018</a> Leipzig, Feb / Mar 2018. (The video can be viewed at the bottom of the article)</figcaption>
</figure>
<!-- /wp:image -->

<!-- wp:block {"ref":341} /-->

<!-- wp:block {"ref":172} /-->

<!-- wp:block {"ref":761} /-->

<!-- wp:heading -->
<h2>Findability Through Persistent Identifiers</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>In addition to implementing <a href="https://www.force11.org/group/fairgroup/fairprinciples" target="_blank">the FAIR Data Principles for research data</a> there is a need to support the sustainable development, use, and publication of research software. This blog post represents an interim status of the development of these competences.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>In addition, it shall introduce a series of articles, which <a href="https://blogs.tib.eu/wp/tib/2017/09/12/the-fair-data-principles-for-research-data/">similarly to the already explained FAIR Data Principles for research data</a> (Kraft 2017) will recommend: concrete examples and actions to scientific software projects, summarizes specialist literature (see the <a href="http://genr.eu/wp/concrete-advice-fair-software#bibliography">bibliography﻿</a>), and also sets goals for our own software projects and those we supports.</p>
<!-- /wp:paragraph -->

<!-- wp:more -->
<!--more-->
<!-- /wp:more -->

<!-- wp:paragraph -->
<p>In the various thematic sections some of the recommendations are addressed separately to scientists and their institutions. In either case they are ranked roughly in the following order:</p>
<!-- /wp:paragraph -->

<!-- wp:list {"className":"list-content"} -->
<ol class="list-content">
	<li><em>low-hanging fruit</em>,</li>
	<li><em>next achievable step</em>,</li>
	<li><em>solid 80% solution</em>, and</li>
	<li><em>really good implementation</em>,</li>
</ol>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p>and imbued with these <em>connotations</em> of being realised. Of course, they should also be understood as a basis for discussion, which is why we are very happy about comments, questions, suggestions, criticism, and reports of experience, etc.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>We'll use the FAIR Data Principles for orientation purposes:</p>
<!-- /wp:paragraph -->

<!-- wp:list {"className":"list-content"} -->
<ul class="list-content">
	<li>Findable</li>
	<li>Accessible</li>
	<li>Interoperable</li>
	<li>Reusable</li>
</ul>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p>For this article we'll focus on the first of the FAIR principles:</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2><strong>F – F</strong>indable</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><a href="https://blogs.tib.eu/wp/tib/2017/09/12/the-fair-data-principles-for-research-data/#f">Analogous to research data</a> we can say that software should be easy to find for both people and computer systems. Basic machine-readable descriptive metadata enable the discovery of interesting software programs and services. In view of this first principle, indeed only minor differences (if any) need to be drawn between finding datasets and software.</p>
<!-- /wp:paragraph -->

<!-- wp:separator -->
<hr class="wp-block-separator" />
<!-- /wp:separator -->

<!-- wp:heading -->
<h3>F1. Software projects receive a globally unique and permanently persistent identifier</h3>
<!-- /wp:heading -->

<!-- wp:heading -->
<h4>What does that mean?</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Each software project should be represented on the Internet under a globally unique and persistent identifier (PID). This can be, for example, a Uniform Resource Locator (URL), or a Digital Object Identifier (DOI), so that software and metadata can be found and referred to. Principle F1 can be classified as the most important, as it is difficult to comply with the other FAIR principles without "globally unique and persistent identifiers".</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h4>FAIR Software — The scientist's role</h4>
<!-- /wp:heading -->

<!-- wp:list {"className":"list-content"} -->
<ol class="list-content">
	<li>If a software project does not already have its own website, a rudimentary one can be created by means of (an account and) a repository on a <a href="https://en.wikipedia.org/wiki/Comparison_of_source_code_hosting_facilities" target="_blank">code hosting platform</a>. Since <a href="https://git-scm.com/" target="_blank">Git</a> is the most widely used source code management program, its use in combination with <a href="https://github.com/" target="_blank">GitHub</a> as the most popular code hosting platform is advised. This already creates a globally unique URL under which the software is found.</li>
	<li>Since a GitHub repo (abbreviation for "repository") <a href="https://guides.github.com/activities/citable-code/" target="_blank">can officially be integrated</a> with <a href="https://about.zenodo.org/" target="_blank">Zenodo</a>, a DOI and a landing page can be generated as favored by the Software Citation Principles (Smith 2016). This means that the project can be cited globally and persistently. As a bonus Zenodo also grabs a backup copy automatically, and repeatedly for each subsequent <a href="https://help.github.com/articles/about-releases/" target="_blank">release</a> version. The <a href="http://help.osf.io/m/addons/l/524149-storage-add-ons" target="_blank">Open Science Framework</a>, and the Project <a href="https://science.mozilla.org/blog/code-as-a-research-object-updates-prototypes-next-steps" target="_blank">"Code as a Research Object" by the Mozilla Science Labs</a> offer similar functionality. The latter primarily uses FigShare, against whose <a href="https://blogs.tib.eu/wp/tib/?s=LZA+Langzeitarchivierung" target="_blank">long-term archiving</a> one <a href="https://doi.org/10.6084/M9.FIGSHARE.1381402" target="_blank">may have reservations</a>. Even if a record has been deleted, its metadata should still be displayed AKA a "tombstone" page. Unfortunately, FigShare doesn't so this at the moment, and leaves the data grave unmarked, so to speak. Besides Zenodo's auto-backup option, Git repos can also be downloaded manually, and submitted to generic <a href="https://www.re3data.org/search?contentTypes%5B%5D=Software%20applications&amp;contentTypes%5B%5D=Source%20code" target="_blank">research data repositories</a> such as <a href="https://www.radar-service.eu/" target="_blank">RADAR</a>, where they are archived and citable.</li>
	<li>DOIs should only be assigned to objects that have found a <em>long term</em> digital home. In order to identify drafts, pre-releases etc., an <a href="https://en.wikipedia.org/wiki/Archival_Resource_Key" target="_blank">Archival Resource Key (ARK)</a> can be used. Here is the list of <a href="https://www.cdlib.org/uc3/naan_table.html" target="_blank">ARK-issuing institutions</a>.</li>
	<li>Step 2 might even be omitted, once <a href="https://www.softwareheritage.org/" target="_blank">SoftwareHeritage.org</a> will be broadly available! This "ambitious initiative for the collection, preservation and joint management of the entire corpus of publicly accessible software source code". (DiCosmo 2017), might make citation software as easy as possible (Katz 2017). Software Heritage automatically creates persistent IDs (PIDs), so that a source code repo becomes citable as soon as it is published.</li>
</ol>
<!-- /wp:list -->

<!-- wp:heading -->
<h4>FAIR Software — The institution's role</h4>
<!-- /wp:heading -->

<!-- wp:list {"className":"list-content"} -->
<ol class="list-content">
	<li>Scientific institutions should provide their members with alternatives to popular, centralized platforms for <a href="https://en.wikipedia.org/wiki/Comparison_of_source_code_hosting_facilities#Version_control_systems" target="_blank">modern Source Code Hosting</a> (like e.g. <a href="https://git.tib.eu/users/sign_in">git.TIB.eu</a>), and guarantee their long-term availability.</li>
	<li>To make such decentralized source code platforms more attractive, institutions should tick all the functional completeness checkboxes (<a href="https://docs.gitlab.com/ce/user/project/pages/index.html" target="_blank">Pages</a>, <a href="https://docs.gitlab.com/ce/ci/quick_start/README.html" target="_blank">CI</a>, etc.) and ensure that the system is kept up to date. They should also ensure their public accessibility (as for example at the <a href="https://git.universitaetskolleg.uni-hamburg.de/explore/projects" target="_blank">University College Hamburg</a>) or in the <a href="https://gitlab.informatik.uni-bremen.de/explore/projects" target="_blank">Department of Computer Science at the university of Bremen</a>), so that the project URLs can be used as public identifiers. Thankfully, GitLab supports persistence. If a user, group or repo name is changed, almost all necessary <a href="https://docs.gitlab.com/ce/user/project/index.html#redirects-when-changing-repository-paths" target="_blank">URL redirections are set up automatically</a>. Although such <a href="https://en.wikipedia.org/wiki/URL_redirection" target="_blank">URL redirects</a> don't attain the same level of persistence as described by <a href="https://de.wikipedia.org/wiki/Uniform_Resource_Name" target="_blank">URNs</a> or <a href="https://de.wikipedia.org/wiki/Persistent_Uniform_Resource_Locator" target="_blank">PURLs</a>, redirected project URLs also play their part in ensuring the findability of digital objects by people and search engine crawlers.</li>
	<li>Similar to the <a href="https://guides.github.com/activities/citable-code/" target="_blank">Zenodo-DOI-ification of GitHub repos</a> also institutional platforms should offer DOI registration services, preferably by the <a href="https://about.gitlab.com/development/" target="_blank">sponsoring</a> of corresponding Free <a href="https://github.com/zenodo/zenodo/issues/1404" target="_blank">Software</a> <a href="https://gitlab.com/gitlab-org/gitlab-ce/issues/35023" target="_blank">modules</a>.</li>
	<li>Institutions that run their own code hosting should prepare its integration with <a href="https://www.softwareheritage.org/2017/03/24/list-the-content-of-your-favorite-forge-in-just-a-few-steps/" target="_blank">SoftwareHeritage.org</a> in order to simplify citation of the works of their members.</li>
	<li>Even if an institution's software projects are scattered across different hosting platforms, there is a remedy. A tool like <a href="https://www.osti.gov/doecode/" target="_blank">DOE Code</a> (<a href="https://github.com/doecode" target="_blank">source code</a>) can provide the developers a central archive, and place to search.</li>
</ol>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p>Thanks for reading! This was some introductory advice on how to make research software projects more sustainable, and especially improve their discoverability by means of persistent identifiers (PIDs). As mentioned, we welcome your comments, questions, suggestions, criticism, experience reports etc. Soon this series will continue with other concrete advice for <a href="https://blogs.tib.eu/wp/tib/2017/09/12/the-fair-data-principles-for-research-data/" target="_blank">FAIR</a>er scientific software.</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2 id="bibliography">Bibliography</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Di Cosmo, Roberto, and Stefano Zacchiroli. 2017. "Software Heritage: Why and How to Preserve Software's Source Code" In <em>iPRES 2017: 14th International Conference on Digital Preservation</em>. Kyoto, Japan. <a href="https://hal.archives-ouvertes.fr/hal-01590958/document" target="_blank">https://hal.archives-ouvertes.fr/hal-01590958/document</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Katz, Daniel S. 2017. "Software Heritage and Repository Metadata: A Software Citation Solution" Daniel S. Katz's Blog. September 25, 2017. <a href="https://danielskatzblog.wordpress.com/2017/09/25/software-heritage-and-repository-metadata-a-software-citation-solution/" target="_blank">https://danielskatzblog.wordpress.com/2017/09/25/software-heritage-and-repository-metadata-a-software-citation-solution/</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Kraft, Angelina. 2017. "The FAIR Data Principles For Research Data" TIB Blog. September 12, 2017. <a href="https://blogs.tib.eu/wp/tib/2017/09/12/the-fair-data-principles-for-research-data/" target="_blank">https://blogs.tib.eu/wp/tib/2017/09/12/the-fair-data-principles-for-research-data/</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Smith, Arfon M., Daniel S. Katz, and Kyle E. Niemeyer. 2016. "Software Citation Principles" <em>PeerJ Computer Science</em> 2 (September): e86. <a href="https://doi.org/10.7717/peerj-cs.86" target="_blank">https://doi.org/10.7717/peerj-cs.86﻿</a></p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>Video (supplementary material)</h2>
<!-- /wp:heading -->

<!-- wp:html -->
<iframe width="840" height="472" scrolling="no" src="//av.tib.eu/player/35351#t=00:08" frameborder="0" allowfullscreen=""></iframe>
<!-- /wp:html -->

<!-- wp:paragraph {"backgroundColor":"very light gray"} -->
<p class="has-background has-very-light-gray-background-color"><em><strong>If the above space is blank</strong> please disable your tracker blocker for this page, 'These aren't the droids you're looking for...'</em></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Video from <a href="https://av.tib.eu/series/415/the+leibniz+mathematical+modeling+and+simulation+mms+days+2018">The Leibniz "Mathematical Modeling and Simulation" (MMS) Days 2018</a> Leipzig, Feb / Mar 2018</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><a href="http://tib.flowcenter.de/mfc/medialink/3/de244013a88953b0e43b182074ef451d68fd177709456664ff26b4d6de9b063ff8/180301-Leibniz-MMS-Days-software-citation-Katrin-Leinweber-TIB.PDF">Slides</a> as PDF</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Video DOI: <a href="https://doi.org/10.5446/35351">https://doi.org/10.5446/35351</a> from TIB AV Portal</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>
	Leinweber, Katrin. ‘Killed By A Thousand Paper Cuts? A Newcomer’s Perspective On Possibilities And Gaps In Software Citation Workflows’. Weierstraß-Institut für Angewandte Analysis und Stochastik (WIAS),Technische Informationsbibliothek (TIB), 2018. <a href="https://doi.org/10.5446/35351">https://doi.org/10.5446/35351</a>.

</p>
<!-- /wp:paragraph -->

<!-- wp:html -->
<div class="wp-block-atomic-blocks-ab-accordion ab-block-accordion ab-font-size-18">
	<details open="">
		<summary class="ab-accordion-title">
			<p>DOI: 10.25815/d6c3-md17</p>
		</summary>
		<p class="ab-accordion-text">Citation format:&nbsp;<em>The Chicago Manual of Style, 17th Edition</em> <br><br>Leinweber, Katrin. ‘Concrete Advice for FAIR Software’, 2018. https://doi.org/10.25815/D6C3-MD17<br></p>
	</details>
</div>
<!-- /wp:html -->