# 2주차 과제

## Q1

다음은 Calculator 클래스이다.

<pre><code>class Calculator:
    def __init__(self):
        self.value = 0

    def add(self, val):
        self.value += val</code></pre>

위 클래스를 상속하는 UpgradeCalculator를 만들고 값을 뺄 수 있는 minus 메서드를 추가해 보자. 즉 다음과 같이 동작하는 클래스를 만들어야 한다.

<pre><code>cal = UpgradeCalculator()
cal.add(10)
cal.minus(7)

print(cal.value) # 10에서 7을 뺀 3을 출력</code></pre>

## Q2

객체변수 value가 100 이상의 값은 가질 수 없도록 제한하는 MaxLimitCalculator 클래스를 만들어 보자. 즉 다음과 같이 동작해야 한다.

<pre><code>cal = MaxLimitCalculator()
cal.add(50) # 50 더하기
cal.add(60) # 60 더하기

print(cal.value) # 100 출력</code></pre>

단 반드시 다음과 같은 Calculator 클래스를 상속해서 만들어야 한다.

<pre><code>class Calculator:
    def __init__(self):
        self.value = 0

    def add(self, val):
        self.value += val</code></pre>