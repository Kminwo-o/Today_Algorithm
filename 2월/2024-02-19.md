### 2024-02-19
|                     문제번호                     | 문제이름 | 나의 풀이 |
|:--------------------------------------------:|:----:|:---------: |
| [1103](https://www.acmicpc.net/problem/1103) |  게임  | [풀이](https://github.com/Kminwo-o/BaekJoon-Algorithm/blob/main/%EB%B0%B1%EC%A4%80/Gold/1103.%E2%80%85%EA%B2%8C%EC%9E%84/%EA%B2%8C%EC%9E%84.java) |

### 게임

- dfs와 dp가 합쳐진 문제이다. 두 가지 개념을 섞는게 익숙하지 않다면 [뮤탈리스크](https://www.acmicpc.net/problem/12869)나 [내리막길](https://www.acmicpc.net/problem/1520)을 풀어보는 것도 도움이 될 것 같다. <br>
    <br>
    IF문으로 구멍에 빠졌을 때, 맵 밖으로 나갔을 때와 싸이클이 발생할 때를 잘 커트하고 최적화를 위해 이미 방문한 곳은 dp에 도달한 cnt를 기록하여 도달했을 때 기록된 cnt보다 작다면 바로 continue하여 dfs 하지 않도록 했다.
    <br><br>
    두 가지 개념을 섞어 써야하는 것, 싸이클을 확인할 아이디어, 게임이 끝나게 되는 상황에 대한 처리. 이 세 가지를 신경 써야하는 문제였다.
  