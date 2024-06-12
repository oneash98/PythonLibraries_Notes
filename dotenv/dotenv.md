dotenv -> 환경변수 관리
<br>

.env 파일 생성
```vim
# .env

KEY = 'value'
```
<br>

dotenv
```python
pip install python-dotenv

import os
from dotenv import load_dotenv

load_dotenv()

KEY = os.getenv("KEY")
```