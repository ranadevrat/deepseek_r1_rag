# Opensource LLM App
Chatbot powered by opensource deepseek-r1:1.5b and RAG with llama index and flask

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install all dependencies.

```bash
pip install -r requirements.txt
```

Goto /data directory

Update dataprovider.py by add your Hugginging face key and OpenAI key for 
```python
key = ''
hg_key =""
```
### Choose LLM for Chatbot, Goto deepseek_r1_rag_app.py file and open in code editor 
goto code line 21:

```python
llm = Ollama(model="deepseek-r1:1.5b", request_timeout=120.0)
```
1. if you want to use OpenAI LLM then uncomment code line 77 and comment 78 line
2. if you want to use opensource LLM deepseek-r1 through Ollama
  Run below coommand to download deepseek-r1 1.5b model locally
```python
ollama pull deepseek-r1:1.5b
```   
   

## Usage of Project

Run below python file to productionize Chatbot powered by opensource LLM and RAG with llama index and flask
```python
deepseek_r1_rag_app.py
```
## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[GNU](https://choosealicense.com/licenses/gpl-3.0/)

