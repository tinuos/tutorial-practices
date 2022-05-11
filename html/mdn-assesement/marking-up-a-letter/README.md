# MDN - HTML Assesement: Marking up a letter

- [실습 페이지](https://developer.mozilla.org/ko/docs/Learn/HTML/Introduction_to_HTML/Marking_up_a_letter)
- 실습에 필요한 자료는 [맨 아래](#실습-자료) 참고

---
---

## 요구사항 분석

### 블럭 및 구조 관련 시맨틱

- HTML 기본 구조 
  - Doctype, html, head, body ✔
- 텍스트와 내용에 따라 적절한 시맨틱 태그 사용
  - 단락 ✔
  - 표제 구분 ✔
  - 목록 구분 ✔
  - 날짜 및 주소 관련 태그 사용 ✔

### 인라인 시맨틱

- 보내는 사람 이름, 받는 사람 이름, Tel, Email 은 `strong` ✔
- 문서 안에 나오는 4개의 날짜는 관련 태그 사용 > `time`과 datetime 속성 ✔
- 첫번째 주소와 날짜는 클래스 설정 - **sender-column** ✔
  - CSS 적용 확인하기 ✔
- 문서 내에 5개의 약어는 관련 태그를 사용하고 전체 이름 설정 ✔
- 문서 내 위첨자, 아래첨자 사용 ✔
  - 화학식 ✔
  - 숫자 103, 104 > 지수 처리 ✔
- 텍스트에서 2개의 적당한 단어를 강조하기 > `strong` 또는 `em` ✔
- 2개의 하이퍼링크를 적절한 제목에 추가하기 > `a` 요소 ✔
  - 주소는 `http://example.com` 활용 ✔
- 대학 모토 인용 그리고 적절한 요소에서 인용이 표시되어야 함 ✔

### head 요소 관련

- 문자인코딩 > `utf-8` ✔
- 작가 정보 포함 ✔
- 제공된 스타일 시트 적용 ✔

---

## 정리

- 편지(letter) 형태의 내용을 마크업
- 주로 텍스트에 대한 내용을 마크업하는 내용을 실습
- 문장으로 풀어쓴 요구사항과 예제 이미지를 참고하여 마크업을 진행

> 현실에서 글을 쓸 때 특수한 텍스트의 표기(지수, 서수, 화학식 등)나 문단, 제목 등의 문서 구조를 HTML의 태그들로 마크업하여 표현 가능하다는 것을 실습을 통해 확인.

> 참고 이미지가 있어서 쉽게 작성할 수 있었지만, 실제 어떠한 내용에 대해 직접 마크업을 하기 위해서는 많은 연습이 필요할 것 같다. 콘텐츠나 구조를 특성을 분석할 수 있는 능력과 정확한 태그를 사용하는 습관을 길러야 겠다. 

---

## 실습 자료

### Raw text

```
Dr. Eleanor Gaye
Awesome Science faculty
University of Awesome
Bobtown, CA 99999,
USA
Tel: 123-456-7890
Email: no_reply@example.com

20 January 2016

Miss Eileen Dover
4321 Cliff Top Edge
Dover, CT9 XXX
UK


Re: Eileen Dover university application

Dear Eileen,

Thank you for your recent application to join us at the University of Awesome's science faculty to study as part of your PhD next year. I will answer your questions one by one, in the following sections.

Starting dates

We are happy to accommodate you starting your study with us at any time, however it would suit us better if you could start at the beginning of a semester; the start dates for each one are as follows:

First semester: 9 September 2016
Second semester: 15 January 2017
Third semester: 2 May 2017

Please let me know if this is ok, and if so which start date you would prefer.

You can find more information about important university dates on our website.


Subjects of study

At the Awesome Science Faculty, we have a pretty open-minded research facility — as long as the subjects fall somewhere in the realm of science and technology. You seem like an intelligent, dedicated researcher, and just the kind of person we'd like to have on our team. Saying that, of the ideas you submitted we were most intrigued by are as follows, in order of priority:

Turning H2O into wine, and the health benefits of Resveratrol (C14H12O3.)
Measuring the effect on performance of funk bassplayers at temperatures exceeding 30°C (86°F), when the audience size exponentially increases (effect of 3 × 103 increasing to 3 × 104.)
HTML and CSS constructs for representing musical scores.

So please can you provide more information on each of these subjects, including how long you'd expect the research to take, required staff and other resources, and anything else you think we'd need to know? Thanks.


Exotic dance moves

Yes, you are right! As part of my post-doctorate work, I did study exotic tribal dances. To answer your question, my favourite dances are as follows, with definitions:

Polynesian chicken dance
A little known but very influential dance dating back as far as 300BC, a whole village would dance around in a circle like chickens, to encourage their livestock to be "fruitful".
Icelandic brownian shuffle
Before the Icelanders developed fire as a means of getting warm, they used to practice this dance, which involved huddling close together in a circle on the floor, and shuffling their bodies around in imperceptibly tiny, very rapid movements. One of my fellow students used to say that he thought this dance inspired modern styles such as Twerking.
Arctic robot dance
An interesting example of historic misinformation, English explorers in the 1960s believed to have discovered a new dance style characterized by "robotic", stilted movements, being practiced by inhabitants of Northern Alaska and Canada. Later on however it was discovered that they were just moving like this because they were really cold.

For more of my research, see my exotic dance research page.

Yours sincerely,
Dr Eleanor Gaye

University of Awesome motto: "Be awesome to each other." -- The memoirs of Bill S Preston, Esq
```

### CSS code

```css
body {
  max-width: 800px;
  margin: 0 auto;
}

.sender-column {
  text-align: right;
}

h1 {
  font-size: 1.5em;
}

h2 {
  font-size: 1.3em;
}

p,ul,ol,dl,address {
  font-size: 1.1em;
}

p, li, dd, dt, address {
  line-height: 1.5;
}
```

---
---