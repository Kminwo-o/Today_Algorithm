### 2024-02-10
|                     문제번호                     | 문제이름 | 나의 풀이 |
|:--------------------------------------------:|:----:|:---------: |
| [9084](https://www.acmicpc.net/problem/9084) |  동전  | [풀이](https://github.com/Kminwo-o/BaekJoon-Algorithm/blob/main/%EB%B0%B1%EC%A4%80/Gold/9084.%E2%80%85%EB%8F%99%EC%A0%84/%EB%8F%99%EC%A0%84.java) |

### 동전

우선 동전을 모두 받은 다음 각 동전 -한 금액이 0이 아닌 경우에만 이전 금액의 경우의 수를 더하고 <br>\
0인 경우에는 경우의 수를 + 1 해줌으로서 dp를 채웠다.  <br>
최대 10000원, 동전의 개수가 20개 일 경우 20 * 10000으로 20만번의 반복문이 일어나게 된다.  <br>
혹시 이 부분에서 시간 제한이 걸리지는 않을까 생각했는데 그렇지는 않았다.  <br>
역시 구현부터 생각하는게 제일인 것 같다.