<!-- .slide: class="titleslide" -->

# Publishing Software and Workflows in QMC-HAMM

## Matthew Turk

<p data-markdown=true><tt>mjturk@illinois.edu</tt></p>

---

# Why publish?

To answer motivations we have to define our standpoint first.

<div class="multiCol">
    <div class="col fragment">

From a scientific perspective, the reasons are "obvious":

* Share *information*
* Promote transparency
* Facilitate reproducibility

    </div>
    <div class="col fragment">

From the perspective of existing in academia, the reasons are equally "obvious":

* Demonstrate *your* impact on the community and your *funder's* impact on *you*
* Assert intellectual priority
* Foster collaboration

</div>
</div>

---

# Definition of Terms

(These are loose, non-formal definitions, just to get us on the same page.)

 * **Publication**: deposition of a fixed record, often used interchangeably with making that record public.
 * **DOI**: Digital Object-Identifer, or a mechanism for identifying and locating something that has existed and may continue to exist, with a metadata record describing it.  These are centrally managed (see [DOI.org](https://doi.org)) but there are issuing authorities such as [CrossRef](https://crossref.org/), [DataCite](https://datacite.org/), and these issuing authorities themselves can delegate issuance.
 * **Metadata**: Affiliated records that capture the acquisition or provenance of the data.  This might include the version of an executable you used to generate data, or which computer you executed it on, or when it happened.
 * **Repository**: A destination that accepts depositions and metadata, and assigns to them a publication and (often) a DOI.
 * **Citation**: A reference in a publication

---

# What We Want: Impact

 * We generate a workflow, a piece of software, or a publication
 * Others either use it, agree with it, disagree with it, or build upon it to conduct research
 * Their publication *references* our publication in a mechanism that is both human-trackable and machine-trackable
 * The "web" of interconnected utilizations can be understood and analyzed
 * Funders, institutions and other individuals can be appropriately credited for advancements that have impact

---

# Publish what?

 * Papers
    * Results and analysis
    * Process and methodology
 * Datasets
    * Unprocessed
    * Processed
 * Generative workflows
    * Turn-key replication methods
    * "Living provenance"
 * Software
    * Software packages with novelty
    * *Anything* reusable

<p class="fragment">I will avoid discussing the first one.</p>

---

# Cost-Benefit Analysis

When working toward publishing a piece of software or a workflow, we need to evaluate the cost and the benefit of preparing something for publication.

<ul>
<li class="fragment">"Cleaning" the software for presentation</li>
<li class="fragment">Documenting the software</li>
<li class="fragment">Rigorously testing the software</li>
</ul>

---

# On Reusability and Workflows

 > "Every so often, in group meeting, I take one of my group member's laptops,
 > smash it, and hand the group member a newer, much better laptop. If they are
 > happy (yay, new, better laptop), they are properly synched! If they are
 > unhappy, they aren't."  
 > &#x2015; David W. Hogg

The more person-in-the-middle steps there are, the more likely it is that there will be **mistakes**, loss of institutional **knowledge**, and difficulties in **replication**.

<div class="fragment">The cost-benefit relationship here is less obvious, as the "benefit" can be derived from merely providing supplemental information about the calculation.  We should err on the side of transparency.</div>

---

# Publish how?

We can develop a procedure for publication of software and workflows.

<ol>
<li class="fragment">Identify publishable parts</li>
<li class="fragment">Collect necessary materials</li>
<li class="fragment">Archive and submit archive to repository</li>
</ol>

<span class="fragment">All of this is made much, much easier if we presuppose our software is in a <b>continuous state of informal release.</b></span>

---

# Publish where?

* Option Zero: Traditional Journals
* Option One: Inert storage
* Option Two: Active storage

---

# Where: "Traditional" Publications

Utilizing traditional publications to describe methods, novel algorithms and overarching projects is a good way of getting exposure to colleagues and peers.

However, the traditional publication pipeline often does not include software-specific publication channels.

---

# Where: Semi-Traditional Publications

Additional journals provide opportunities for publishing software.  Two in particular:

<div class="multiCol">
<div class="col">

![](https://openresearchsoftware.metajnl.com/static/images/header.png) <!-- element: style="width: 100%" -->

</div>
<div class="col">

[JORS](https://openresearchsoftware.metajnl.com/) features peer reviewed Software Metapapers describing research software with high reuse potential. 

Typically, these will be *longer* papers that focus on the methodology of the publication, and where the *paper* is the subject of review rather than the software itself.

</div>
</div>

---

# Where: Semi-Traditional Publications

Additional journals provide opportunities for publishing software.  Two in particular:


<div class="multiCol">
<div class="col">

![](https://joss.theoj.org/logo_large.jpg) <!-- element: style="width: 100%" -->

</div>
<div class="col">

[JOSS](https://joss.theoj.org/) is a fully-open, peer-reviewed system for reviewing software that utilizes GitHub as its backend.  It is designed to be developer-friendly, for both publication *and* review.

Typically, JOSS is for short papers that describe the basic workings of a software package; these papers are included in the repository.

</div>
</div>

---

# Where: Inert Storage

Systems that provide storage, but without the ability to directly execute computations.  In many cases, these treat data and software essentially identically; for workflows, this poses a unique problem as they walk the line between the two.

There are three in particular I would highlight:

<div class="multiCol">
<div class="col">

![](https://about.zenodo.org/static/img/logos/zenodo-gradient-2500.png) <!-- element: style="width: 100%" -->

</div>
<div class="col">

[Zenodo](https://zenodo.org/) is a data repository that provides large-scale storage solutions and issues identifiers.

</div>
</div>


---

# Where: Inert Storage

Systems that provide storage, but without the ability to directly execute computations.  In many cases, these treat data and software essentially identically; for workflows, this poses a unique problem as they walk the line between the two.

There are three in particular I would highlight:

<div class="multiCol">
<div class="col">

![](https://www.digital-science.com/wp-content/uploads/2015/02/logo-figshare.png) <!-- element: style="width: 100%" -->

</div>
<div class="col">

[FigShare](https://figshare.com) is a data repository that is increasingly partnering with institutions to provide mechanisms for sharing categorized units of research such as individual files, figures, small datasets, posters, and the like.

</div>
</div>

---

# Where: Inert Storage

Systems that provide storage, but without the ability to directly execute computations.  In many cases, these treat data and software essentially identically; for workflows, this poses a unique problem as they walk the line between the two.

There are three in particular I would highlight:

<div class="multiCol">
<div class="col">

![](https://www.ideals.illinois.edu/themes/ideals-alt/images/IDEALS_logo_2x.png) <!-- element: style="width: 100%" -->

</div>
<div class="col">

[IDEALS](https://ideals.illinois.edu/) is an institutional repository at Illinois that is used for deposition of publications and datasets.

Note also that the Illinois Data Bank is focused on data specifically and may be a much better fit.

</div>
</div>


---

# Where: Active Storage

Systems that provide computation next to a dataset.

<div class="multiCol">
<div class="col">

![](https://wholetale.org/img/whole_tale_logo.svg)

</div>
<div class="col">

[Whole Tale](https://wholetale.org/) is a curation-focused system for sharing completed work products.

These are designed to be narrative, with the ability to explore results.  At present it does not itself issue persistent identifiers.

</div>
</div>

---

# Where: Active Storage

Systems that provide computation next to a dataset.

<div class="multiCol">
<div class="col">

![](https://dataverse.org/files/dataverseorg/files/dataverse_r_project.png)

</div>
<div class="col">

[Dataverse](https://dataverse.org/) is not itself active, but provides mechanisms for adding presentation layers or outsourcing the active analysis to other platforms (such as Whole Tale).

</div>
</div>

---

# Where: Active Storage

Systems that provide computation next to a dataset.

<div class="multiCol">
<div class="col">

![](https://girder.hub.yt/api/v1/file/5b6b3de1323d120001ab702f/download?contentDisposition=inline)

</div>
<div class="col">

[yt Hub](https://hub.yt/) is an active data repository that utilizes the same underlying architecture as Whole Tale.

We have the greatest flexibility with utilizing this repository.

</div>
</div>

---

# Where: Hybrid

This is what I think we should do.

<div class="multiCol">
    <div class="col">

## Data

Data should be published to Illinois Data Bank or Zenodo for 'safe-keeping' and identifier issuance, with copies in "active" repositories such as [hub.yt](https://hub.yt/).

For final releases of datasets, we can work with curators at the Illinois Library to develop necessary and appropriate metadata.

</div>
<div class="col">

## Software

Software should be versioned in open GitHub repositories, with the goal of publication of individual packages in JOSS.

Larger-scale projects (amalgams of multiple software projects) that are software-focused should be published in either domain-specific journals or JORS.

This should be used *generously* to publish our software -- from the very small to the very large.

</div>
<div class="col">

## Workflows

Workflows should be packaged *like* software and published directly to Zenodo.  Each time a production run is undertaken, we "tag" a release and push a new version to Zenodo.

Additionally, in our papers, we should cite the hash and DOI used for each dataset, and represent that in the metadata.

</div>
</div>

---

<!-- .slide: class="titleslide" -->

# Thank you!
