# vivi_spacy
Vivi_spacy is the first attempt to add support for Vietnamese in spacy(io). Word vectors trained with wikipedia corpus, size = 128 
## Installation 
Download vivi model directly using pip: e.g. pip install https://github.com/trungtv/vivi_spacy/raw/master/en_vivi-0.0.1/dist/en_vivi-0.0.1.tar.gz
## Usage: import as module 
```python
import spacy
import en_vivi
from pyvi.pyvi import ViTokenizer # Vietnamese tokenizer in python 
nlp = en_vivi.load()
doc = nlp(ViTokenizer.tokenize(u'Bách Khoa Hà Nội'))
```
