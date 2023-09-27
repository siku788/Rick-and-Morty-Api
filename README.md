# Rick and Morty API Data Extraction

In this document, we'll explore code snippets for extracting data from the Rick and Morty API and processing it using Python.

## Python Function: `main_request(url, endpoint, page_number)`

```python
def main_request(url, endpoint, page_number):
    full_url = f'{url}{endpoint}?page={page_number}'
    r = requests.get(full_url)
    return r.json()



