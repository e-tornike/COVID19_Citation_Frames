# A Meta-Analysis of Scientific Literature on COVID-19 through Citation Frames

### Getting started 

Download the CORD-19 dataset from [here](https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge?). The data should be in `./cord19`.

Install dependencies:

```bash
python -m venv venv
source venv/bin/activate
pip install --upgrade pip setuptools
pip install -r requirements.txt
```

Start neo4j server (only needed if running analysis and plotting neo4j graph):

```bash
bash neo4j-community-4.1.2/bin/neo4j start
```

Run jupyter and open notebook:

```bash
jupyter notebook
```

To reproduce the results, follow the steps below:

1. Fine-tune SciBERT on SciCite (citation_intent_classification.ipynb)
2. Process the CORD-19 data (process_data.ipynb)
3. Run the anaylsis (analysis.ipynb)
