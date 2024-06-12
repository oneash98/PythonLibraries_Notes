tqdm -> 진행상황 확인 
<br>

tqdm
```python
from tqdm import tqdm # 주피터 노트북에서는 from tqdm.notebook import tqdm

for i in tqdm(iterable):
    code
```

```python
pbar = tqdm(iterable)

for i in pbar:
    pbar.set_description(f"Processing {i}") # 상태메시지
    code

pbar.close()

### 또는 ###

with tqdm(iterable) as pbar:
    for i in pbar:
        code

### 또는 ###

with tqdm(iterable) as pbar:
    for i in iterable:
        code
        pbar.update(1)
```