### 2024-03-11
|                     문제번호                     |  문제이름  | 나의 풀이  |
|:--------------------------------------------:|:------:|:------:|
| [2812](https://www.acmicpc.net/problem/2812) | 크게 만들기 | [풀이](https://github.com/Kminwo-o/BaekJoon-Algorithm/blob/main/%EB%B0%B1%EC%A4%80/Gold/2812.%E2%80%85%ED%81%AC%EA%B2%8C%E2%80%85%EB%A7%8C%EB%93%A4%EA%B8%B0/%ED%81%AC%EA%B2%8C%E2%80%85%EB%A7%8C%EB%93%A4%EA%B8%B0.java) |

### 크게 만들기
처음에 생각했을 때, 단순히 numbers[pre]가 numbers[now]보다 작고 k번을 넘지 않았으면 pre를 지우고 now를 남겨주면 되는거 아닌가? 라고 생각했다. <br>
<br>
편하게 수를 넣고 빼기 위해서 Stack을 사용했다. numbers의 앞에서 부터 Stack이 비어있지 않고 지울 수 있는 횟수가 남았으며 현재 숫자가 Stack.top() 보다 큰 경우 while문을 통해 pop()해줬다.
그리고 이후 N이 최대 500,000이기 때문에 StringBuilder를 사용해 Stack 내용을 모두 빼서 sb에 담고 이것을 reverse()해서 출력했다. <br>
<br>
당연히 통과될 줄 알았는데 72%에서 틀렸습니다가 발생했다. 엣지케이스가 생각나지 않아 질문게시판을 들어갔더니 다음과 같은 반례가 있었다.
```java
5 1
54321

ans : 5432
output : 54321
```
숫자가 연속으로 이전 값이 가장 큰 경우 k개 만큼 빼야함에도 불구하고 그 이상의 길이로 출력되는 문제였다. 
이를 해결하기 위해 while(true)를 통해 stack의 size()가 n-k가 될 때 까지 pop()하고 난 다음에 sb.append를 해주었더니 통과되었다. <br>
<br>
괜히 골드 3이 아니었다. 실제 테스트에서 만났으면 엣지 케이스를 못 찾아서 틀렸을 것 같다.