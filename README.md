## 2024-04-23
|                     문제번호                     | 문제이름 | 나의 풀이  |
|:--------------------------------------------:|:----:|:------:|
| [2493](https://www.acmicpc.net/problem/2493) |  탑   | [풀이](https://github.com/Kminwo-o/BaekJoon-Algorithm/blob/main/%EB%B0%B1%EC%A4%80/Gold/2493.%E2%80%85%ED%83%91/%ED%83%91.java) |

## 탑
### 문제 풀이
- 답안 확인 여부 : ❌ <br>
- 문제 풀이 시간 : 28분

### 코드 작성시 도전한 풀이 방법
<details>
<summary> 풀이 방법 </summary>
<div markdown="1">

- Stack : Array로 받아서 하나씩 idx를 높여가면서 확인하고 StringBuilder에 append 하는 방식으로 풀었음
> 1. Array 배열에 탑을 순서대로 input 한다.
> 2. cnt 0 부터 시작해서 n까지 진행한다.
>   - 왼쪽으로 레이저가 날아가기 때문에 역순으로 시작해야할 것 같지만 이래나 저래나 어차피 idx 값을 들고 가기 때문에 똑같음. 
> 3. stack이 비어 있다면 제일 왼쪽 탑이거나 보다 높은 탑이 없기 때문에 StringBuilder에 0을 추가하고 stack에 now를 push한다.
> 4. stack이 있는 경우 now 값이 stack의 top 보다 크다면 stack을 pop한다.(어차피 도달할 수 없음 + 지나왔던 탑 중에 높았던 탑 찾아줘야함) 
> 5. cnt가 n과 같아지면 sb를 출력
</div>
</details>

### 문제 풀이시 주의점
1. 시간초과가 쉽게 날 수 있기 때문에 n번 만큼만 돌아야한다.

### 코드 작성 시 놓쳤던 부분
없음.

### 어려움을 느꼈던 부분
없음.