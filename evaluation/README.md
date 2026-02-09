## Method 1 - using the competition's docker container

```
# Pull the docker container for the different dependencies
$ docker run --net=host --platform linux/amd64 -itd -u root amrkeleg/codabench-custom:py39 /bin/bash

# Check the `CONTAINER ID` and its `NAMES`
$ docker ps

# Copy the evaluation packs(preferrably the zip files to the running container), the reference data, and the prediction files to the container's root directory
$ docker cp FILE_LOCATION CONTAINER NAME:/

# Run the container in interactive mode
# Note: replace `CONTAINER_ID` with the id you got from the `docker ps` command
$ docker exec -it -u root CONTAINER_ID bash

# Unzip the evaluation script for the task of interest
$ unzip EVAL_SCRIPT.zip

# Add the Reference data to /app/input/ref
# Add the Predictions to /app/input/res
# Note: Check the filenames and directories hard-coded in the scripts

# Run the evaluation script
python3 scoring.py
```

## Method 2 - using a custom python environment (no guarantee of full reproducibility)

- Use `Python 3.9.12` to minimize any discrepancies
- Install the following dependencies (note: some data files will need to be downloaded when running the script)
```
pip install pandas
pip install numpy
pip install spacy
pip install konlpy
pip install hausastemmer
pip install nlp-id
pip install hazm
pip install qalsadi
pip install cltk
pip install spark-nlp==5.3.3 pyspark==3.3.1
pip install jieba
pip install mecab-python3
pip install unidic-lite
pip install simplemma
pip install lemmy
pip install pystemmer==3.0.0
pip install stanza
pip install amharicNLP==1.1.0
```

- Unzip the evaluation script for the task of interest
$ unzip EVAL_SCRIPT.zip

- Add the Reference data to /app/input/ref
- Add the Predictions to /app/input/res
    - Note: Check the filenames and directories hard-coded in the scripts

- Run the evaluation script `python3 scoring.py`