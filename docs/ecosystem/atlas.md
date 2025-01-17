# AtlasDB

This page covers how to use Nomic's Atlas ecosystem within LangChain.
It is broken into two parts: installation and setup, and then references to specific Atlas wrappers.

## Installation and Setup
- Install the Python package with `pip install nomic`
- Nomic is also included in langchains poetry extras `poetry install -E all`

## Wrappers

### VectorStore

There exists a wrapper around the Atlas neural database, allowing you to use it as a vectorstore.
This vectorstore also gives you full access to the underlying AtlasProject object, which will allow you to use the full range of Atlas map interactions, such as bulk tagging and automatic topic modeling.
Please see [the Nomic docs](https://docs.nomic.ai/atlas_api.html) for more detailed information.



To import this vectorstore:
```python
from langchain.vectorstores import AtlasDB
```

For a more detailed walkthrough of the Chroma wrapper, see [this notebook](../modules/indexes/examples/vectorstores.ipynb)
