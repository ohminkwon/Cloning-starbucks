[![Netlify Status](https://api.netlify.com/api/v1/badges/9f2f756f-e1fc-48d9-9c07-b7d7433d8aaa/deploy-status)](https://app.netlify.com/sites/cloning-starbucks-ohminkwon/deploys)

# ☕️ Starbucks

스타벅스 메인 페이지(홈페이지)를 따라 만든 예제입니다.

[DEMO](https://cloning-starbucks-ohminkwon.netlify.app/)

![Starbucks](https://i.postimg.cc/vBh7gg5c/main-screenshot.jpg)

## 문자 인코딩(Character Encoding) 설정

문자가 인코딩되는 방식을 설정합니다.

```html
<meta charset="UTF-8" />
```

- `UTF-8`: 초성, 중성, 종성으로 구분하여 문자를 작성(권장)
- `EUC-KR`: 하나의 완성된 글자를 인식

## 뷰포트(Viewport) 렌더링 방식 설정

웹페이지가 화면(Viewport)에 표현되는 방식을 설정합니다.<br>
모바일 환경에서 적용 됩니다.

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

- `width=device-width` : 화면의 가로 너비를 각 디바이스(device)의 가로 너비와 동일하게 적용
- `initial-scale=1.0` : 화면의 초기 화면 배율(확대 정도)을 설정
- `user-scalable=no` : 사용자가 디바이스 화면을 확대(`yes`)/축소(`no`)할 수 있는지 설정
- `maximum-scale=1` : 사용자가 화면을 확대할 수 있는 최댓값
- `minimum-scale=1` : 사용자가 화면을 축소할 수 있는 최솟값

## 오픈 그래프(The Open Graph protocol)

웹페이지가 소셜 미디어(페이스북 등)로 공유될 때 우선적으로 활용되는 정보를 지정합니다.

**Slack**

![Slack Open Graph example](https://i.postimg.cc/QdZBDNWP/slack-message-og-example.jpg)

**KakaoTalk**

![KakaoTalk Open Graph example](https://i.postimg.cc/0yGzygYN/kakao-og-example.jpg)

[더 많은 오픈 그래프 속성 보기](https://ogp.me/)

```html
<meta property="og:type" content="website" />
<meta property="og:site_name" content="Starbucks" />
<meta property="og:title" content="Starbucks Coffee Korea" />
<meta property="og:description" content="스타벅스는 세계에서 가장 큰 다국적 커피 전문점으로, 64개국에서 총 23,187개의 매점을 운영하고 있습니다." />
<meta property="og:image" content="./images/starbucks_seo.jpg" />
<meta property="og:url" content="https://starbucks.co.kr" />
```

- `og:type` : 페이지의 유형(E.g, `website`, `video.movie`) 
- `og:site_name` : 속한 사이트의 이름
- `og:title` : 페이지의 이름(제목)
- `og:description` : 페이지에 대한 간단한 설명
- `og:image` : 페이지의 대표 이미지 주소(URL)
- `og:url` : 페이지 주소(URL)

## 트위터 카드(Twitter Cards)

웹페이지가 소셜 미디어(트위터)로 공유될 때 우선적으로 활용되는 정보를 지정한다.

[더 많은 트위터 카드 보기](https://developer.twitter.com/en/docs/twitter-for-websites/cards/guides/getting-started)

```html
<meta property="twitter:card" content="summary" />
<meta property="twitter:site" content="Starbucks" />
<meta property="twitter:title" content="Starbucks Coffee Korea" />
<meta property="twitter:description" content="스타벅스는 세계에서 가장 큰 다국적 커피 전문점으로, 64개국에서 총 23,187개의 매점을 운영하고 있습니다." />
<meta property="twitter:image" content="./images/starbucks_seo.jpg" />
<meta property="twitter:url" content="https://starbucks.co.kr" />
```

- `twitter:card` : 페이지(카드)의 유형(E.g, `summary`, `player`)
- `twitter:site` : 속한 사이트의 이름
- `twitter:title` : 페이지의 이름(제목)
- `twitter:description` : 페이지의 간단한 설명
- `twitter:image` : 페이지의 대표 이미지 주소(URL)
- `twitter:url` : 페이지 주소(URL)