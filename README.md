# Cross-lingual Clinical NER with XLM-R

This project investigates multilingual clinical named entity recognition
and cross-lingual transfer between the English i2b2 corpus and the
Spanish MEDDOCAN corpus using XLM-RoBERTa.

## Experiments

1. Train and evaluate an English model on i2b2.
2. Evaluate the English model on Spanish MEDDOCAN data.
3. Train and evaluate a Spanish model on MEDDOCAN.
4. Evaluate the Spanish model on English i2b2 data.

## Data preprocessing

The original datasets were converted into CoNLL files with BIO labels
before training.

The MEDDOCAN BRAT annotations were converted to BIO format using a
separate preprocessing script.

The datasets are not included in this repository because of access,
privacy, and licensing restrictions.

## Cross-lingual label mapping

Only entity labels with a reliable semantic correspondence between
i2b2 and MEDDOCAN were compared. Unmapped labels were assigned `-100`
and ignored during evaluation.

## Files

- `Final Project llm medicine.ipynb`: final notebook
- `requirements.txt`: required Python packages
