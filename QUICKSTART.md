# hexo-theme-cola 빠른 시작 가이드

> `hexo-theme-cola`는 `Hexo` 기반의 블로그 테마로, 스타일은 **간결함**을 추구합니다.
> 
> 화려한 인터페이스나 복잡한 기능 없이, 사용자가 블로그 작성에 집중할 수 있도록 설계되었습니다.

## 시작하기

### 1. Hexo 프로젝트 초기화

먼저 Hexo로 프로젝트를 초기화합니다:

```bash
hexo init blog
```

### 2. 테마 클론

프로젝트 디렉토리로 이동한 후, `themes` 디렉토리에 테마를 클론합니다:

```bash
git clone git@github.com:Aizener/hexo-theme-cola.git themes/hexo-theme-cola
```

### 3. 테마 설정

프로젝트 루트 디렉토리의 `_config.yml` 파일에서 테마를 설정합니다:

```yaml
theme: hexo-theme-cola
```

### 4. 의존성 설치 및 실행

의존성을 설치한 후, 다음 명령어로 사이트를 생성하고 서버를 실행합니다:

```bash
npm install
hexo clean && hexo g && hexo s
```

## 페이지 생성

테마 설치 후 다음 페이지들을 생성해야 합니다:

1. **로그 페이지**: `hexo new page log`
2. **友链 페이지**: `hexo new page link`
3. **소개 페이지**: `hexo new page about`
4. **분류 페이지**: `hexo new page categories`
5. **태그 페이지**: `hexo new page tags`
6. **도구 페이지**: `hexo new page tools`

> **참고**: 필요한 페이지만 생성하면 됩니다.

### 로그 항목 생성

로그 페이지에 개별 로그 항목을 추가하려면 다음 명령어를 사용합니다:

```bash
hexo new page --path log/logName "logName"
```

이 명령어는 `log` 디렉토리에 `logName`이라는 제목의 파일을 생성합니다. 일반 글 작성과 동일하게 작성하면 됩니다.

## 테마 설정

테마 디렉토리의 `_config.yml` 파일에서 다양한 설정을 변경할 수 있습니다:

### 기본 설정

```yaml
# 사이트 제목
title: Cola의 블로그

# 작성자 이름 (좌측 사이드바)
author_name: Cola.

# 좌측 사이드바 태그 (2개만 가능)
tag1: 중二
tag2: 宅

# GitHub 링크
github_url: https://github.com/your-username

# 좌측 사이드바 좌우명 (2줄)
motto_prev: "꽃은 다시 피지만, 사람은 다시 젊어지지 않는다"
motto_last: "단순하고 평범한 소년"

# 사이트 공개 날짜 (운영 기간 계산용)
public_date: 2022-02-16
```

### 메뉴 설정

```yaml
# 좌측 사이드바 메뉴
menu:
  - [홈, '/', 'icon-shouye']
  - [로그, '/log', 'icon-rizhi']
  - [友链, '/link', 'icon-youqinglianjie']
  - [소개, '/about', 'icon-guanyuwomen']
```

### 友链 설정

```yaml
# 友链: [아바타, 이름, 링크]
links:
  - ['https://example.com/avatar.png', '친구 이름', 'https://example.com']
  - ['https://example.com/avatar2.png', '친구 이름2', 'https://example2.com']
```

### 공지사항

```yaml
# 우측 사이드바 공지사항
notice: 안녕하세요~ 환영합니다. Cola의 블로그에 오신 것을 환영합니다!
```

### 음악 플레이리스트

```yaml
# 우측 음악 목록: [제목, 아티스트, 링크, 커버 이미지]
musics:
  - ['노래 제목', '아티스트', 'http://example.com/music.mp3', 'https://example.com/cover.jpg']
  - ['노래 제목2', '아티스트2', '/music/kabuda.mp3', 'https://example.com/cover2.jpg']
```

### 개인 소개

```yaml
# 개인 소개 정보
likes:
  - 이름: 홍길동
  - 나이: 27
  - 성별: ♂
  - 고향: 서울특별시
  - 현재 거주지: 서울특별시 강남구
  - 직업: 웹 프론트엔드 개발자
  - 취미: 게임, 수영, 체스
```

### 저작권 정보

```yaml
# 저작권 정보
copyright: © 2024 Cola. All rights reserved.
```

## 참고 자료

원본 가이드: [hexo-theme-cola 사용 방법](https://aizener.github.io/2022/02/17/%E5%A6%82%E4%BD%95%E4%BD%BF%E7%94%A8hexo-theme-cola%E4%B8%BB%E9%A2%98/)

---

**이제 블로그를 시작할 준비가 되었습니다! (^▽^)**
