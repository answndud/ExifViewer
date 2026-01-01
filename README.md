# 📷 EXIF Viewer & Remover

이미지에 숨겨진 EXIF 메타데이터를 확인하고 안전하게 제거하는 웹 기반 프라이버시 도구입니다. 모든 처리는 브라우저에서 이루어져 개인정보가 외부로 전송되지 않습니다.

![Privacy](https://img.shields.io/badge/Privacy-100%25%20Local-green)
![EXIF](https://img.shields.io/badge/EXIF-View%20%26%20Remove-blue)
![No Server](https://img.shields.io/badge/Server-Not%20Required-orange)

## ✨ 주요 기능

### 📋 EXIF 메타데이터 분석
- **카메라 정보**: 제조사, 모델명, 렌즈, 소프트웨어
- **날짜/시간**: 촬영 일시, 수정 일시
- **촬영 설정**: ISO, 셔터 속도, 조리개, 초점 거리, 플래시
- **GPS 위치**: 위도/경도 좌표 및 Google Maps 링크

### ⚠️ 개인정보 경고
- GPS 좌표가 포함된 이미지 감지 시 경고 표시
- 민감한 정보 시각적 강조 (빨간색 표시)
- 지도에서 촬영 위치 확인 가능

### 🧹 메타데이터 제거
- Canvas API를 통한 완전한 메타데이터 제거
- 원본 화질 유지 (JPEG 92% 품질)
- 정리 전/후 파일 크기 비교

### 🔒 완벽한 프라이버시
- 100% 클라이언트 사이드 처리
- 서버 업로드 없음
- 네트워크 전송 없음

## 🚀 사용 방법

### 메타데이터 확인
1. 이미지를 업로드합니다 (드래그 앤 드롭 또는 클릭)
2. EXIF 메타데이터가 자동으로 분석되어 표시됩니다
3. GPS 정보가 있으면 경고와 함께 지도 링크가 표시됩니다
4. "전체 메타데이터 보기"를 클릭하면 모든 태그를 확인할 수 있습니다

### 메타데이터 제거
1. 이미지를 업로드합니다
2. "메타데이터 제거" 버튼을 클릭합니다
3. 처리가 완료되면 "정리된 이미지 다운로드"를 클릭합니다
4. 메타데이터가 제거된 안전한 이미지가 다운로드됩니다

## ⚠️ EXIF 메타데이터의 위험성

### 📍 위치 정보 노출
스마트폰으로 촬영한 사진에는 대부분 GPS 좌표가 포함되어 있습니다:
- 집 주소 노출 가능
- 직장 위치 추적 가능
- 자주 가는 장소 파악 가능

### 📅 시간 정보
- 촬영 날짜 및 시간
- 사용자의 일상 패턴 추론 가능

### 📱 기기 정보
- 사용하는 스마트폰/카메라 모델
- 소프트웨어 버전

## 🛠️ 기술 스택

| 분류 | 기술 |
|------|------|
| **프론트엔드** | HTML5, CSS3, Vanilla JavaScript |
| **EXIF 파싱** | exif-js 라이브러리 |
| **이미지 처리** | HTML5 Canvas API |
| **폰트** | IBM Plex Sans, IBM Plex Mono |
| **배포** | GitHub Pages |

## 📁 프로젝트 구조

```
ExifViewer/
├── index.html      # 메인 애플리케이션 (HTML/CSS/JS 통합)
├── README.md       # 프로젝트 문서
└── TECHNICAL.md    # 기술 상세 문서
```

## 🖼️ 지원 형식

| 형식 | 읽기 | 쓰기 |
|------|:----:|:----:|
| JPEG/JPG | ✅ | ✅ |
| PNG | ✅ | ✅ |
| WebP | ✅ | ✅ |
| TIFF | ✅ | ❌ |

## 🌐 브라우저 호환성

| 브라우저 | 지원 |
|----------|------|
| Chrome | ✅ |
| Firefox | ✅ |
| Safari | ✅ |
| Edge | ✅ |

## 📜 라이선스

MIT License - 자유롭게 사용, 수정, 배포 가능합니다.

## 🔗 관련 링크

- [exif-js Library](https://github.com/exif-js/exif-js)
- [Canvas API - MDN](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)
- [EXIF Specification](https://www.exif.org/Exif2-2.PDF)

---

Made with 🔒 for your privacy

