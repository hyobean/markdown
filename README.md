# markdown
마크다운 설명 

### 11. 표
|번호|아이디|이름|레벨|이메일|등록일|
|:---------|:---------|:---------|---------:|:---------------|:---------:|
|1   |hyobean1|정효빈1|1|wjd4427947@naver.com|2023-01-27|
|2   |hyobean2|정효빈2|1|wjd4427947@naver.com|2023-01-27|
|3   |hyobean3|정효빈3|1|wjd4427947@naver.com|2023-01-27|
|4   |hyobean4|정효빈4|1|wjd4427947@naver.com|2023-01-27|
|5   |hyobean5|정효빈5|1|wjd4427947@naver.com|2023-01-27|
|6   |hyobean6|정효빈6|1|wjd4427947@naver.com|2023-01-27|

### 10. 인라인
문단 중간에 `CODE` 를 넣을 수 있다.(고정 폭 폰트를 표시해야 할 때 사용)
예를 들어 `question_list = Question.objects.order_by('-create_date')`  처럼

### 9. 강조
**spring**을 만끽하세요
spring을 만끽하세요

### 8. 이미지 넣기
![아반떼 N](doc/IMG_example.jpg "이미지 삽입 예시")

### 7. 하이퍼 링크
[e클래스](https://cafe.daum.net/pcwk "e클래스의 cafe입니다.")

### 6. 가로 라인
---
***
--------------

### 5. 코드 블록
```
def index(request):
    ''' Question 목록 '''
    # list order create_date desc
    print('index 레벨로 출력')
    question_list = Question.objects.order_by('-create_date')  # order_by('-필드') desc, asc, order_by('필드')
    context = {'question_list': question_list}
    print('question_list:{}'.format(question_list))

    return render(request, 'pybo/question_list.html', context)
```

### 4. 목록
1. 아이템1
2. 아이템2  
  9. 단계 하위 아이템  
    3. 단계 하위 아이템  
9. 아이템3

+ 아이템 1
- 아이템 2
  - 1단계 하위 아이템
    * 2단계 하위 아이템


순서 없는 목록
* 목록 이름
- 목록
+ 목록

순서 있는 목록
1. 목록 이름
2. 목록
3. 목록 3번

### 3. 인용문
> 여기에 인용할 내용을 넣으면 된다.
> 빈 줄이 없으면 자동으로 인용 상자에 포함.

### 2. 헤더
# 헤더1
## 헤더2
### 헤더3
#### 헤더4
##### 헤더5

### 1. 문단 구분을 위한 개행
문단을 작성한다. (개행 공백 2개)   
겨울이 가고 봄이 온다.
