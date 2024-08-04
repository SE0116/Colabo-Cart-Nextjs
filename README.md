# Colabo-Cart-Nextjs
장바구니 페이지 구현 웹 페이지

<img src="https://img.shields.io/badge/Nextjs-000000?style=flat-square&logo=nextdotjs&logoColor=white"/> <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=JavaScript&logoColor=white"/>

<img src="https://github.com/SE0116/Colabo-Cart/assets/87646738/8e1f79d6-a58f-4b18-ba05-2274ad932861" width="270" height="300">
 

## 주요 기능
### 장바구니에 담기
- 원하는 서비스를 장바구니에 담고, 수량 및 할인 적용 여부를 선택할 수 있게 했습니다.

![salon_1](https://github.com/SE0116/Colabo-Cart/assets/87646738/cfa26d90-f89c-4bcc-ae83-e9fdfa4afbd6)
![salon_2](https://github.com/SE0116/Colabo-Cart/assets/87646738/76eef002-50e3-4c81-9e66-3e94c56d615f)

### 장바구니 목록 삭제
- 장바구니에 담긴 시술 / 할인 아이템을 삭제 후 남아있는 아이템들의 총 가격을 계산합니다.

![salon_3](https://github.com/SE0116/Colabo-Cart/assets/87646738/f785e4c2-73b2-4387-bd3b-29f22e508ccb)


## 구현 사항 체크리스트
- [] `item`, `discount`는 각각 장바구니로 추가/삭제 가능
- [] 동일한 아이템을 장바구니로 담을 수 없음
- [] `item`의 수량 선택 가능 eg. `item x 3`
- [] `discount`의 할인 대상 `item`을 선택하지 않으면 장바구니에 담긴 모든 `item`을 할인 적용
- [] `discount`의 할인 대상 `item`을 선택한 경우 선택한 항목만 할인 적용
- [] 장바구니에 담긴 내용이 변경될 때 마다 사용자에게 최종 금액을 표시
- [] 최종 금액은 `currency_code`에 따라 표시
  - 현재 가능한 화폐 단위는 KRW, USD, EUR 세 가지입니다.


## 프로젝트 구조
```bash
├── frontend
│   ├── node_modules
│   ├── public
│   ├── src
│   │   ├── app                       # 라우팅 관련 파일
│   │   │    ├── layout.tsx 
│   │   │    └── page.tsx 
│   │   ├── components                # UI 컴포넌트
│   │   └── lib                       # 유틸리티 및 헬퍼 함수
│   ├── package.json
│   └── tsconfig.json
└── README.md
``` 