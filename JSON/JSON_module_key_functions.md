## json.dumps

파이썬 객체를 JSON 형식으로 직렬화(serializing).
<br>
```python
import json

data = {'key1': 'value1', 'key2': 'value2'}
json_string = json.dumps(data)
```
<br>

## json.loads

JSON 형식의 문자열을 파이썬 객체로 역직렬화(deserializing).
<br>
```python
json_string = "{'key1': 'value1', 'key2': 'value2'}"
data = json.loads(json_string)
```
<br>

## json.dump

파이썬 객체를 JSON 형식으로 직렬화하여 파일에 저장
<br>
```python
data = {'key1': 'value1', 'key2': 'value2'}

with open("data.json", "w) as f:
    json.dump(data, f)
```
<br>

## json.load

파일에서 JSON 데이터를 읽어들여 파이썬 객체로 역직렬화
<br>
```python
with open("data.json", "r") as f:
    data = json.load(f)
```