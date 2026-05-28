### [ICML'26] Certified Circuits: Stability Guarantees for Mechanistic Circuits

<p align="center">
<a href="https://alaaanani.github.io/"><strong>Alaa Anani</strong></a><sup>1,2</sup>,
<a href="https://www.t-lorenz.com/">Tobias Lorenz</a><sup>2</sup>,
<a href="https://www.mpi-inf.mpg.de/departments/computer-vision-and-machine-learning/people/bernt-schiele">Bernt Schiele</a><sup>1</sup>,
<a href="https://cispa.de/en/people/mario.fritz">Mario Fritz</a><sup>2,*</sup>,
<a href="https://www.mpi-inf.mpg.de/departments/computer-vision-and-machine-learning/people/jonas-fischer">Jonas Fischer</a><sup>1,*</sup>
</p>

<p align="center">
<sup>1</sup> Max Planck Institute for Informatics,
<sup>2</sup> CISPA Helmholtz Center for Information Security<br>
<sup>*</sup> Equal advising
</p>

[![Website](https://img.shields.io/badge/Website-Certified%20Circuits-blue)](https://alaaanani.github.io/#/project/certified-circuits) [![arXiv](https://img.shields.io/badge/arXiv-2602.22968-b31b1b.svg)](https://arxiv.org/abs/2602.22968)

**Code will be released soon.**

<table>
  <tr>
    <td><img src="assets/teaser_circuit%20%281%29-1.png" alt="Certified Circuits teaser" height="280"></td>
    <td><img src="assets/teaser_better.png" alt="Certified Circuits accuracy and circuit size teaser" height="280"></td>
  </tr>
</table>

**Abstract:**
Understanding <em>how</em> neural networks arrive at their predictions is essential for debugging, auditing, and deployment. Mechanistic interpretability pursues this goal by identifying <em>circuits</em> - minimal subnetworks responsible for specific behaviors. However, existing circuit discovery methods are brittle: circuits depend strongly on the chosen concept dataset and often fail to transfer out-of-distribution, raising doubts whether they capture the concept or merely dataset-specific artifacts. We introduce <em>Certified Circuits</em>, which provide provable stability guarantees for circuit discovery. Our framework wraps any black-box discovery algorithm with randomized data subsampling to certify that inclusion decisions over circuit components - neurons or edges of the model graph, depending on the base algorithm - are invariant to bounded edit-distance perturbations of the concept dataset. Unstable components are abstained from, yielding circuits that are more compact and more accurate. We validate across three architectures (ResNet, ViT, GPT-2) on vision (ImageNet and four OOD datasets) and language (IOI, IOI-Hard, Greater-Than) tasks. Certified circuits achieve up to 56% higher accuracy and up to 80% fewer components, and remain reliable where baselines degrade. <em>Certified Circuits</em> puts circuit discovery on formal ground by producing mechanistic explanations that are provably stable and better aligned with the target concept.

---

### Citation

If you find our work useful, please cite it as:

```bibtex
@inproceedings{anani2026certified,
    title={Certified Circuits: Stability Guarantees for Mechanistic Circuits},
    author={Anani, Alaa and Lorenz, Tobias and Schiele, Bernt and Fritz, Mario and Fischer, Jonas},
    booktitle={Proceedings of the 43rd International Conference on Machine Learning (ICML)},
    year={2026}
}
```
