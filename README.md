**Instructions for getting started with this model**

**Download the MS MARCO dataset**

wget https://msmarco.blob.core.windows.net/msmarco/train_v1.1.json.gz
wget https://msmarco.blob.core.windows.net/msmarco/dev_v1.1.json.gz
wget https://msmarco.blob.core.windows.net/msmarco/test_public_v1.1.json.gz

**Download GloVe vectors**
wget http://nlp.stanford.edu/data/glove.840B.300d.zip
unzip glove.840B.300d.zip

**Download NLTK punkt**
python3 -m nltk.downloader -d $HOME/nltk_data punkt

**Run convert_msmarco.py**
You may need to modify some paths

**Run tsv2ctf.py**
You may need to modify some paths

**Use the model to predict answer**
python train_pm.py -test $testdir -outputdir $outputdir -model pm.model7
$testdir means the data path
$outputdir means the model path

