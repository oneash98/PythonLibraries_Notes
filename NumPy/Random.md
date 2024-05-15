```python
import numpy as np

# rand(): 0~1 사이 난수 array 생성
np.random.rand(n) # n개 생성
np.random.rand(n, m, ...)

# randint(): 임의의 정수
np.random.randint(n, m) # n~m 사이 임의의 정수
np.random.randint(n, m, size = i) # i개만큼 array로 반환

# randn(): 표준정규분포 N(0, 1)에 맞게 난수 반환
np.random.randn(n) # 평균 0, 표준편차 1인 정규분포에서 난수 n개 반환

# normal(): 정규분포에 맞게 난수 반환
np.random.normal(n, m, size =i) # 평균 n, 표준편차 m인 정규분포에서 난수 i개 반환
```