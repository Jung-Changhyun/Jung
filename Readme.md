# 인공지능 사관학교 프리코스 과제 목차

## 1주차 과제 (2020.05.21)
[1주차](https://github.com/Jung-Changhyun/Jung/blob/master/1%EC%A3%BC%EC%B0%A8%EA%B3%BC%EC%A0%9C.ipynb)

## 2주차 과제 (2020.05.31)
2주차 과제
>

파이썬 문제
인공지능 수학 문제
*주의사항

-- 문제에서 제시된 변수에 저장된 값을 직접 변경하는 것은 오답으로 처리됩니다. (예외도 있으니 문제설명을 자세히 읽어주세요)

-- 제시된 변수 이외의 변수를 추가해서 문제를 풀어도 됩니다 (문제 설명에 명시된 변수 변경만 불가합니다.)

파이썬 문제
01번 문제 (Data Type)
다음 변수 a, 변수 b, 변수 c의 자료형을 출력하세요.

In [0]:
# 주어진 변수(a, b, c) 직접 수정불가
a = 'str'
b = 123
c = True


print(a,b,c)
str 123 True
02번 문제 (for문)
다음 변수 num_list에 있는 요소를 모두 더한 값을 for문을 활용하여 변수 answer에 저장하고 그 값을 출력하세요.

In [0]:
# 주어진 변수(num_list) 직접 수정 불가
# for문을 사용 하지 않은 경우 오답처리
num_list = [1,2,3,4,5,6,7,8,9]
answer = 0

for i in num_list:
  answer += i
  print(answer)
1
3
6
10
15
21
28
36
45
03번 문제 (slice string)
다음 변수 date를 슬라이스해서 year(년), month(월), day(일)를 각각 출력하세요. (출력 : 2020 05 11)

(tip: None을 지우고 date를 슬라이싱해서 각각의 데이터를 저장하세요!)

In [0]:
# 주어진 변수(date)만 직접 수정불가, 다른 year, month, day 변수는 직접 수정가능
# 슬라이스를 사용 안 할 경우 오답처리
date = '20200511'

year = date[0:4]
month = date[4:6]
day = date[6:8]

print(year, month, day)
2020 05 11
04번 문제(for)
다음 변수 summary에 1 부터 100까지 모두 더한 값을 저장하여 출력하세요.

In [0]:
# 주어진 변수(summary) 직접 수정불가
summary = 0
for i in range(1,101):
  summary += i
print(summary)
5050
05번 문제(string reverse)
다음 변수 hangul의 문자열을 거꾸로 출력하세요. (출력:‘사바마라다나가’)

In [0]:
# 주어진 변수(hangul) 직접 수정불가
hangul = '가나다라마바사'

# 출력
print(hangul[::-1])
사바마라다나가
06번 문제(str -> list -> int 변환)
다음 변수 num에는 공백으로 구분된 4개의 점수가 들어 있습니다. 평균을 구해서 출력하세요.

In [0]:
# 주어진 변수(num) 직접 수정불가
num = "70 50 90 70"

#출력
sum =0
list_num = num.split()
list_num = list(map(int, list_num))

for i in list_num:
  sum += i
  avg = sum / len(list_num)
  print('평균 : ',avg)
평균 :  17.5
평균 :  30.0
평균 :  52.5
평균 :  70.0
07번 문제(if문)
다음 변수 n에 입력한 값이 짝수 일 경우 ‘짝수’를, 짝수가 아닐 경우 ‘짝수가 아닙니다’를 판별하여 출력하세요. (출력: 짝수 or 짝수가 아닙니다)

In [0]:
# 주어진 변수(n) 직접 수정불가
n = int(input('숫자를 입력해주세요'))

#출력
if n%2 == 0 :
  print('짝수')
else :
  print('짝수가 아닙니다.')
숫자를 입력해주세요1
짝수가 아닙니다.
08번 문제(산술 연산 및 list index)
직사각형의 대각선의 길이를 구하는 공식은 밑변의 제곱 + 높이의 제곱 = 대변의 제곱이다.

다음 변수 list_08에는 하나의 직사각형의 밑변과 높이가 저장되어 있습니다.

각각 밑변이 3이고 높이가 4일 때, 직사각형의 대변의 제곱의 길이를 출력하세요.

In [0]:
# 주어진 변수(list_08) 직접 수정불가
list_08 = [3, 4]

# 출력
sum = 0

def i (list) :
  return[i*i for i in list]

for su in i(list_08) :
  sum += su

  print(sum)
9
25
09번 문제(소수 판별 프로그램)
입력받은 숫자가 소수인지 아닌지 출력하는 프로그램을 작성 해 주세요. (출력 : 소수 or 소수가 아닙니다)

In [0]:
# 주어진 변수(num_10) 직접 수정불가
# 함수(prime_number) 직접 수정가능

num_10 = int(input('숫자를 입력해주세요'))

def prime_number(number):

    if number != 1:                 
     
        for i in range(2, number):  
           
            if number % i == 0:     
                return False    
    else:                       
        return False            

    return True                 
  
if prime_number(int(num_10)):
    print("소수")
else:
    print("소수가 아닙니다.")
숫자를 입력해주세요5
소수
인공지능 수학 문제
1번 문제 (Hypothesis)
다음 공식은 Hypothesis를 구하는 공식입니다. 다음과 같이 값이 주어졌을때 H(x)의 값을 구하시오.

W = 3
x = 10
b = 1
$$h(x) = Wx + b$$
정답 : 31
2번 문제 (Cost function)
다음 공식은 Cost를 구하는 공식입니다. 다음과 같이 값이 주어졌을때 cost의 값을 구하세요.

W = 2
x = [2, 4, 8]
y = [5, 12, 21]
(tip: x1=2, y1=5 / x2=4, y2=12 / x3=8, y3=21)

$$cost(W) =  \frac{1}{n}\sum_{i=1}^n (Wx^{(i)}-y^{(i)})^2$$
정답 : 242
3번 문제 (Logistic regression sigmoid function)
다음 공식은 로지스틱 시그모이드 함수입니다. x가 양의 무한대로 갈때 f(x)가 수렴하는 값을 구하세요.

대체 텍스트

정답 : 1
