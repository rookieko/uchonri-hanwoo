# 한우면우촌리 · Uchonri Hanwoo

한우 도매·소매·유통 소개 사이트. 배포 도메인: https://uchonri-hanwoo.me/

## 로컬 실행

별도 패키지 설치나 빌드 없이 실행합니다.

```sh
cd /workspace/uchonri-hanwoo
python3 -m http.server 8000 --bind 127.0.0.1
```

`index.html`과 `assets/`를 함께 배포하세요. 기존 `CNAME`은 유지합니다.

## 구성

- `index.html`: 브랜드 소개, 정육·B2B 유통 안내, 용도별 탭, 납품 문의, 리센츠점 방문 안내, FAQ
- `assets/style.css`: 데스크톱·모바일 반응형 스타일
- `assets/main.js`: 모바일 메뉴, 키보드 접근 가능한 탭, 주소 복사
- `assets/hanwoo.webp`: 기존 HTML의 한우 사진을 별도 WebP로 최적화한 이미지
- `assets/favicon.svg`: 브랜드 파비콘

납품 문의는 기존 `admin@uchonri-hanwoo.me` 이메일로 연결하며, 메일 제목과 상담 항목을 미리 채웁니다. 이메일 버튼은 사용자의 메일 앱을 엽니다. 사이트에서 직접 메일을 발송하지 않습니다.

이미지는 기존 페이지에 표시된 [Wikimedia Commons 사진](https://upload.wikimedia.org/wikipedia/commons/3/30/%EC%84%9C%EC%82%B0_9%EB%AF%B8_%ED%95%9C%EC%9A%B0.jpg)을 재사용했으며, 페이지 하단의 출처 링크를 유지합니다. Google Fonts를 이용하며 시스템 글꼴로 대체할 수 있습니다.

## 정보 업데이트

네이버 스토어는 https://smartstore.naver.com/hanwoolll1217 에 연결합니다. 다른 매장의 상세 주소는 확인 후 추가할 수 있습니다. 현재 방문 안내는 기존 자료에 있는 리센츠점에 연결합니다. 가격, 등급, 납품 범위·조건은 확정된 내용을 제공받기 전까지 상담 안내로 표시합니다.

## 검증

Chromium에서 320, 390, 768, 1024, 1440px 화면의 가로 넘침과 이미지 로딩을 확인했습니다. 모바일 메뉴의 열기·닫기·Escape, 탭 클릭과 방향키·End 키, 주소 복사 성공 및 사용 불가 시 주소 표시, FAQ, 내부 링크, 정적 파일 응답을 확인했습니다.
