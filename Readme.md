# FastAPI

FastAPI framework, high performance, easy to learn, fast to code, ready for production

![FastAPI](https://camo.githubusercontent.com/86d9ca3437f5034da052cf0fd398299292aab0e4479b58c20f2fc37dd8ccbe05/68747470733a2f2f666173746170692e7469616e676f6c6f2e636f6d2f696d672f6c6f676f2d6d617267696e2f6c6f676f2d7465616c2e706e67)

FastAPI is a modern, fast (high-performance), web framework for building APIs with Python 3.7+ based on standard Python type hints.

## Requirements
Python 3.7+

FastAPI stands on the shoulders of giants:

<ul>
<li><a href="https://www.starlette.io/" class="external-link" target="_blank">Starlette</a> for the web parts.</li>
<li><a href="https://pydantic-docs.helpmanual.io/" class="external-link" target="_blank">Pydantic</a> for the data parts.</li>
</ul>

## Installation
```bash
pip install fastapi
pip install "uvicorn[standard]"
```

## Run it
```bash
uvicorn main:app --reload
```
<ul>
<li><code>main</code>: the file <code>main.py</code> (the Python "module").</li>
<li><code>app</code>: the object created inside of <code>main.py</code> with the line <code>app = FastAPI()</code>.</li>
<li><code>--reload</code>: make the server restart after code changes. Only do this for development.</li>
</ul>

## Check it

<p>Open your browser at <a href="http://127.0.0.1:8000/items/5?q=somequery" class="external-link" target="_blank">http://127.0.0.1:8000/items/5?q=somequery</a>.</p>

You will see the JSON response as:

```json
{"item_id": 5, "q": "somequery"}
```

## Interactive API docs

<p>Now go to <a href="http://127.0.0.1:8000/docs" class="external-link" target="_blank">http://127.0.0.1:8000/docs</a>.</p>

<p>You will see the automatic interactive API documentation (provided by <a href="https://github.com/swagger-api/swagger-ui" class="external-link" target="_blank">Swagger UI</a>)</p>