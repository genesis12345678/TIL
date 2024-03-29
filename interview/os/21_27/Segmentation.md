# 세그먼테이션이란 무엇인가요?

- 메모리를 **서로 크기가 다른** 논리적인 블록 단위인 [세그먼트(`segment`)](https://github.com/genesis12345678/TIL/blob/main/interview/os/11_20/Paging.md#segmentation)로 분할하고 메모리를 할당하여 물리 주소를 논리 주소로 변환하는 것을 말한다.
- 미리 분할하는 것이 아니라 사용할 시점에 할당된다.
- 내부 단편화는 없지만 **외부 단편화가 발생할 수 있다.**

## 세그먼테이션과 페이징을 비교해 주세요.

- 세그먼테이션은 [페이징](https://github.com/genesis12345678/TIL/blob/main/interview/os/11_20/Paging.md#%ED%8E%98%EC%9D%B4%EC%A7%95%EC%9D%B4%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%B8%EA%B0%80%EC%9A%94)보다 **보호와 공유 면에서 더 낫다.**
- 세그먼테이션은 `read`, `write`,`execute` 권한을 테이블에 추가하는데, 이때 이것을 **논리적으로 나누기 때문에** 해당 비트를 설정하기 간단하고 안전하다.
- 반면 페이징은 `Code + Data + Stack` 영역이 존재할 때 이를 **일정한 크기로 나누기 때문에** 영역이 섞여 비트를 설정하기 까다로워 질 수 있다.
- 공유 면에서도 마찬가지로, 페이징은 영역과 섞일 가능성이 존재하지만, 세그먼테이션은 정확히 영역을 나누므로 더 효율적으로 공유를 할 수 있다.
- 현재 대부분은 **세그먼테이션보다 페이징 기법을 많이 사용한다.**
- 왜냐하면, 세그먼테이션의 세그먼트 크기가 **일정하지 않고 다양하기 때문이다.**
- 세그먼트의 크기가 다양하기 때문에 **다양한 `hole`이 발생해 외부 단편화가 발생하여** 메모리 낭비가 크게 된다.

<br>

### 참고
- [참고 블로그](https://code-lab1.tistory.com/57)