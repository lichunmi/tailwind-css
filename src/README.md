# CLI 사용법  
```plain text
    1. npm init -y                 = package.jason
    2. npm install -D tailwindcss  = package.jason에 devDependencies 생김
    3. npx tailwindcss init        = tailwind.config.js 파일 생김
                                    = tailwind.config.js -> 코드 수정(tailwindcss class쓰는걸 css파일로 만들어주는 코드)
                                                            index.html 은 src 폴더 안에 있어야함

                                                            /** @type {import('tailwindcss').Config} */
                                                            module.exports = {
                                                            content: ["./src/**/*.{html,js}"],
                                                            theme: {
                                                                extend: {},
                                                            },
                                                            plugins: [],
                                                            }
    4. src 폴더 생성
    5. src 폴더에 input.css 생성      =   하단 코드추가
                                        @tailwind base;
                                        @tailwind components;
                                        @tailwind utilities;
    6. src 폴더에 index.html 넣기
    7. npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
       (input.css 가 dist/output.css 폴더로 연결됨)

    ***** 7번 쉽게 사용 방법 : package.jason *****
                "scripts": {
                        "test": "echo \"Error: no test specified\" && exit 1"
                },
                ====
                "scripts": {
                    "dev": "npx tailwindcss -i ./src/input.css -o ./src/output.css --watch"
                },
    ***** 7번 명령어 대신 npm run dev 명령어 쓰면됨 *****  
    npm run dev
```  

# CDN 사용법  
```html
        <script src="https://cdn.tailwindcss.com"></script>
        <script>
            // 테마색 등록
            tailwind.config = {
            theme: {
                extend: {
                colors: {
                    jun: '#da373d',
                }
                }
            }
            }
        </script>
        <style type="text/tailwindcss">
            /* 같은 스타일 등록 */
            @layer components {
                .junjun {
                    @apply h-32 w-32;
                }
                .junjunjun {
                    @apply h-32 w-32 bg-jun;
                }
            }
        </style>
```