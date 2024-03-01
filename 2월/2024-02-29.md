### 2024-02-29 (live)
|                     문제번호                     | 문제이름 | 나의 풀이 |
|:--------------------------------------------:|:----:|:---------: |
| [2096](https://www.acmicpc.net/problem/2096) |  내려가기  | [풀이](https://github.com/Kminwo-o/BaekJoon-Algorithm/blob/main/%EB%B0%B1%EC%A4%80/Gold/2096.%E2%80%85%EB%82%B4%EB%A0%A4%EA%B0%80%EA%B8%B0/%EB%82%B4%EB%A0%A4%EA%B0%80%EA%B8%B0.java) |

### 내려가기
DP 문제다. 최근 DP를 열심히 풀어서 그런가 바로 풀이방법을 생각해냈다. <br>
maxDP, minDP 배열을 만들고 값을 넣은 다음 가능한 값 중 최소, 최대 값을 골라 배열에 넣었다. <br>
<br>
이후 max[n][i] 중 가장 최대 값과 최소값을 찾아 출력했다. <br>