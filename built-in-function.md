# Python-Quiz

Python Quiz


1. 빌트인 함수만을 이용하여서 주민등록번호 앞자리를 16진법을 표현하고 10진법으로 어떤수인지 다시 설명하세요.(print문으로 출력)

예) "0xdbd9b 의 10 진법은  900507 입니다."


2. dict()함수를 이용하여서, 아래 딕셔너리에 추가값을 입력하세요.   
dict_val = {'윤수': 25}   
추가값 : 핸드폰번호 - [본인 연락처]    


3. next()를 이용하여서 StopIteration Error를 발생시키세요.


4. 10 을 3으로 나눈 몫과 나머지를 튜플로 얻으세요 (글자수 제한 12글자)


5. O, X문제
id로 리턴된 'identity'는 중복되지 않는다.(O, X)
id의 값은 -- 제외한 JPython, Cython등에서는 메모리 주소를 나타낸다(O, X)
object는 인자를 받을 수도, callable 할수도 없다.(O, X)


6-1. 
[1, 2, 3, 4, 5] 리스트를 sorted 함수를 이용하여서 역순으로 반환시키세요.

6-2.
dict.get([key])는 해당 dict에서 해당하는 key값에 value 를 리턴합니다.
dict.get()을 이용하여서, 아래 dict를 value값 순서대로 key값을 리턴하세요.

dict_val = { 'a': 3, 'b':1, 'c': 2 }

기대값 : ['b', 'c', 'a']



7. 반장이 먹튀한 씨형님 키보드에서 '*'(별표, shift+ 8)키 와 '%'(퍼센트, shift+5)를 드디어 부셔먹었습니다.
  12의 3제곱을 10으로 나눈 나머지를 알고 싶은데 어떤 방법을 사용하면 될지 아래 보기에서 고르세요.

1) exec(10, 3, 12)

2) remaind( square(12, 3), 10 )

3) pow(12, 3, 10)

기대값 == (12 ** 3) % 10



8, 

```
class Good(object):
    ....
    
class Bad(object):
    ....
    
class NotBad(Good):
    ....
```

위와 같은 클래스를 이용하여 코드를 작성중에, 프로그램내에서 수많은 인스턴스를 무분별하게 생성하게 되버렸습니다.  
원하는 지점에서 각 인스턴스들의 `attr` 들을 아래 조건에 맞춰 관리하고자 합니다.
빈칸을 채우세요

```
조건

1. 인스턴스가 Good Class의 인스턴스면 어떠한 조작도 하지 않습니다.
2. 인스턴스가 Bad Class의 인스턴스이면 instance.some 에 값을 가지고 있다면, 해당 값을 제거해야 합니다.
3. Bad Class 인스턴스가 some의 값을 가지고 있지 않다면, worst라는 attr에 True(bool)값을 넣어야 합니다.
4. 모든 빈칸에는 built-in function을 넣고싶습니다.
```


```
코드

def check_instance(ins):
  # instance를 인자로 받습니다.
  
  if [  빈 칸 1 ] : # Good인스턴스인지 확인
    return True
  if [ 빈 칸 2 ] : # Bad인스턴스인지 확인
    if [ 빈 칸 3] : # some 라는 attr를 가지고 있는지 확인
      [ 빈 칸 4 ] # 해당값(some) 제거    
    else:
      [ 빈 칸 5 ] # worst attr에 값 입력()

```


8-1.

힘들게 코드를 짠 다음 물한잔 먹고왔더니, NotBad라는 클래스가 Good class를 상속받았는지, Bad class를 상속받았는지 기억이 나지 않습니다.
class가 정의된 코드를 열지않고, Python Shell에서 각 class를 import해와서 확인하는 방법이 있을까요?
built-in function으로 가능하다면  어떻게 하면될까요?

