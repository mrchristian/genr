---
ID: 571
post_title: 'Software Preservation: A Stepping Stone for Software Citation'
author: Morane Gruenpeter
post_excerpt: ""
layout: post
permalink: >
  http://genr-updraft.consortium.io/software-preservation/
published: true
post_date: 2018-06-18 14:05:02
---
<!-- wp:image {"id":632,"align":"wide"} -->
<figure class="wp-block-image alignwide"><img src="http://genr.eu/wp/wp-content/uploads/2018/06/2018-04-archive-growth.png" alt="" class="wp-image-632" />
	<figcaption>The Software Heritage archive growth graph (view live on <br/><a href="https://www.softwareheritage.org/larchive-software-heritage/" target="_blank" rel="noopener">https://www.softwareheritage.org/larchive-software-heritage/</a>)</figcaption>
</figure>
<!-- /wp:image -->

<!-- wp:block {"ref":341} /-->

<!-- wp:block {"ref":172} /-->

<!-- wp:paragraph -->
<p>In recent years software has become a<strong> legitimate product of research</strong> gaining more attention from the scholarly ecosystem than ever before, and researchers feel increasingly the need to cite the software they use or produce. Unfortunately, there is no well established best practice for doing this, and in the citations one sees used quite often ephemeral URLs or other identifiers that offer little or no guarantee that the cited software can be found later on.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>But for software to be findable, it must have been preserved in the first place: hence software preservation is actually a prerequisite of software citation.</p>
<!-- /wp:paragraph -->

<!-- wp:more -->
<!--more-->
<!-- /wp:more -->

<!-- wp:heading -->
<h2>Preservation: why is it important?</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Software preservation is not a simple task. There are many use cases and the complexity of software may lead to different solutions for each of these use cases. One can find various approaches to describe a software system, for example in the paper 'A framework for software preservation' (<a href="https://doi.org/10.2218/ijdc.v5i1.145" target="_blank">Matthews et al. 2010</a>) an identification schema is proposed with four elements:</p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul>
	<li><em>Product,</em></li>
	<li><em><em>Version,</em></em>
	</li>
	<li><em><em><em>Variant, </em>and</em>
		</em>
	</li>
	<li><em><em>﻿<em>Instance), </em></em>
		</em>
	</li>
</ul>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p>but up to now the focus has been mainly on archiving software executables only. While an <strong>executable</strong> software artifact can be reused in certain circumstances — if the hardware and Operating System for which it was built still exists, a ‘big if’ when time goes by — it is often <strong>stripped of all the human knowledge</strong> a software source code may contain and is readable only by a machine. The executable is definitely important as a tool but it can’t be <strong>interpreted</strong>, <strong>studied</strong> or <strong>modified</strong>. That’s why the preservation of the source code is crucial if we want to keep the technical, functional, and cultural knowledge a software may contain, especially when dealing with <strong>research software</strong>.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>In the scholarly ecosystem, the quest for making scientific results reproducible, and to <strong>pass the knowledge</strong> over to future generations depends on the preservation of the three main pillars: scientific articles that describe the results, the data sets used or produced, and the software that embodies the logic of the data transformation (<a href="https://ipres2017.jp/wp-content/uploads/19Roberto-Di-Cosmo.pdf" target="_blank">Di Cosmo and Zacchiroli 2017</a>).</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":593} -->
<figure class="wp-block-image"><img src="http://genr.eu/wp/wp-content/uploads/2018/06/preservation_triangle_color.png" alt="" class="wp-image-593" />
	<figcaption><strong>Image: </strong>The pillars of knowledge preservation</figcaption>
</figure>
<!-- /wp:image -->

<!-- wp:heading -->
<h2>Software heritage: preserving the source code</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Software Heritage is an initiative aiming to <strong>collect</strong>, <strong>preserve</strong> and <strong>share</strong> all software source code, our<strong> software commons</strong>. The project was started in 2015 by <a href="https://www.inria.fr/" target="_blank">Inria</a> (The French Institute for Research in Computer Science and Automation) and has grown over time into a small and dedicated team led by <strong>Roberto Di Cosmo </strong>and <strong>Stefano Zacchiroli</strong>. As a non-profit organization Software Heritage will provide an infrastructure capable of responding to multiple stakeholders in a variety of situations.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Behind the scenes, the engineers created a mechanism that is <strong>actively crawling </strong>repositories (a task that we call <em>listing</em>) and collecting everything new it finds (a task that we call <em>loading</em>). The Software heritage archive is the <strong>largest software source code library </strong>to date and contains more than eighty-three million repositories, as of 6.6.2018.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>The current sources of the software are:</p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul>
	<li>live and updated regularly: GitHub, Debian</li>
	<li> one shot archival: Gitorious, Google Code and GNU</li>
	<li> in progress: Bitbucket</li>
</ul>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p>This is a significant head start, but there is still a long way to go to achieve the monumental task of archiving <strong>all software source code</strong> from development <strong>forges</strong>, <strong>package managers</strong>, <strong>repositories</strong>, <strong>FOSS distributions</strong> and even <strong>single URLs</strong> not hosted on major forges — which is the case with many researchers publishing their software on their personal page.</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2><strong>Software deposit: publish the source code and promote Open Science</strong></h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Researchers in many domains are using software for their work and some are creating software to support their research. For data, there are many organizations, initiatives and working groups promoting the <strong>FAIR data principles</strong>, yet software is a new actor in the field and making software discoverable and <strong>open source is still not the default</strong>. Furthermore, finding the correct metadata to cite software is even more difficult. The <strong>CodeMeta</strong> initiative (<a href="https://doi.org/10.5063/schema/codemeta-2.0" target="_blank">CodeMeta 2017</a>) and the <strong>CITATION file format </strong>(<a href="https://zenodo.org/record/1003150" target="_blank">Druskat 2017﻿</a>) are two projects providing a metadata schema to enable citation by including a metadata file inside the source code. Unfortunately, these metadata files are really scarce today.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>To promote <strong>Open Science</strong> and <strong>Open Source Software</strong> a new collaboration has emerged between Software Heritage, <a href="https://hal.inria.fr/" target="_blank">Hal-Inria</a> (the open archive of Inria) and the <a href="https://www.ccsd.cnrs.fr/" target="_blank">CCSD</a> (The Center for Direct Scientific Communication). It has resulted with a new type of scientific deposit in the French national open archive. Researchers have now the possibility to deposit software source code on <a href="https://hal.inria.fr/" target="_blank">Hal-Inria</a> (<a href="https://hal.inria.fr/hal-01738741" target="_blank">Barborini et al. 2018</a>). With this new possibility, research software is pushed with the submitted metadata to the Software Heritage archive and a <em>swh-id</em> (an intrinsic identifier) is returned by Software Heritage.The swh-id is an intrinsic identifier because it is calculated using the content of the digital artifact, which means that if calculated by another organization with the same cryptographic hash (<a href="https://en.wikipedia.org/wiki/SHA-1" target="_blank">SHA1</a>, <a href="https://en.wikipedia.org/wiki/BLAKE_(hash_function)" target="_blank">BLAKE256</a>, etc.) it will result with the same identifier. We use it in our archive's resolver with a specific semantic schema. The citation format on Hal-Inria, inspired by the <strong>software citation principles </strong>(<a href="https://doi.org/10.7717/peerj-cs.86" target="_blank">Arfon et al. 2016</a>)<strong>,</strong> includes the <em>swh-id</em> which is a<strong> direct access</strong> to the archived software source code.</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2><strong>The swh-id: a digital finger-print for a software artifact</strong></h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Source code is massively duplicated across projects and across forges, hence, as explained in more detail in (<a href="https://ipres2017.jp/wp-content/uploads/19Roberto-Di-Cosmo.pdf" target="_blank">Di Cosmo and Zacchiroli 2017</a>), the data model used for the Software Heritage archive is a Merkle Direct Acyclic Graph (DAG) (<a href="https://doi.org/10.1007/3-540-48184-2" target="_blank">Ralph C. Merkle. 1987</a>), commonly known as a hash tree. Using this structure, each object present in the Software Heritage archive is associated with an <strong>intrinsic identifier</strong> computed through<strong> cryptographic hashes</strong>.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":615,"align":"center"} -->
<figure class="wp-block-image aligncenter"><img src="http://genr.eu/wp/wp-content/uploads/2018/06/merklevertical.png" alt="" class="wp-image-615" />
	<figcaption>Image: Software Heritage data model: a uniform Merkle DAG containing source code artifacts and their development history</figcaption>
</figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>These identifiers are guaranteed to remain <strong>stable</strong> over time, and are resolved with a persistent identifier schema directly on <em>https://archive.softwareheritage.org/&lt;swh-id></em>, described in the <a href="https://docs.softwareheritage.org/devel/swh-model/persistent-identifiers.html" target="_blank">persistent identifiers documentation﻿</a>. To access the persistent identifiers a <strong>permalinks</strong> box is available on a side tab and provides identifiers for the current <em>directory, revision</em> (a commit on a particular branch) or <em>snapshot </em>(the complete set of branches in a version control system):</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":624,"align":"center"} -->
<figure class="wp-block-image aligncenter"><img src="http://genr.eu/wp/wp-content/uploads/2018/06/Permalinks.png" alt="" class="wp-image-624" />
	<figcaption>Image: Access Gensim source code in the archive <a href="https://archive.softwareheritage.org/swh:1:dir:774f7d3f4a99f9754e785e1335fe718a4234eba7;origin=https://github.com/RaRe-Technologies/gensim/" target="_blank">https://archive.softwareheritage.org/swh:1:dir:774f7d3f4a99f9754e785e1335fe718a4234eba7;origin=https://github.com/RaRe-Technologies/gensim/</a></figcaption>
</figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>And the great advantage of the swh-ids is that they are now already available for all the billions of software artifacts stored in the Software Heritage archive: yes, that means that you can reference all kind of software, not just the few projects that have proper metadata attached!</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>The metadata challenge</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Many challenges are still ahead. As noted in (<a href="https://danielskatzblog.wordpress.com/2017/09/25/software-heritage-and-repository-metadata-a-software-citation-solution/" target="_blank">Katz 2017</a>) giving credit to the developers and finding the appropriate metadata for citation can’t be solved by Software Heritage alone. However, Software Heritage fulfills the need of software preservation, that is a stepping stone to proper software citation, and we are planning on <strong>extracting the metadata</strong> included in the source code in AUTHORS, CONTRIBUTORS, README, LICENCE, codemeta.json, CITATION.cff and other metadata files. That’s why we urge all researchers and developers to <strong>include metadata files in their source code</strong> and keeping these files updated.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>You are welcome to visit our <strong>online browsable </strong><strong>archive</strong> on <strong><a href="https://archive.softwareheritage.org/" target="_blank">https://archive.softwareheritage.org/</a></strong> where you can search through the more than eighty million origins urls, browse the contents, obtain a swh-id and download a directory or a revision. <em>Enjoy!</em></p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>References</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Matthews, A. Shaon, J. Bicarregui, and C. Jones, “A framework for software preservation” , International Journal of Digital Curation, vol. 5, no. 1, pp. 91-105, 2010. <a href="https://doi.org/10.2218/ijdc.v5i1.145" target="_blank" rel="noopener">doi:10.2218/ijdc.v5i1.145</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Roberto Di Cosmo and Stefano Zacchiroli. 2017. Software Heritage: Why and How to Preserve Software Source Code. In Proceedings of the 14th International Conference on Digital Preservation, iPRES 2017.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Matthew B. Jones, Carl Boettiger, Abby Cabunoc Mayes, Arfon Smith, Peter Slaughter, Kyle Niemeyer, Yolanda Gil, Martin Fenner, Krzysztof Nowak, Mark Hahnel, Luke Coy, Alice Allen, Mercè Crosas, Ashley Sands, Neil Chue Hong, Patricia Cruse, Daniel S. Katz, Carole Goble. 2017. CodeMeta: an exchange schema for software metadata. Version 2.0. KNB Data Repository. <a href="https://doi.org/10.5063/schema/codemeta-2.0">doi:10.5063/schema/codemeta-2.0</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Druskat, Stephan. 2017. Citation File Format (CFF). Zenodo. <a href="https://zenodo.org/record/1003150" target="_blank" rel="noopener">doi:10.5281/zenodo.1003150﻿</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Yannick Barborini, Roberto Di Cosmo, Antoine R. Dumont, Morane Gruenpeter, Bruno Marmol, et al. The creation of a new type of scientific deposit: Software. <em>RDA Eleventh Plenary Meeting, Berlin, Germany</em>, Mar 2018. <a href="https://www.rd-alliance.org/rda-11th-plenary-poster-session">https://www.rd-alliance.org/rda-11th-plenary-poster-session</a>. <a href="https://hal.inria.fr/hal-01738741">(hal-01738741)﻿</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Smith, Arfon M., Katz, Daniel S., Niemeyer, Kyle E., &amp; FORCE11 Software Citation Working Group. 2016. Software citation principles. <em>PeerJ Computer Science</em>, <em>2</em>, e86. <a href="https://doi.org/10.7717/peerj-cs.86">https://doi.org/10.7717/peerj-cs.86﻿</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Ralph C. Merkle. 1987. A Digital Signature Based on a Conventional Encryption Function. In Advances in Cryptology – CRYPTO ’87, A Conference on the Theory and Applications of Cryptographic Techniques, Santa Barbara, California, USA, August 16-20, 1987, Proceedings (Lecture Notes in Computer Science), Carl Pomerance (Ed.), Vol. 293. Springer, 369–378. <a href="https://doi.org/10.1007/3-540-48184-2" target="_blank">https://doi.org/10.1007/3-540-48184-2 32</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Persistent identifiers documentation, Software Heritage –  <a href="https://docs.softwareheritage.org/devel/swh-model/persistent-identifiers.html" target="_blank" rel="noopener">https://docs.softwareheritage.org/devel/swh-model/persistent-identifiers.html﻿</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Daniel S. Katz. 2017. Software Heritage and repository metadata: a software citation solution. Daniel S. Katz’s blog. <a href="https://danielskatzblog.wordpress.com/2017/09/25/software-heritage-and-repository-metadata-a-software-citation-solution/" target="_blank">https://danielskatzblog.wordpress.com/2017/09/25/software-heritage-and-repository-metadata-a-software-citation-solution/</a></p>
<!-- /wp:paragraph -->

<!-- wp:separator -->
<hr class="wp-block-separator" />
<!-- /wp:separator -->

<!-- wp:html -->
<div class="wp-block-atomic-blocks-ab-accordion ab-block-accordion ab-font-size-18">
	<details open="">
		<summary class="ab-accordion-title">
			<p>DOI: 10.25815/0ZBH-2W14</p>
		</summary>
		<p class="ab-accordion-text">Citation format:&nbsp;<em>The Chicago Manual of Style, 17th Edition</em> <br><br>Gruenpeter, Morane. ‘Software Preservation: A Stepping Stone for Software Citation’, 2018. https://doi.org/10.25815/0ZBH-2W14.<br></p>
	</details>
</div>
<!-- /wp:html -->

<!-- wp:separator -->
<hr class="wp-block-separator" />
<!-- /wp:separator -->