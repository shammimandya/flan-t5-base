# flan-t5-base


Preprocess Stanford Contract NLI Dataset
----------------------------------------

Download contranct nli dataset (contract-nli.zp) from: https://stanfordnlp.github.io/contract-nli/ and unzip to folder ./stanford_contract_nli/contract-nli

To prepare Stanford Contract NLI dataset, run:

python preprocess_contract_nli_data.py --dataset_dir="./stanford_contract_nli/contract-nli/" --output_dir="./stanford_contract_nli/contract-nli-csv/"

Input arguments

dataset_dir: path to contract NLI dataset directory 
output_dir: path to output directory where ouptut csv files will be saved.

Genearted schema in the output file:

statement: policy statement
status: whether the statement is actionable or not
business_rue: business rule annotated for the statement
rule_code: unique id for business rule
source: Document ID of the policy document from which the policy statement is extracted
nli_label: natural language inference label for the instance.
