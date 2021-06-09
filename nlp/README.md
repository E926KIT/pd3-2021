# 環境のセットアップ
```
conda create -n nlp jupyter scikit-learn matplotlib pandas

conda activate nlp

conda install -c pytorch pytorch torchtext cudatoolkit=11.1 -c nvidia  # cf. https://pytorch.org/get-started/locally/
conda install -c conda-forge sentencepiece pytorch-lightning
# pip install transformers
```

<strike>最後の行で `conda install -c huggingface transformers` とやると conflict のためインストールに失敗する（何がコンフリクトしているのかは表示されず）</strike>

```
conda install -c conda-forge transformers
```
