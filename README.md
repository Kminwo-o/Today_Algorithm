### 2024-03-27
|                     문제번호                     | 문제이름  | 나의 풀이  |
|:--------------------------------------------:|:-----:|:------:|
| [5430](https://www.acmicpc.net/problem/5430) | AC | [풀이](https://github.com/Kminwo-o/BaekJoon-Algorithm/blob/main/%EB%B0%B1%EC%A4%80/Gold/5430.%E2%80%85AC/AC.java) |

### AC

Deque를 사용해서 풀이하는 문제이다. T는 최대 100, p는 최대 100,000이기 때문에 직접 배열을 돌리면 사고가 난다. <br>
따라서 다음과 같이 풀이한다.
> 1. Deque를 만든다.
> 2. reverse 상태를 파악하는 boolean 자료를 통해 reverse = true면 뒤에서, reverse = false면 앞에서 요소를 제거한다.
> 3. TC 케이스가 모두 돌아야하기 때문에 println을 하면 너무 출력이 느리기 때문에 sb를 통해 한번에 출력한다.

배열을 sort하기 보다 deque를 통해 앞 뒤로 빼냈다. deque를 사용하는 건 골드 5 정도여야 할 수 있는건가보다.