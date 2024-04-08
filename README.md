# cai-webagent
Using pyenv package to set 
```bash
$ python --version
Python 3.12.2
```
## prod dependencies:
```bash
cp ./env_example ./env
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements_lock.txt
```
## dev env:
```bash
cp ./env_example ./env
python3 -m venv .venv
source .venv/bin/activate
pip install -U crewai duckduckgo-search langchain_community
```
freeze packages 
```bash
pip freeze > requirements_lock.txt
```

TODO:
- agent: python executor and file writer
- tools: hiearchical folder structure with annotations
- agent: tool picker from /tools folder based on use case eval 
