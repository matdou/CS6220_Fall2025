# How to reproduce

## Setup

1. Make sure you have **Python 3.9+** installed.  
2. Install all required packages:
```bash
pip install -r requirements.txt
```

If you don’t have Jupyter installed:
```bash
pip install notebook
```



## Hugging Face Login


1. Go to [https://huggingface.co/settings/tokens](https://huggingface.co/settings/tokens)  
2. Click **New Token** → choose **Read** access  
3. Copy your token and log in:

**Option A: uncomment those lines inside the notebook**
```python
from huggingface_hub import login
login(token="YOUR_TOKEN_HERE")
```

**Option B: from the terminal**
```bash
huggingface-cli login
```



## Run the Notebook

After logging in, open and run the notebook.



## Notes


- GPU is necessary for inference (`torch.cuda.is_available()`).  

---

**Author:** Mathis Doutre  
**File:** `notebook.ipynb`  
