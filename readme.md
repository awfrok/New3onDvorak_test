작성: 2021.01.28.

#  (가칭) 새세벌식 한글 글쇠 배열: Dvorak 배열의 영문에 한글 글쇠를 배치하고, Dvorak 배열의 부호와 기호를 그대로 사용함.

![KeyboardLayout_HangulNew3onDvorak_v0.2.2.jpg](https://github.com/awfrok/HangulNew3onDvorak/blob/master/KeyboardLayout_HangulNew3onDvorak_v0.2.2.jpg?raw=true)

## 설명

1. 드보락의 알파벳에 한글 글쇠를 배치함.
2. 드보락의 부호와 기호의 위치를 그대로 사용함.
3. 글쇠 하나가 초성, 중성, 종성 중에서 최대 두 가지 기능만 함.
4. 오른손으로 시작해서 왼손으로 끝나는 세벌식의 특징을 차용함.
5. 겹자음의 연타와 복모음의 조합을 허용하는 신세벌식의 특징을 차용함. shift를 눌러 ㄲ, ㄸ을 입력하기보다 연타를 하락하여 새끼의 부담을 줄임. 어차피 2타의 시간이 비슷하다고 생각함.
6. 빈도가 낮은 종성(ㅈ,ㅋ,ㅊ)과 중성(ㅑ,ㅠ)을 오른손 자리에 배열하여 왼손 자리의 부족함을 해결.
6. F와 X를 기본자리에서 지나치게 벗어났다고 보고, 빈도가 가장 낮은 중성 (ㅖ,ㅒ), 종성(ㄷ)을 배치함.



## 특징 및 장단점

1. 검지와 중지를 다른 손가락보다 자주 사용함.
2. 네 손가락의 기본자리에 주로 사용하는 초성과 중성을 배열하였음.
3. 왼손이 중성과 종성 대부분을 담당하기 때문에 오른손보다 왼손이 상대적으로 부담이 큼.
4. 불쌍한 약지를 배려하고 새끼를 기본자리에서 활용함.
4. 기본 자리와 윗줄이 90%를 담당하고, 아랫줄이 10%를 담당함.

	> https://cafe.daum.net/3bulsik/6CY8/328
	>
	> https://cafe.daum.net/3bulsik/6CY8/345
	>
	> https://cafe.daum.net/3bulsik/6CY8/334



## 제작 동기

1. 2006년부터 영문에 대해 드보락을 선택하여 연습하여 만족하였음.
2. 한글의 경우 MS Windows의 두벌식을 계속 사용하다가
   아무래도 한글을 입력할 때 왼손 손목에 부담을 많이 느껴서
   여러 세벌식을 연습하였으나
   기본 자리위치를 벗어나는 글쇠가 많고 손이 크지 않아서 쉽지 않았음.
   부호와 기호를 입력하기 위해서 영문으로 바꾸는 부담도 컸음.
3. 새롭게 글쇠 배열을 만들기로 하고, 
   찾아보니 공세벌식보다 신세벌식의 조합방식이 내 의도를 잘 살릴것으로 생각함.
   
   > https://ko.wikipedia.org/wiki/%EC%84%B8%EB%B2%8C%EC%8B%9D_%EC%9E%90%ED%8C%90
4. 김용묵의 날개셋입력기에 대해 알게 되어
   자체 배열을 만들었음.



## 조건 및 과정

1. 한글 자음과 모음의 초성, 중성, 종성 출현 빈도에 대해 연구 논문을 찾아봄.

2. 초성에 대해, (별로 어렵지 않았음.)
   빈도가 높은 초성을 기본자리와 윗줄의 검지와 중지의 자리에 배치하고, 
   빈도가 낮은 초성을 그외 자리에 배치함.
   새끼를 기본자리에서 최대한 머무르도록 윗줄과 아랫줄에 초성 빈도가 가장 낮은 ㅌ,ㅍ 을 배치함.
   
3. 중성에 대해, 
   빈도가 높은 중성을 왼손 기본자리에 배치하고, 
   빈도가 낮은 모음을 검지가 멀리 움직이는 자리와 약지를 사용하는 자리에 배치함.
   
4. 종성에 대해, 
    중성과 연타를 줄이는 방향으로 배열하여
    리듬감을 살리려고 하였음.
    
5. 한 자리에 있는 중성과 종성에 대해,
    빈도를 고려하여 상반된 자리를 지정해서 왼손 검지와 중지의 연타를 줄임.
    높은 빈도의 중성과 낮은 빈도의 종성, 혹은, 낮은 빈도의 중성과 높은 빈도의 종성을 한 자리에 배치함.
    겹자음이 될 수 초성(ㄲ, ㄸ, ㅃ, ㅆ, ㅉ)의 자리에 중성을 배치할 수 없음.
    예외적으로 ㅈ의 경우 세 가지 초성 ㅈ, ㅉ, 종성 ㅈ을 담당함.
    
    



## 구현 및 목표

1. 리눅스 uim, uim-byeoru를 통해 구현함. 윈도우에서 날개셋 입력기를 사용함.

   > https://github.com/awfrok/uim-byeoru_for_HangulNew3onDvorak
   >
   
2. 리눅스 libhangul을 통해 구현하기. 

   > libhangul을 사용하는 맥오에스의 구름 입력기도 시험하기.



## 가능성

1. 이 방식의 조합 규칙을 사용하면, Qwerty자판에서 기호를 그대로 사용하면서 알파벳에만 한글 자모를 배치할 수 있다. 물론 효율적인 배치를 연구해야 한다.



## 가칭 "새세벌식"

1. 신세벌식의 '신'이 개발자 신광조의 성을 따르고 있어서 그것과 구분하려고 "새세벌식"으로 부른다.



## License

open-source나 개인 저작에 대해 아직 license 등을 어떻게 지정해야 하는지 몰라서 추후에 하겠다.



#### 혼잣말

오래 전에 개발해 두고 리눅스에서 사용하려고 시도하였으나 실패하였다. 몇 년을 잊고 있다가 얼마 전부터 리눅스를 다시 써야 할 일이 생겼고, 한글글쇠배열을 해결하려고 검색하던 중, 며칠 전 나빌레라 님이 KLDP에 2019년에 작성한 글을 발견하였다. 그래서 급히 깃허브를 만들어서 배우면서 기록으로 남기고 있다. 