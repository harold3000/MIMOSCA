<img src="https://github.com/asncd/MIMOSCA/blob/master/common_files/mimosca_logo.png" title="MIMOSCA" alt="MIMOSCA" height=99 width=372>

## Related Resources

* <a href="https://groups.google.com/forum/#!forum/perturb-seq">Perturb-seq Google Forum</a>
* <a href="http://biorxiv.org/content/early/2016/12/12/093237">Chimera Correction</a>  and <a href="https://github.com/asncd/schimera">Code</a>
* <a href="http://www.clontech.com/US/Products/Genome_Editing/CRISPR_Cas9/Resources/Online_tools_for_guide_RNA_design">sgRNA Design Tools</a>

## Contents

* [Design of Experiments](https://github.com/asncd/MIMOSCA/blob/master/README.md#design-of-experiments--power-calculations)
* GBC/CBC pairing
* Cell state definition
* Beta Features

Still under construction and will be updated in the coming weeks.

<img src="http://www.clipartbest.com/cliparts/ncE/KRE/ncEKRE7Ai.gif" title="Under Construction" alt="Under Construction">

## Design of Experiments & Power Calculations

<img src="https://github.com/asncd/MIMOSCA/blob/master/common_files/comp_knob.png" title="Experimental Design" alt="Experimental Design" height=360 width=432>

In designing Perturb-seq like experiments, there are a few key factors to keep in mind:

### Signatures vs. individual transcript-level phenotypes
Are you interested in broad transcriptional signatures or individual gene level differential expression? If the former, a rough approximation may be around 10 cells/perturbation. If the later, 100 or more cells may be required based on the effect size. 

### Library Size and Representation

As in any pooled screen, the representation of each perturbation in the library will vary. With genome wide CRISPR libraries the difference between the 10th and 90th percentile of a library is roughly 6-fold (Wang, 2013). Depending on how much a user wants to ensure every member of the library is represented, the cells/perturbation factor should be multiplied by an additional factor to reflect this variance.

## Computational Workflow

<img src="https://github.com/asncd/MIMOSCA/blob/master/common_files/comp_flow2.png" title="Overview" alt="Overview" height=662 width=569>
