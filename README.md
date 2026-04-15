<div align="center">

# 🖼️ Picture Story Generator

**Transform your images into emotionally rich, AI-crafted stories**

[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4o-412991?style=flat-square&logo=openai&logoColor=white)](https://platform.openai.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)](LICENSE)

<br/>

> **Lab Exercise 3** — A no-install, browser-based web app that lets you upload images, pick an emotion, and generate a short story using OpenAI's GPT-4o Vision model.

<br/>

[🇺🇸 English](#-english) · [🇰🇷 한국어](#-한국어)

</div>

---

<br/>

| | | |
|:---:|:---:|:---:|
| <img width="280" alt="스크린샷 2026-04-15 오후 9 43 39" src="https://github.com/user-attachments/assets/793efc21-2cc4-4887-8f8f-5801431306cf" /> | <img width="280" alt="스크린샷 2026-04-15 오후 9 44 54" src="https://github.com/user-attachments/assets/55945b21-3b50-442a-b81a-970748b4f755" /> | <img width="280" alt="스크린샷 2026-04-15 오후 9 45 07" src="https://github.com/user-attachments/assets/621c5940-39b8-4a01-8507-8575dde0c8d4" /> |

## 🇺🇸 English

### 📁 Project Files

| File | Description |
|------|-------------|
| [`picture-story.html`](picture-story.html) | Main app — English default with 🇺🇸/🇰🇷 language toggle |
| [`그림이야기.html`](그림이야기.html) | Legacy Korean-only version (kept for reference) |

---

### ✨ Features

- 🎨 **18 Dynamic Emotion Themes** — each emotion transforms the entire page palette, typography, and mood
- 🖼️ **Multi-image Upload** — drag & drop or click to upload multiple images; order is preserved as story sequence
- 🤖 **GPT-4o Vision** — OpenAI's multimodal model analyzes every image and weaves them into a cohesive narrative
- ⚡ **Zero Setup** — plain HTML/CSS/JS, no build tools, no server, no dependencies
- 🔒 **Privacy First** — your API key lives only in browser memory; nothing is stored or logged

---

### 🚀 Getting Started

#### Prerequisites

| Requirement | Details |
|-------------|---------|
| **OpenAI API Key** | Must have access to `gpt-4o`. Get one at [platform.openai.com/api-keys](https://platform.openai.com/api-keys) |
| **Internet connection** | Required for OpenAI API calls and Google Fonts |
| **Modern browser** | Chrome, Safari, Firefox, or Edge (latest recommended) |

#### Running the App

Simply open the HTML file in your browser — no server needed.

```bash
# macOS — default browser
open picture-story.html

# macOS — specific browser
open -a "Google Chrome" picture-story.html
open -a "Safari" picture-story.html
```

Or **double-click** `picture-story.html` in Finder.

---

### 📖 How to Use

```
Step 1 ──► Enter your OpenAI API Key  (sk-...)
Step 2 ──► Choose an emotion
Step 3 ──► Upload one or more images
Step 4 ──► Click "✨ Generate Story"
Step 5 ──► Read your story!
```

#### Step 1 — API Key
Enter your `sk-...` key in the **🔑 OpenAI API Key** field at the top of the page.

#### Step 2 — Choose an Emotion
Click any emotion button to set the story's mood. The entire page theme updates instantly.

<details>
<summary>View all 18 emotions</summary>

| | | |
|---|---|---|
| 😊 Happy | 😢 Sad | 😰 Suspenseful |
| 🥰 Excited | 🌌 Mysterious | 🌸 Warm |
| 🍂 Bittersweet | 😄 Cheerful | 😱 Scary |
| ✨ Fantastical | 🌙 Lonely | 🕊️ Nostalgic |
| 🦁 Brave | 🌿 Peaceful | 🌊 Dreamlike |
| ⚡ Epic | 🐣 Cute | 🎢 Thrilling |
| 🌋 Furious | 💔 Heartbroken | 🦋 Hopeful |
| 🎭 Dramatic | 🌧️ Melancholic | |

</details>

#### Step 3 — Upload Images
Drag & drop images onto the dashed area, or click it to browse. Upload multiple images — they'll appear in numbered order as the story sequence. Supported formats: **JPG · PNG · WEBP**

#### Step 4 — Generate
Once all three inputs are ready, the **✨ Generate Story** button activates. Click it and wait ~5–15 seconds.

#### Step 5 — Read & Iterate
Your story appears in the **📜 Generated Story** section with the selected emotion tag and character count. Change the emotion or swap images and regenerate as many times as you like.

---

### 🌈 Dynamic Emotion Themes

When you select an emotion, the page transforms:

| Element | What Changes |
|---------|-------------|
| **Background** | Smooth gradient transition (0.7s animation) |
| **Borders & Accents** | Card borders, buttons, and inputs update to match the theme |
| **Typography** | Lyrical emotions (sad, nostalgic…) use serif + italic; energetic emotions use sans-serif |

---

### ⚙️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Front-end | Plain HTML5 / CSS3 / Vanilla JavaScript |
| AI Model | OpenAI GPT-4o (Vision + Text) |
| Fonts | Google Fonts — Playfair Display, Inter |
| Build tools | None — single file, runs anywhere |

---

### 🔒 Security Notes

> ⚠️ **Never commit your API key.** This app is intended for local use only.

- Your API key is stored **only in browser memory** for the duration of the session
- The key is sent **directly to OpenAI's API** — it never passes through any third-party server
- Do **not** deploy this file on a public web server without a secure backend key proxy

---

### ❓ Troubleshooting

| Symptom | Fix |
|---------|-----|
| Generate button is grayed out | All three required: API key + emotion + at least 1 image |
| `API Error: 401` | API key is invalid or revoked — double-check at [platform.openai.com](https://platform.openai.com) |
| `API Error: 429` | Rate limit exceeded — wait a moment and retry |
| Images won't upload | Ensure file is JPG/PNG/WEBP; try compressing if over 20MB |
| Text renders as boxes | Check internet connection — Google Fonts must load |

---

<br/>

## 🇰🇷 한국어

### 📁 프로젝트 파일

| 파일 | 설명 |
|------|------|
| [`picture-story.html`](picture-story.html) | 메인 앱 — 영어 기본, 🇺🇸/🇰🇷 언어 전환 지원 |
| [`그림이야기.html`](그림이야기.html) | 레거시 한국어 전용 버전 (참고용) |

---

### ✨ 주요 기능

- 🎨 **18가지 동적 감정 테마** — 감정 선택 시 페이지 전체의 색상, 서체, 분위기가 변경
- 🖼️ **다중 이미지 업로드** — 드래그&드롭 또는 클릭으로 여러 장 업로드 가능, 업로드 순서가 이야기 순서로 반영
- 🤖 **GPT-4o Vision** — OpenAI 멀티모달 모델이 이미지를 분석하고 하나의 이야기로 엮어냄
- ⚡ **설치 불필요** — 순수 HTML/CSS/JS, 빌드 도구·서버·의존성 없음
- 🔒 **프라이버시 보호** — API Key는 브라우저 메모리에만 저장, 외부 서버로 전송되지 않음

---

### 🚀 시작하기

#### 사전 요구사항

| 항목 | 내용 |
|------|------|
| **OpenAI API Key** | `gpt-4o` 사용 권한 필요. [platform.openai.com/api-keys](https://platform.openai.com/api-keys) 에서 발급 |
| **인터넷 연결** | OpenAI API 호출 및 Google Fonts 로드에 필요 |
| **최신 브라우저** | Chrome, Safari, Firefox, Edge 최신 버전 권장 |

#### 실행 방법

HTML 파일을 브라우저에서 바로 열면 됩니다. 별도 서버 설치가 필요 없습니다.

```bash
# 기본 브라우저로 열기
open 그림이야기.html

# 특정 브라우저로 열기
open -a "Google Chrome" 그림이야기.html
open -a "Safari" 그림이야기.html
```

또는 Finder에서 `그림이야기.html` 파일을 **더블클릭**하세요.

---

### 📖 사용 방법

```
1단계 ──► OpenAI API Key 입력  (sk-...)
2단계 ──► 감정 선택
3단계 ──► 이미지 업로드
4단계 ──► "✨ 이야기 생성하기" 클릭
5단계 ──► 이야기 감상!
```

#### 1단계 — API Key 입력
페이지 상단 **🔑 OpenAI API Key** 입력란에 `sk-...` 형식의 키를 입력합니다.

#### 2단계 — 감정 선택
감정 버튼을 클릭해 이야기 분위기를 설정합니다. 페이지 전체 테마가 즉시 변경됩니다.

<details>
<summary>18가지 감정 전체 보기</summary>

| | | |
|---|---|---|
| 😊 행복한 | 😢 슬픈 | 😰 긴장감 있는 |
| 🥰 설레는 | 🌌 신비로운 | 🌸 따뜻한 |
| 🍂 슬프고 아름다운 | 😄 유쾌한 | 😱 무서운 |
| ✨ 환상적인 | 🌙 외로운 | 🕊️ 그리운 |
| 🦁 용감한 | 🌿 평화로운 | 🌊 몽환적인 |
| ⚡ 웅장한 | 🐣 귀여운 | 🎢 짜릿한 |
| 🌋 분노한 | 💔 상처받은 | 🦋 희망찬 |
| 🎭 극적인 | 🌧️ 우울한 | |

</details>

#### 3단계 — 이미지 업로드
점선 영역에 이미지를 드래그&드롭하거나 클릭하여 업로드합니다. 여러 장 업로드 시 번호 순서가 이야기 순서가 됩니다. 지원 형식: **JPG · PNG · WEBP**

#### 4단계 — 이야기 생성
세 가지 입력이 모두 완료되면 **✨ 이야기 생성하기** 버튼이 활성화됩니다. 클릭 후 약 5~15초 소요됩니다.

#### 5단계 — 결과 확인 및 반복
**📜 생성된 이야기** 섹션에 선택 감정 태그와 글자 수와 함께 이야기가 표시됩니다. 감정이나 이미지를 바꿔 원하는 만큼 재생성할 수 있습니다.

---

### 🌈 감정별 동적 테마

| 항목 | 변경 내용 |
|------|-----------|
| **배경** | 감정에 맞는 그라데이션으로 전환 (0.7초 애니메이션) |
| **테두리·강조색** | 섹션 카드, 버튼, 입력창 색상이 테마에 맞게 변경 |
| **글씨체** | 서정적 감정(슬픈, 그리운 등)은 명조체+이탤릭 / 활동적 감정은 고딕체 |

---

### ⚙️ 기술 스택

| 레이어 | 기술 |
|--------|------|
| 프론트엔드 | 순수 HTML5 / CSS3 / Vanilla JavaScript |
| AI 모델 | OpenAI GPT-4o (Vision + Text) |
| 폰트 | Google Fonts — Noto Serif KR, Noto Sans KR |
| 빌드 도구 | 없음 — 단일 파일, 어디서든 실행 가능 |

---

### 🔒 보안 유의사항

> ⚠️ **API Key를 절대 코드에 직접 입력하거나 공개 저장소에 업로드하지 마세요.**

- API Key는 **브라우저 메모리에만** 저장되며 세션이 끝나면 사라집니다
- 키는 **OpenAI API로 직접 전송**되며, 제3자 서버를 경유하지 않습니다
- 이 파일을 **공개 웹 서버에 배포할 경우** 반드시 백엔드 키 프록시를 사용하세요

---

### ❓ 자주 묻는 문제

| 문제 | 해결 방법 |
|------|-----------|
| 버튼이 비활성화 상태 | API Key 입력 + 감정 선택 + 이미지 1장 이상 — 세 가지 모두 필요 |
| `API 오류: 401` | API Key가 잘못되었거나 만료됨. [platform.openai.com](https://platform.openai.com) 에서 재확인 |
| `API 오류: 429` | API 사용량 한도 초과. 잠시 후 다시 시도하세요 |
| 이미지가 안 올라감 | JPG/PNG/WEBP 형식인지 확인, 20MB 초과 시 압축 필요 |
| 글씨가 깨져 보임 | 인터넷 연결 확인 (Google Fonts 로드 필요) |

---

<br/>

<div align="center">

Made with ❤️ for **SNU AI Application** · Lab Exercise 3

</div>
