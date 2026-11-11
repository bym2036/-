# 💌 배영민 님의 디지털 롤링페이퍼 (Digital Rolling Paper)

누구나 접속하여 따뜻한 축하와 응원의 메시지를 남길 수 있는 공개용 웹 롤링페이퍼 서비스입니다.

![Preview](https://images.unsplash.com/photo-1517842645767-c639042777db?auto=format&fit=crop&w=1000&q=80)

## ✨ 주요 기능
- **공개 메모 작성**: 접속하는 누구나 로그인 없이 닉네임과 함께 메시지 등록 가능
- **감성 커스텀 스티커 & 컬러**: 6가지 파스텔 메모지 색상 및 축하 이모티콘 스티커 선택
- **실시간 저장 및 조회**: Supabase Database를 이용한 실시간 데이터 영구 보관
- **폭죽 애니메이션**: 메시지 등록 시 팡파레(Confetti) 효과
- **반응형 디자인**: PC 모니터부터 모바일 스마트폰 화면까지 완벽 대응
- **원클릭 링크 복사**: 친구 및 지인들에게 카카오톡 등으로 즉시 공유 가능

## 🛠 기술 스택 (Tech Stack)
- **Frontend**: HTML5, Tailwind CSS, Vanilla JavaScript, Lucide Icons
- **Backend / Database**: Supabase (PostgreSQL + Row Level Security)
- **Deployment**: Vercel & GitHub

## 🚀 빠른 시작 가이드

### 1. Supabase 데이터베이스 세팅
1. [Supabase](https://supabase.com)에 로그인 후 새 프로젝트(`New Project`)를 생성합니다.
2. 좌측 메뉴의 **SQL Editor**로 이동합니다.
3. 이 저장소의 `supabase-setup.sql` 파일 내용을 복사하여 붙여넣고 **Run** 버튼을 클릭합니다.
4. 좌측 메뉴 **Project Settings** > **API**로 이동하여 다음 두 가지를 복사합니다:
   - `Project URL`
   - `anon public` Key

### 2. 코드에 Supabase 키 연결
`index.html` 파일을 열고 상단의 설정을 본인의 정보로 변경합니다:
```javascript
const SUPABASE_URL = '여기에_복사한_Project_URL_붙여넣기';
const SUPABASE_ANON_KEY = '여기에_복사한_anon_key_붙여넣기';
```

### 3. Vercel 배포
1. 본 프로젝트를 GitHub에 업로드(Push)합니다.
2. [Vercel](https://vercel.com)에서 **Add New...** > **Project**를 클릭합니다.
3. 방금 올린 GitHub 저장소를 선택하고 **Deploy** 버튼을 누르면 10초 만에 나만의 라이브 URL이 생성됩니다!

