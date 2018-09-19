---
ID: 30
post_title: 'Software Citation for Humans: The Citation File Format'
author: Stephan Druskat
post_excerpt: ""
layout: post
permalink: >
  http://genr-updraft.consortium.io/software-citation-for-humans/
published: true
post_date: 2018-06-11 10:04:25
---
<!-- wp:image {"id":386,"align":"center"} -->
<figure class="wp-block-image aligncenter"><img src="http://genr.eu/wp/wp-content/uploads/2018/06/First_Web_Server.jpg" alt="" class="wp-image-386" />
	<figcaption>Image: This NeXT workstation was used by Tim Berners-Lee as the first Web server on the World Wide Web in 1991. It is shown here as displayed in 2005 at Microcosm, the public science museum at CERN. Creative Commons Attribution-Share Alike 3.0 Unported. <a href="https://commons.wikimedia.org/wiki/File:First_Web_Server.jpg" target="_blank">Wikimedia Commons</a>.</figcaption>
</figure>
<!-- /wp:image -->

<!-- wp:block {"ref":341} /-->

<!-- wp:block {"ref":172} /-->

<!-- wp:paragraph -->
<p>Software is an important research product. It embeds knowledge. Thus, it should be cited like all other scientific products. But how do you cite the software that you use in your research?</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Until a more suitable system for software citation exists, we need to leverage the one in place for papers and books. But finding the metadata needed for citation is usually harder for software than for papers. Therefore authors must provide it visibly and accessibly.</p>
<!-- /wp:paragraph -->

<!-- wp:more -->
<!--more-->
<!-- /wp:more -->

<!-- wp:heading -->
<h2>Providing software citation metadata</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Robin Wilson has suggested one way of doing this in a <a href="https://www.software.ac.uk/blog/2013-09-02-encouraging-citation-software-introducing-citation-files" target="_blank">blog post</a>: Include a file containing the relevant information in the code repository. Name the file CITATION — in analogy to LICENSE and README — so that users can find it easily, and cite the software correctly.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>The next step is to make the CITATION file machine-readable and open it up for further use cases, by using a standard format. This way, its contents can be used easily</p>
<!-- /wp:paragraph -->

<!-- wp:list {"className":"list-content"} -->
<ul class="list-content">
	<li>
		in the software itself, e.g., in <em>About</em> dialogs, cite() commands, data output;
	</li>
	<li>
		in repositories, publishing platforms, software directories, e.g., to display a formatted reference;
	</li>
	<li>
		by indexers, publishers, reference managers, etc., for further processing.
	</li>
</ul>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p>But as one of the most important use cases for CITATION files is still discovery by users, it is necessary to preserve human-readability.
</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>Using the correct software citation metadata</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>In order to unlock the full potential of software citation, including the enablement of research reproducibility, the citation metadata must adhere to a number of principles: the software citation principles (Smith et al. 2016). According to these, the available metadata for a software must at least include:</p>
<!-- /wp:paragraph -->

<!-- wp:list {"className":"list-content"} -->
<ul class="list-content">
	<li>
		A unique identifier
	</li>
	<li>
		The software name
	</li>
	<li>
		The author(s)
	</li>
	<li>
		The version number
	</li>
	<li>
		The release date
	</li>
	<li>
		The location or repository of the software
	</li>
</ul>
<!-- /wp:list -->

<!-- wp:heading -->
<h2>The Citation File Format</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Emanating from a lightning talk (Druskat 2017), the prerequisites of a useful format for CITATION files have been discussed at the <a href="http://wssspe.researchcomputing.org.uk/wssspe5-1/" target="_blank">WSSSPE5.1 workshop</a>, and the results are published in a <a href="https://www.software.ac.uk/blog/2017-12-12-standard-format-citation-files" target="_blank">blog post</a>. It suggests that such a format must fulfill at least two criteria:</p>
<!-- /wp:paragraph -->

<!-- wp:list {"className":"list-content"} -->
<ol class="list-content">
	<li>
		human- and machine-readability;
	</li>
	<li>
		adherence to the software citation principles.
	</li>
</ol>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p>The <a href="https://citation-file-format.github.io/" target="_blank">Citation File Format</a> (CFF) fulfills these criteria. It is implemented as a key-value map in <a href="http://yaml.org/" target="_blank">YAML</a>, a “human friendly data serialization standard for all programming languages”. It supports the software citation principles by requiring central keys (see above), and allowing for the fallback solutions also defined in Smith et al. (2016). Additionally, it is self-explanatory by providing a free text message field which states the purpose of the metadata and directions for its use.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>A simple valid CITATION.cff file looks something like this:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>cff-version: 1.0.3
message: "If you use this software, cite it with below metadata."
authors:
  - family-names: Druskat
    given-names: Stephan
title: My Research Tool
version: 1.0.4
doi: 10.5281/zenodo.1234
date-released: 2017-12-18
repository-code: https://github.com/sdruskat/my-research-tool</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>
	The Citation File Format also provides keys for other metadata, such as license, different repository types, keywords, contact information, etc. Additionally, it allows the specification of secondary references which users should also cite under specific circumstances. These references can be scoped to define when they should be cited.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>message: If you use My Research Tool (MRT), please cite the software AND the outline paper.
    ...
references:
  - type: article
    scope: Cite this paper to reference the general concepts of the tool.
    authors:
      - family-names: Maus
        given-names: Ketty
    title: "My Research Tool: A 100% accuracy syntax parser for all languages"
    year: 2099
    journal: Journal of Hard Science Fiction
    volume: 42
    issue: "13"
    doi: 10.9999/hardscifi-lang.42132</code></pre>
<!-- /wp:code -->

<!-- wp:heading -->
<h2>
	The Citation File Format as the first step in the software citation workflow
</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Given its human-friendly, yet machine-actionable, properties, the Citation File Format represents a suitable entry point to the software citation workflow, and depositing a CITATION.cff file in a repository should be the first step.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Further downstream in the software citation workflow, the metadata will have to be exchanged between different actors without human intervention, e.g., when it is harvested from long-term storage or publication platforms by indexing services. At this point, automated linking and resolving capabilities become more important than human-readability or fine-grained recording of secondary references. For these purposes, the metadata should be converted into a linked data exchange format: <a href="https://codemeta.github.io/" target="_blank">CodeMeta</a> JSON-LD.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>The Citation File Format is compatible with CodeMeta, and in order to facilitate smooth transfer between the two formats, the Citation File Format community develop a number of software tools, among them a <a href="https://github.com/citation-file-format/cff-converter-python" target="_blank">converter</a> which can transform CITATION.cff files to CodeMeta JSON-LD. These tools can be used — for example in the build and release processes — to make sure that the software citation metadata is preserved and re-usable across the complete workflow.</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>Development and outlook</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>The Citation File Format is supported by different projects. It is, for example, one of the source formats for <a href="http://citeas.org/" target="_blank">CiteAs.org</a>, a citation resolver for different metadata formats, and the <a href="https://www.esciencecenter.nl/" target="_blank">Netherlands eScience Center</a> has adopted it for its software projects. Its integration into the wider software citation workflow is also worked on in the scope of the <a href="https://www.force11.org/group/software-citation-implementation-working-group" target="_blank">FORCE11 Software Citation Implementation WG</a>.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>The current version of the Citation File Format — the “Core Module” — is centred around providing the necessities for software citation. Development of further modules is planned for the future in order to support a wider range of software metadata for, e.g., data requirements and transitive credit.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>To support developers, users, and integration efforts, and to foster uptake, <a href="https://github.com/citation-file-format/citation-file-format" target="_blank">software tools for CFF</a> have been, and continue to be, developed by the community. They include <a href="https://github.com/citation-file-format/schema" target="_blank">validation schemas</a>, <a href="https://github.com/citation-file-format/cff-reader-java" target="_blank">a reader library</a>, <a href="https://github.com/citation-file-format/cff-converter-python" target="_blank">a multi-format converter</a>, <a href="https://github.com/citation-file-format/doi2cff" target="_blank">a DOI</a> and a <a href="https://github.com/citation-file-format/github2cff" target="_blank">GitHub/GitLab resolver</a>, and <a href="https://github.com/citation-file-format/ruby-cff" target="_blank">Ruby tooling</a>. A web application is currently in development, based on work started during the <a href="https://software.ac.uk/cw18" target="_blank">SSI Collaborations Workshop 2018</a> Hack Day. And on 5 September, the first ever <a href="https://citation-file-format.github.io/events/rse18-hack-day/" target="_blank">Citation File Format Hack Day</a> will take place in Birmingham, co-locating with the <a href="http://rse.ac.uk/conf2018/" target="_blank">3rd Conference of Research Software Engineers</a>.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>The <a href="https://github.com/citation-file-format/citation-file-format.github.io" target="_blank" rel="noopener">Citation File Format itself</a>, as well as all tooling, is <a href="https://github.com/citation-file-format" target="_blank">maintained openly on GitHub</a> and welcomes contributions!</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>References</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Druskat, Stephan. 2017. ‘Track 2 Lightning Talk: Should CITATION Files Be Standardized?’ In <em>Proceedings of the Workshop on Sustainable Software for Science: Practice and Experiences (WSSSPE5.1)</em>, edited by Neil Chue Hong, Stephan Druskat, Robert Haines, Caroline Jay, Daniel S. Katz, and Shoaib Sufi. figshare. <a href="https://doi.org/10.6084/m9.figshare.3827058" target="_blank" rel="noopener">https://doi.org/10.6084/m9.figshare.3827058﻿</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Smith, Arfon M., Daniel S. Katz, Kyle E. Niemeyer, and FORCE11 Software Citation Working Group. 2016. ‘Software Citation Principles’. <em>PeerJ Computer Science 2 (e86)</em>. <a href="https://doi.org/10.7717/peerj-cs.86" target="_blank" rel="noopener">https://doi.org/10.7717/peerj-cs.86﻿</a></p>
<!-- /wp:paragraph -->

<!-- wp:spacer {"height":24} -->
<div style="height:24px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:spacer -->

<!-- wp:atomic-blocks/ab-notice {"noticeTitle":"Disclosure","noticeBackgroundColor":"#676767"} -->
<div style="color:#32373c;background-color:#676767" class="wp-block-atomic-blocks-ab-notice ab-font-size-18 ab-block-notice" data-id="cffcb1">
	<div class="ab-notice-title" style="color:#fff">
		<p>Disclosure</p>
	</div>
	<div class="ab-notice-text" style="border-color:#676767">
		<p>Stephan Druskat is a founder and the project lead of the <strong>Citation File Format</strong> project</p>
	</div>
</div>
<!-- /wp:atomic-blocks/ab-notice -->

<!-- wp:separator -->
<hr class="wp-block-separator" />
<!-- /wp:separator -->

<!-- wp:atomic-blocks/ab-accordion {"accordionTitle":"DOI:, 10.25815/p3dh-hz85","accordionOpen":true} -->
<div class="wp-block-atomic-blocks-ab-accordion ab-block-accordion ab-font-size-18">
	<details open>
		<summary class="ab-accordion-title">
			<p>DOI: 10.25815/p3dh-hz85</p>
		</summary>
		<p class="ab-accordion-text">Citation format: <em>The Chicago Manual of Style, 17th Edition</em> <br/><br/>Druskat, Stephan. ‘Software Citation for Humans: The Citation File Format’. Leibniz Research Alliance Science 2.0, 2018. https://doi.org/10.25815/P3DH-HZ85.<br/></p>
	</details>
</div>
<!-- /wp:atomic-blocks/ab-accordion -->

<!-- wp:separator -->
<hr class="wp-block-separator" />
<!-- /wp:separator -->