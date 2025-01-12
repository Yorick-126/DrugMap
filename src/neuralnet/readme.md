Here, we used machine learning to probe a fundamental question in drug discovery... **can structural information be leveraged to infer cysteine ligandability**? 

<p align="center">
  <img src="https://github.com/bplab-compbio/DrugMap/blob/main/src/images/structural.mapping.png" >
</p>

We first aligned as many cysteines to the [Protein Data Bank](https://www.rcsb.org/) as possible. We partitioned protein structures into their corresponding rotamers when available. For each cysteine, we chose representative structures while optimizing for both 1.) completeness of structural coverage and 2.) resolution.

<p align="center">
  <img src="https://github.com/bplab-compbio/DrugMap/blob/main/src/images/neural.net.png" >
</p>

We then fed a [deep neural network](https://github.com/bplab-compbio/DrugMap/blob/main/src/neuralnet/notebook.ipynb) both geometric and vectorized data, all encapsulating unique dimensions of a cysteine's structural locale, to allow the network to learn whether a cysteine is ligandable or not. We hope that the structural data and methodology deposited herein will further the community's quest to predict cysteine ligandability!
