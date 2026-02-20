# rfDiff - GFP Protein Design with RFdiffusion

Colab notebooks for GFP protein design using RFdiffusion, created as lab exercise templates.

These notebooks demonstrate two complementary approaches to protein design using the RFdiffusion framework, applied to Green Fluorescent Protein (GFP, PDB: 1GFL) as a teaching example.

## Notebooks

- **GFP_Option1_MotifScaffolding.ipynb** - Motif scaffolding: fixes the GFP chromophore triad (S65-Y66-G67) and diffuses a new scaffold around it
- **GFP_Option2_PartialDiffusion.ipynb** - Partial diffusion: noises and rebuilds the full GFP beta-barrel, preserving topology

## Parameters Used

### Option 1 — Motif Scaffolding
| Parameter | Value |
|-----------|-------|
| contigs | 60/A60-75/60 |
| pdb | 1GFL |
| iterations | 100 |
| hotspot | A65,A66,A67 |
| num_designs | 4 |
| partial_T | auto |

### Option 2 — Partial Diffusion
| Parameter | Value |
|-----------|-------|
| contigs | A |
| pdb | 1GFL |
| iterations | 100 |
| num_designs | 4 |
| partial_T | 40 |

## Attribution

These notebooks are based on and derived from the **ColabDesign RFdiffusion notebook** by Sergey Ovchinnikov (sokrypton) and the RFdiffusion team:

- **Original Colab notebook:** [diffusion.ipynb](https://colab.research.google.com/github/sokrypton/ColabDesign/blob/main/rf/examples/diffusion.ipynb)
- **ColabDesign repository:** [sokrypton/ColabDesign](https://github.com/sokrypton/ColabDesign)

### RFdiffusion Citation

If you use these notebooks or RFdiffusion in your work, please cite:

> Watson, J.L., Juergens, D., Bennett, N.R., Trippe, B.L., Yim, J., Eisenach, H.E., Ahern, W., Borst, A.J., Ragotte, R.J., Milles, L.F., Wicky, B.I.M., Hanikel, N., Pellock, S.J., Courbet, A., Sheffler, W., Wang, J., Venkatesh, P., Sappington, I., Torres, S.V., Lauko, A., De Bortoli, V., Mathieu, E., Ovchinnikov, S., Barzilay, R., Jaakkola, T.S., DiMaio, F., Baek, M., Baker, D. (2023). De novo design of protein structure and function with RFdiffusion. Nature, 620, 1089-1100. https://doi.org/10.1038/s41586-023-06415-8

### ProteinMPNN Citation

> Dauparas, J., Anishchenko, I., Bennett, N., Bai, H., Ragotte, R.J., Milles, L.F., Wicky, B.I.M., Courbet, A., de Haas, R.J., Bethel, N., Leung, P.J.Y., Huddy, T.F., Pellock, S., Tischer, D., Chan, F., Koepnick, B., Nguyen, H., Kang, A., Sankaran, B., Bera, A.K., King, N.P., Baker, D. (2022). Robust deep learning-based protein sequence design using ProteinMPNN. Science, 378(6615), 49-56. https://doi.org/10.1126/science.add2187

## License

Please refer to the [ColabDesign](https://github.com/sokrypton/ColabDesign) and [RFdiffusion](https://github.com/RosettaCommons/RFdiffusion) repositories for their respective licenses.
