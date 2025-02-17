# Link-Confirm 라이브러리

라이브러리에 대한 간단한 설명

## installation

이 라이브러리는 jsdelivr cdn을 사용합니다.
HTML의 `<head>` 부분에 다음과 같이 CDN을 작성하시면 됩니다.

이 코드는 jQuery에 기반하므로 반드시 jQuery가 먼저 불러와져야 합니다


```html
<script src="https://code.jquery.com/jquery-3.7.1.min.js"></script>
<script scr="https://cdn.jsdelivr.net/gh/sanghunlee1333/cdn/link-confirm/index.js"></script> 
```

## usage

확인창을 출력하고 싶은 `<a>`태그에 `.link-confirm' 이라는 클래스를 부여하여 사용할 수 있습니다.

```html
<a href = "https://www.google.com" class = "link-confirm">구글로 이동</a>
```

위와 같이 작성하면 `정말 이동하시겠습니까?` 라는 메세지가 나오며 확인을 누르면 href에 설정된 목적지가 나옵니다.

## customize

만약 사용자에게 보여줄 코멘트를 바꾸고 싶다면 `data-comment`라는 속성을 추가할 수 있습니다.

```html
<a href = "#" class = "link-confirm" data-comment = "정말 삭제하시겠습니까?">삭제하기</a>
```

`data-comment`가 설정된 경우 기본 메세지보다 우선적으로 출력됩니다.
