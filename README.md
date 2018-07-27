# vivi_spacy
Vivi_spacy contains Vietnamese models for spaCy. We trained word2vec on a combination of wikipedia and news corpus, vector size = 150. Pos tagger and DEP parser are trained on UD Vietnamese (http://universaldependencies.org/treebanks/vi/index.html)
## Installation 
1. Download vivi model directly using pip: e.g. pip install https://github.com/trungtv/vivi_spacy/raw/master/vi/vi_core_news_md-2.0.1/dist/vi_core_news_md-2.0.1.tar.gz

    You can also download from my google drive: https://drive.google.com/file/d/1d5boGovdupmynsgDRhHyk3E6pNhwFXff/view

2. This is a dirty patch while we are preparing to send spaCy a pull request 
    ```bash 
    cp vi/vi [your installed spaCy]/spacy/lang/vi
    ```
3. You may need to install pyvi as well
    ```bash 
    pip install pyvi 
    ```

## Usage: import as module 
```python
import spacy
nlp = spacy.load('vi_core_news_md')
doc = nlp('Cộng đồng xử lý ngôn ngữ tự nhiên'))
```
