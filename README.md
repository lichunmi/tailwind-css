# tailwind-css
[위니브 강의자료](https://www.notion.so/paullabworkspace/Tailwind-CSS-c3aebde0f224435ba615fc12e6abc843)

- vsc Extension
- JetBrains IDE 사용시 @apply 문법이 HTML 문서 내에서 사용 가능

# VS CODE Snippets 설정
스니팻 설정 > 설정 > User Snippets > html.jason > 코드 추가

```javascript
      "print to console": {
      "prefix": "!ko",
      "body": [
            "<!DOCTYPE html>",
            "<html lang=\"ko\">",
            "<head>",
            "<meta charset=\"UTF-8\">",
            "<meta http-equiv=\"X-UA-Compatible\" content=\"IE=edge\">",
            "<meta name=\"viewport\" content=\"width=device-width, initial-scale=1.0\">",
            "<title>$1</title>",
            "</head>",
            "<body>",
            "	$2",
            "</body>",
            "</html>"
      ],
      "description": "한국어 페이지용 html 템플릿"
	}
```

# Node JS
**mkdic test**  
->폴더 test 만들기

**cd test**  
->test 폴더 안으로 들어가기

**clear**  
->화면을 지우겠다

[shift]+[insert] 누르면 붙혀넣기  
**npm instal -D tailwindcss**  
**npm tailwindcss init**  
-> node_modules 폴더 생김  
-> tailwind.config.js  
