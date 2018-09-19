---
ID: 168
post_title: 'Open Science #Barcamp: Software Citation'
author: Sophia Dörner
post_excerpt: ""
layout: post
permalink: >
  http://genr-updraft.consortium.io/barcamp-software-citation/
published: true
post_date: 2018-06-25 16:09:16
---
<!-- wp:paragraph {"fontSize":"small"} -->
<p class="is-small-text">Image: Barcamp Open Science, Berlin, March 2018. Photo credits: Bettina Ausserhofer. All photos are also published at <a href="https://commons.wikimedia.org/w/index.php?title=Category:Barcamp_Open_Science" target="_blank">Wiki Commons</a> under the CC BY 4.0 license.</p>
<!-- /wp:paragraph -->

<!-- wp:block {"ref":341} /-->

<!-- wp:block {"ref":172} /-->

<!-- wp:paragraph -->
<p>A report from the <a href="https://etherpad.wikimedia.org/p/oscibar2018_session10">barcamp session</a> on software citation at <a href="https://www.open-science-conference.eu/barcamp/">Barcamp Open Science</a>, Berlin, March 2018.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>The Barcamp Open Science organized by the <a href="http://leibniz-science20.de/en/">Leibniz Research Alliance Science 2.0</a> and hosted by Wikimedia Deutschland was designed as a pre-event before the two day <a href="http://www.open-science-conference.eu/">Open Science Conference</a>. The Barcamp offers a space for discussion, for developing new ideas and knowledge exchange on experiences and best practices in Open Science for researchers and practitioners from various backgrounds, with an emphasis on bringing together novices and experts.</p>
<!-- /wp:paragraph -->

<!-- wp:more -->
<!--more-->
<!-- /wp:more -->

<!-- wp:paragraph -->
<p>Research software is starting to be recognized as a valid research product and tool that calls for independent and proper attribution, and credit within the academic merit-system. Still there is no consistent procedure, let alone standard for software citation that allows the management of research software aligned with the <a href="https://blogs.tib.eu/wp/tib/2017/09/12/die-fair-data-prinzipien-fuer-forschungsdaten/">FAIR principles of research data</a>. The question underlying the discourse can be described as threefold. Why to cite software, what to cite exactly, and how to cite it.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Developments that regard clarification of the first two aspects can be found in the work of the FORCE11 <a href="https://www.force11.org/group/software-citation-working-group" target="_blank" rel="noopener">Software Citation Working Group</a>, which started in early 2015, and completed its work in late 2016 with publishing the <a href="https://peerj.com/articles/cs-86/" target="_blank" rel="noopener">Software Citation Principles</a> (Smith AM et al. 2016). Separately, the Research Software Working Group within the <a href="https://www.allianzinitiative.de/en/" target="_blank" rel="noopener">Alliance of German Science Organisations</a> was established in 2016. Their work resulted in the publication of the <a href="https://zenodo.org/record/1172988" target="_blank" rel="noopener">Recommendations on the Development, Use and Provision of Research Software</a> (Katerbow et al. 2018). The most important software types for these recommendations consist of self-developed research software, software applications for research, and infrastructure software and services. Following the ending of the FORCE11 Software Citation Working Group a new follow-on working group was setup the <a href="https://www.force11.org/group/software-citation-implementation-working-group">Software Citation Implementation Working Group</a> which was set up to tackle the implementation of the Software Citation Principles by developing guidelines and testing implementation scenarios. Thus tackling the aspect of how to cite software by facilitating the development of consistent procedures, tools and suitable workflows.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>The barcamp session on software citation was proposed with the aim to emphasize the importance of the topic in general and to introduce current developments in software citation. The questions that were under discussion were based on the Software Citation Principles, but with a stronger focus on the pragmatic implementation of software citation from a developer and user perspective. In addition, some already existing tools were presented and discussed. The session was attended by around fifteen people affiliated with various research projects and institutions such as <a href="https://www.fokus.fraunhofer.de/en" target="_blank" rel="noopener">Fraunhofer FOKUS</a>, <a href="https://www.tib.eu/en/" target="_blank" rel="noopener">TIB</a>, <a href="http://www.sysmed.uni-wuerzburg.de/en/start/" target="_blank" rel="noopener">Core Unit Systemmedizin</a>, <a href="https://www.ub.uni-bielefeld.de/english/" target="_blank" rel="noopener">Bielefeld University Library</a>, <a href="https://www.hu-berlin.de/en?set_language=en" target="_blank" rel="noopener">Humboldt University Berlin</a>, and others. When asked about the role of software within their research all participants reported that they often come into contact with software within their research either as users or as developer themselves. So, discussing why to cite software it seemed that the overall consensus was that software citation leads to an improved overall research practice, integrity and reproducibility on one hand and makes for better credit for the work of developers on the other, even if they are not publishing a paper or article alongside the software. This also coincides with the examinations and findings of the various working groups of FORCE11, and of the Alliance of German Science Organisations. Whereas the aspect of <strong>what to cite exactly</strong> led to more discussion. First off, it depends on what software, software package, language, library or other component is used in the process of research and how the findings depend on it. Determining what to cite turns out to be difficult regarding the multiple dependencies inherent in software leading also to concerns of <strong>transitive credit</strong>—how to attribute micro-contributions over time. The topic of transitive credit as well as a first step towards a solution has previously been addressed (Katz D.S. 2014)(<a href="http://doi.org/10.5334/jors.by" target="_blank" rel="noopener">Katz D.S. &amp; Smith A.M. 2015</a>). However it is perceived to be most sufficient to cite the software itself as opposed to an affiliated article describing the software. This leaves the question of how to describe software; precisely which metadata fields would be mandatory. As for the barcamp session the metadata fields that led to more elaborate discussion were author, title, version information and persistent identifier as they were perceived as a minimal prerequisite for describing software entities. Overlapping with matters of transitive credit—authorship has been discussed—questioning attribution to: contributor, testers, and managers alike as an issue that needs to be addressed further. As for <strong>persistent identifier</strong> questions that arose and partly could not be answered within the scope of the session were if a repository URL or a commit hash make for a sufficient identifier, also is it suitable to assign an identifier for every release or every commit?</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>As for questions of how to cite software there have already been efforts made to develop services that support researchers with citing software. During the session <a href="https://sdruskat.net/" target="_blank">Stephan Druskat</a> introduced the <a href="https://github.com/citation-file-format/citation-file-format.github.io" target="_blank">Citation File Format</a> in context of discussing dissemination of software metadata. It makes for a sufficient and user-centric way to store software metadata within the codes root directory in a so-called CITATION file. Including mandatory fields the developers preference for citing the software can be passed on directly to the user. Another service that was discussed more extensively was the coupling of <a href="https://guides.github.com/activities/citable-code/" target="_blank">Github with Zenodo</a>. The services both parties have built allows for software that is developed on GitHub to get a backup at the <a href="http://cds.cern.ch/record/1998637" target="_blank">CERN</a> based Zenodo, as well as a DOI minted by Zenodo to make the repository citable. Having a minted DOI and providing CITATION files makes for a sufficient way citing software independent of specifics. However certain communities are engaged as well in making their specific language, software, or library citable. Prominently the <a href="https://www.r-project.org/" target="_blank">R Community</a> provides a citation function for R and R packages—though this is not in alignment with the Software Citation Principles since the function only offers citation information for a manual as opposed to the software itself. For the Python language <a href="https://github.com/duecredit/duecredit" target="_blank">DueCredit</a> offers a framework facilitating citing Python and Python packages. From a user perspective it is may not sufficient to harvest the citation information yourself especially if there are different software entities involved in the research process and metadata are disseminated through different channels and formats. The <a href="http://citeas.org/" target="_blank">CiteAs</a> platform offers a service where it performs web-based searches based on the input of a URL, DOI, or arxivID to create a citation string with additional information of citation provenance. The aim of CiteAs is to provide citation information for all kinds of research products.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>The community is still working on a standard metadata schema but as for now the existing services provide first access points and an improvement software citation. So go on, <strong>cite the software you use</strong> and <strong>make your software citable</strong>. And if you are still not convinced visit <a href="https://research-software.org/citation/" target="_blank" rel="noopener">research-software.org</a> and <a href="https://mr-c.github.io/shouldacite/index.html" target="_blank" rel="noopener">shouldacite</a>.</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>
	References</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Smith AM, Katz DS, Niemeyer KE, FORCE11 Software Citation Working Group. (2016) Software Citation Principles. PeerJ Computer Science 2:e86 <a href="https://doi.org/10.7717/peerj-cs.86" target="_blank" rel="noopener">https://doi.org/10.7717/peerj-cs.86</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Katerbow, Matthias, &amp; Feulner, Georg. (2018, March 16). Recommendations on the development, use and provision of Research Software. Zenodo. <a href="http://doi.org/10.5281/zenodo.1172988" target="_blank" rel="noopener">http://doi.org/10.5281/zenodo.1172988</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Katz, D.S., (2014). Transitive Credit as a Means to Address Social and Technological Concerns Stemming from Citation and Attribution of Digital Products. Journal of Open Research Software . 2 ( 1 ) , p . e20 . DOI: <a href="http://doi.org/10.5334/jors.be" target="_blank" rel="noopener">http://doi.org/10.5334/jors.be</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Katz, D.S. &amp; Smith, A.M., (2015). Transitive Credit and JSON-LD. Journal of Open Research Software . 3 ( 1 ) , p . e7 . DOI: <a href="http://doi.org/10.5334/jors.by" target="_blank" rel="noopener">http://doi.org/10.5334/jors.by</a></p>
<!-- /wp:paragraph -->

<!-- wp:separator -->
<hr class="wp-block-separator" />
<!-- /wp:separator -->

<!-- wp:html -->
<iframe width="600" height="290" src="http://www.openscienceradio.org/wp-content/plugins/podlove-podcasting-plugin-for-wordpress/lib/modules/podlove_web_player/player_v4/dist/share.html?episode=http://www.openscienceradio.org/?podlove_player4=731" frameborder="0" scrolling="no"></iframe>
<!-- /wp:html -->

<!-- wp:paragraph -->
<p>POD cast interview with Sophia Dörner from the barcamp session. Thanks to <a href="http://www.openscienceradio.org" target="_blank">Open Science Radio</a>.</p>
<!-- /wp:paragraph -->

<!-- wp:separator -->
<hr class="wp-block-separator" />
<!-- /wp:separator -->

<!-- wp:atomic-blocks/ab-accordion {"accordionTitle":"DOI:, 10.25815/2F2X-NS46","accordionOpen":true} -->
<div class="wp-block-atomic-blocks-ab-accordion ab-block-accordion ab-font-size-18">
	<details open>
		<summary class="ab-accordion-title">
			<p>DOI: 10.25815/2F2X-NS46</p>
		</summary>
		<p class="ab-accordion-text">Citation format: <em>The Chicago Manual of Style, 17th Edition</em> <br/><br/>Dörner, Sophia. ‘Open Science #Barcamp: Software Citation’, 2018. https://doi.org/10.25815/2F2X-NS46.<br/></p>
	</details>
</div>
<!-- /wp:atomic-blocks/ab-accordion -->

<!-- wp:separator -->
<hr class="wp-block-separator" />
<!-- /wp:separator -->