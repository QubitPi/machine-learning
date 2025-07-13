Independent Setup of Italian ASR Notebook
=========================================

[This notebook](./Italian%20ASR.ipynb) requires [dedicated dependency](./requirements.txt) which should be setup and run
with the following commands:

```cnosole
cd italian-asr
python3 -m virtualenv .venv
source .venv/bin/activate
pip3 install -r requirements.txt
python3 -m ipykernel install --user --name=python3 && jupyter notebook
```

> [!NOTE]
> 
> The numpy used in this notebook has been downgraded to 1.x, because Whisper was trained in 2022 using numpy 1.x. Newer
> versions of numpy such as 2.x has shown some incompatibility on Whisper
