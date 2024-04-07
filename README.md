### 2024-04-07
|                      문제번호                      | 문제이름 | 나의 풀이  |
|:----------------------------------------------:|:----:|:------:|
| [13414](https://www.acmicpc.net/problem/13414) | 수강신청 | [풀이](https://github.com/Kminwo-o/BaekJoon-Algorithm/blob/main/%EB%B0%B1%EC%A4%80/Silver/13414.%E2%80%85%EC%88%98%EA%B0%95%EC%8B%A0%EC%B2%AD/%EC%88%98%EA%B0%95%EC%8B%A0%EC%B2%AD.java) |

### 수강신청

문제 자체는 쉬웠다. 나는 여태까지 HashMap은 순서가 일정하다고 생각했으나 그렇지 않았다.<br>
그래서 입력된 순서를 보장하기 위해 HashMap에서 value기준으로 정렬이 가능한지 알아보던 중 LinkedHashSet이라는 자료구조를 알게 되었다. <br>
<br>
해당 자료구조는 HashSet의 형태로 작동하지만 입력된 순서를 보장해준다. <br>
그래서 LinkedHashSet에 값을 넣고 contains == true라면 값을 지우고 다시 수험번호를 넣어주는 형태로 로직을 작성했다. StringBulider를 사용해서 수강 가능한 인원까지만 sb에 담고 출력하였다.