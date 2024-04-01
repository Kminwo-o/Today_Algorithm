### 2024-03-29
|                     문제번호                     |      문제이름       | 나의 풀이  |
|:--------------------------------------------:|:---------------:|:------:|
| [5397](https://www.acmicpc.net/problem/5397) | 키로거 | [풀이](https://github.com/Kminwo-o/BaekJoon-Algorithm/blob/main/%EB%B0%B1%EC%A4%80/Silver/5397.%E2%80%85%ED%82%A4%EB%A1%9C%EA%B1%B0/%ED%82%A4%EB%A1%9C%EA%B1%B0.java) |

### 키로거

풀이는 다음과 같다.
> 1. Stack을 두 개를 활용한다.
> 2. "<"나 ">"가 나오면 스택에서 하나씩 빼서 left나 right로 넘긴다.
> 3. password입력이 모두 끝나면 모두 rightStack으로 몰아넣은 다음 pop하여 출력한다.

솔직히 시간초과가 날 줄 알았는데 나지 않았다.