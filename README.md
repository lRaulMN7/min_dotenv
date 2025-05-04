<h1 align="center"> Minimal Dotenv </h1>
<h3 align="center"> Experimental dotenv loader </h3>  

</br>

## ⚙️ Installation

You can install `min_dotenv` using your preferred Python dependency manager:

```bash
pip install min-dotenv
```

Make sure you have Python 3.12 or higher installed.


## 💧 Usage

Given an environment file (e.g. `.env`) with key-value pairs
```
# Comments in your .env file are allowed
variable_name = "variable_content"
another_var_name = 123
```

You can **hydrate** these variables into Python’s `os.environ` using `min_dotenv`

```python
import os
from min_dotenv import hyd_env
hyd_env('.env')

for name, val in os.environ.items()
    print(f"{name}: {val}")
```

Example output:
```bash
variable_name: variable_content
another_var_name: 123
```

## 🔖 License

Licensed under the [MIT License](LICENSE).  
© 2025 Raúl Telo Sánchez