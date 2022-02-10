# Python/Js 코딩테스트 kit


## 1. 입출력

>
  - python
```python
# 입력 받은것 공백을 기준으로 분할. 리스트로 반환
a,b = input().split()
# 한줄에 여러 숫자를 입력받아서 리스트에 넣기
a = list(map(int,input().split()))
# sys
import sys
sys.stdin.readline().rsplit('\n')
```
- Javascript
```javascript
```

## 2. 리스트/배열



### 2-1. 순회
>
- python
```python
for i in arr:
	print(i)
# 연속된 숫자 생성 
arr = list(range10) # arr = [0,1,2,3,4,5,6,7,8,9]
```
- Javascript
```javascript
for(let i in arr){
	console.log(i)
}
```

### 2-2. 추가
>
- python
```python
# 끝에 요소 추가. 원본 배열을 변경
arr.append(1)
# 특정 인덱스에 요소 추가 insert(index,element)
arr.insert(len(arr),999)
```
- Javascript
```javascript
let arr = [0]
// 끝에 요소 추가
arr.push(1) // arr = [0,1]
// 끝에 요소 추가. 원본 배열을 변경하지 않는다
arr.concat(1) // arr = [0]
```

### 2-3. 삭제
>
- python
```python
#마지막 요소를 삭제하고 반환. 원본 배열 변경
a = arr.pop()
#특정한 요소 삭제하고 반환
a = arr.pop(x)
#특정한 요소 삭제
del arr[x]
#첫번째로 나오는 요소 삭제
a.remove(x)
```
- Javascript
```javascript
// 마지막 요소를 삭제하고 반환. 원본 배열 변경
let a = arr.pop()
```

### 2-3-1. 자르기
>
- python
```python
arr = [1,2,3,4,5]
#원본 배열을 변경하지 않음
arr[3:4] #[4], arr = [1,2,3,4,5]
```
- Javascript
```javascript
let arr = [1,2,3,4,5]
//원본 배열을 변경
arr.splice(3,4) // # [4,5], arr = [1,2,3]
//원본 배열을 변경하지 않음
arr.slice(3,4) // # [4,5], arr = [1,2,3,4,5]
```

### 2-4. join
>
- python
```python
arr = ['1','2','3','4']
#원본 배열 변경x
''.join(arr) # '1,2,3,4'
```
- Javascript
```javascript
let arr = [1,2,3,4]
//원본 배열 변경x
arr.join() // '1,2,3,4'
arr.join('') // '1234'
```

### 2-5. reverse
>
- python
```python
# 원본 배열이 변경된다
arr.reverse()
```
- Javascript
```javascript
// 원본 배열이 변경된다
arr.reverse()
```

### 2-6. includes, count, index
>
- python
```python
arr = [1,2,3]
# 요소의 존재 여부
1 in arr # True
1 not in arr # False
# 요소의 개수 세기
arr.count(1)
# 요소의 위치 반환
arr.index(1)
```
- Javascript
```javascript
let arr = [1,2,3];
// 요소의 존재 여부
arr.includes(2); // true
```

### 2-7. 함수
>
#### sort
- python
```python
arr = [1,5,3,2,4]
# 원본 배열이 변경됨
arr.sort() #[1,2,3,4,5]
arr.sort(reverse=True) #[5,4,3,2,1] 
# 원본 배열이 변경되지 않음
sorted(arr) #[1,2,3,4,5]
```
- Javascript
```javascript
let arr = [1,5,3,2,4]
// 원본 배열이 변경됨
arr.sort((a,b)=>a-b) //[1,2,3,4,5]
arr.sort((a,b)=>b-a) //[5,4,3,2,1] 
```


