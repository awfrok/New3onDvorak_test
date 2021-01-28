#  한글 글쇠 배열: Dvorak 영문 글쇠 배열의 부호와 기호를 그대로 사용하는 신세벌식 조합방식의 한글 글쇠 배열

![layout_HangulNew3onDvorak](https://user-images.githubusercontent.com/78065210/106119672-4fb8a400-610a-11eb-8ed2-8bb637b36941.jpg)

## 설명

1. 드보락의부호와 기호의 위치를 그대로 사용함.
   (즉 드보락의 알파벳에만 한글 글쇠를 배치함.)
2. 오른손으로 시작해서 왼손으로 끝나는 세벌식의 특징을 차용함.
3. 겹자음과 복모음의 연타와 조합을 허용하는 신세벌식의 특징을 차용함.
4. 일부 빈도가 낮은 받침자음에 대해 오른 손에 배열하여 왼손 부담을 오른손에 나눔.
5. 한 글쇠가 초성, 중성, 종성 중에서 최대 두 가지 기능만 함.



## 특징

1. 엄지와 검지를 사용하는 빈도가 높음.
2. 네 손가락의 기본자리를 사용하는 빈도가 높음.
3. 오른손보다 왼손이 상대적으로 부담이 큼(왼손이 중성과 종성을 담당함.)
4. 불쌍한 약지를 배려하고 새끼를 기본자리에서 활용함.



## 동기

1. 2006년부터 영문에 대해 드보락을 선택하여 연습하여 만족하였음.
2. 한글의 경우 MS Windows의 두벌식을 계속 사용하다가
   아무래도 한글을 입력할 때 왼손 손목에 부담을 많이 느껴서
   여러 세벌식을 연습하였으나
   기본 자리위치를 벗어나는 글쇠가 많아고 손지 크지 않아서 쉽지 않았음.
3. 새롭게 글쇠 배열을 만들기로 하고, 
   찾아보니 세벌식보다 신세벌식이 내 의도를 잘 살릴것으로 생각함.
4. 김용묵의 날개셋입력기에 대해 알게 되어
   자체 배열을 만들었음.



## 과정

1. 한글 자음과 모음의 초성, 중성, 종성 출현 빈도에 대해 연구 논문을 찾아봄.
2. 초성에 대해, 
   빈도가 높은 초성을 기본자리와 검지와 중지의 자리에 배치하고, 
   빈도가 낮은 초성을 그외 자리에 배치함.
   별로 어렵지 않았음.
3. 중성과 종성에 대해,
   빈도를 고려하여 상반된 자리를 지정해서 왼손 검지와 중지의 연타를 줄임.
   (오래전 일이라 기억이 불명료함.)
4. 중성에 대해, 
   빈도가 높은 중성을 왼손 기본자리에 배치하고, 
   빈도가 낮은 모음을 검지가 멀리 움직이는 자리와 약지를 사용하는 자리에 배치함.
5. 종성에 대해, 
   중성과 연타를 줄이는 방향으로 배열하여
   리듬감을 살리려고 하였음. 
6. 종성의 기본자리에 대해서,
    일 년 정도 계속 바꾸면서 시험하여서 지금의 자리를 확정함.



## 목표

> https://kldp.org/node/160815 와 https://kldp.org/node/161067 를 발견하고 가능성이 있다고 생각함.

1. 리눅스 uim, uim-byeoru를 통해 구현하기.
2. 리눅스 libhangul을 통해 구현하기. (맥오에스의 구름 입력기도 시험하기.)
3. 윈도우에서 입력기를 구현하기.



## License

open-source나 개인저작에 대해 아직 license 등을 어떻게 지정해야 하는지 몰라서 추후에 하겠다.



#### 혼잣말

오래 전에 개발해 두고 리눅스에서 사용하려고 시도하였으나 실패하였다. 몇 년을 잊고 있다가 얼마 전부터 리눅스를 다시 써야 할 일이 생겼고, 한글글쇠배열을 해결하려고 검색하던 중, 며칠 전 나빌레라 님이 KLDP에 2019년에 작성한 글을 발견하였다. 그래서 급히 깃허브를 만들어서 배우면서 기록으로 남기고 있다. 