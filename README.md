# provenance-tracing
An algorithm for interpreting or tracing the provenance of score computed by random-walk based network diffusion algorithms.

## Conda Environment Setup
If you haven't cloned the repository yet, run the following command to clone it and navigate to the provenance-tracing folder:
```bash
git clone https://github.com/n-tasnina/provenance-tracing.git
cd provenance-tracing
```

Then, follow the steps below to set up the `provenance` environment with required libraries using the provided [`provenance_env.yml`](./provenance_env.yml) file.

```bash
conda env create -f provenance_env.yml
```
To run the command, make sure Conda is installed. If not, install [Anaconda](https://www.anaconda.com/docs/getting-started/anaconda/install) or the lighter version, [Miniconda](https://www.anaconda.com/docs/getting-started/miniconda/install).

After the environment is created, activate it using:
```bash
conda activate provenance
```

To verify that the environment and its dependencies are set up correctly, you can list the installed packages:
```bash
conda list
```


## Download Processed Dataset
Datasets used in this study has been uploaded to [Zenodo repository](https://doi.org/10.5281/zenodo.16423354).

## How to Run

The choice of algorithms and networks to run the experiments is configured using a YAML file (e.g., [signor_s12.yaml](./config-files/signor_s12.yaml)). 
To predict scores of proteins, and to compute node, path based effective diffusion, and diffusion betweenness score, run the following bash script.
```
   sh run.sh config-files/signor_s12.yaml
```


