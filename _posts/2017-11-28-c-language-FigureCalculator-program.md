---
title: "C언어 도형계산기"
author: 4season
date: 2017-11-28 22:33
category: Report
tags: ["Programming", "C", "FigureCalculator"]
image:
  src: https://www.dropbox.com/s/ax3yvrxe2ppd7o2/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%2827%29.png?dl=1
  copyright: Delighit Lab
---
 ```c
#include <stdio.h>


int main() {
	float a, b;
	int ch;

	printf("도형을 선택하시오.(1.원, 2.삼각형, 3.사각형) :");
	scanf_s("%d", &ch, 1);

	switch (ch) {
	case 1:
		printf("1. 원을 선택하셨습니다.\n");
		printf("반지름 입력 : ");
		scanf_s("%f", &a, 1);
		printf("원의 면적 = %.2f\n", a * a * 3.14);
		break;
	case 2:
		printf("2. 삼각형을 선택하셨습니다.\n");
		printf("밑변 입력 : ");
		scanf_s("%f", &a, 1);
		printf("높이입력 : ");
		scanf_s("%f", &b, 1);
		printf("삼각형의 면적 = %.2f\n", a * b / 2);
		break;
	case 3:
		printf("3. 사각형을 선택하셨습니다.\n");
		printf("가로입력 : ");
		scanf_s("%f", &a);
		printf("세로입력 : ");
		scanf_s("%f", &b);
		printf("사각형의 면적 = %.2f\n", a * b);
	}
	return 0;
}
```
<br>

C언어로 만든 `도형` 계산기 입니다. <br>
기능은 `원, 삼각형, 사각형` 이 있습니다. <br>

<img scr="https://www.dropbox.com/s/tqjubsvdavb409z/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%2826%29.png?dl=1" width="70%"> <br>
<img src="https://www.dropbox.com/s/ax3yvrxe2ppd7o2/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%2827%29.png?dl=1" width="70%"> <br>

한글이 깨저버린건 정말로 기분탓이지만, 소스에 적힌대로 질문하는 것이니 당황하시지말구 한번 계산해보세요!
