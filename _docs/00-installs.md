
## Prep
```bash
cd my_pydantic
uv init
uv add ruff

# edit pyproject.toml
# requires-python = ">=3.11"
uv self update
uv python install 3.11
uv python pin 3.11
uv venv # this ensure that python has been downgraded to 3.11 from 3.12
source .venv/bin/activate
python --version # check if 3.11 is there
```

Check:
```bash
(my_pydantic) dp@P920:~/Desktop/Github/my_pydantic$ ll
total 48
drwxrwxr-x  5 dp dp 4096 Jan 27 12:57 ./
drwxrwxr-x 13 dp dp 4096 Jan 27 12:10 ../
drwxrwxr-x  8 dp dp 4096 Jan 27 12:40 .git/
-rw-rw-r--  1 dp dp   66 Jan 27 11:55 .gitattributes
-rw-rw-r--  1 dp dp   89 Jan 27 12:11 hello.py
-rw-rw-r--  1 dp dp  177 Jan 27 12:48 pyproject.toml
-rw-rw-r--  1 dp dp    5 Jan 27 12:54 .python-version
-rw-rw-r--  1 dp dp  285 Jan 27 12:28 README.md
-rw-rw-r--  1 dp dp 5245 Jan 27 12:12 uv.lock
drwxrwxr-x  4 dp dp 4096 Jan 27 12:57 .venv/
drwxrwxr-x  2 dp dp 4096 Jan 27 12:40 .vscode/
(my_pydantic) dp@P920:~/Desktop/Github/my_pydantic$ 
```


## Install [Pydantic AI](https://ai.pydantic.dev/install/)
```bash
uv add pydantic-ai
uv add 'pydantic-ai[logfire]'
```

```bash
uv add asyncio
uv add dataclasses
uv add devtools
uv add html-to-markdown
uv add python-dotenv
```