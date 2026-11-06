# EasyDoPhoto

카메라 · 앨범 · 사진 편집을 잇는 오프라인 안드로이드 앱. 앱을 켜면 바로 카메라가 나오고, 사진은 기기 안에서만 처리함. EasyDo 시리즈.

## 다운로드

최신 버전 0.2.4 — [Releases](https://github.com/parkrye/AppProject_EasyDoPhoto/releases)에서 `EasyDoPhoto-<버전>.apk`를 받아 설치. Android 11 이상.

- 처음 설치 시 "출처를 알 수 없는 앱" 설치 허용 필요. Play 프로텍트가 검사 화면을 띄울 수 있음
- 업데이트는 새 APK를 같은 방식으로 덮어 설치. 설정 · 내 프리셋 유지
- 앱 안 업데이트 알림 없음. `설정 → 앱 정보 → 새 버전 받기`에서 직접 확인
- 서명 인증서 SHA-256: `acb218cf6b835dffa90e847c8b74dd71faaeeecfdbe0d130cdbe460dc1c4ed82`
  (`apksigner verify --print-certs EasyDoPhoto-<버전>.apk`로 확인)

## 기능

| 도구 | 내용 |
|---|---|
| 카메라 | 촬영 프리셋 16종 실시간 미리보기, 화각 · 촬영 각도 · 렌즈 효과 포함 세부 조절 후 내 프리셋으로 저장, 촬영 처리(자동 보정 · HDR · 야간, 기기 지원 시) · 화질(최고 · 높음 · 보통) · 플래시 · 타이머 · 비율 · 격자 · 확대 · 초점 · 밝기, QR 모드(QR 코드 읽기 · 웹 링크 열기 · 복사) |
| 앨범 | 전체 사진 날짜별 격자, 폴더별 보기, 여러 장 선택 · 공유 · 삭제, 사진 확대 · 정보 · 편집 |
| 회전 · 반전 | 좌우 · 상하 반전, 90도 회전, ±45° 0.1도 단위 회전, 상하 · 좌우 기울기, 가로 · 세로 기울임 |
| 자르기 | 자유 · 고정 비율 |
| 크기 | 픽셀 지정 · 비율 |
| 조정 | 밝기 · 색 · 효과 묶음 탭. 노출 · 밝기 · 대비 · 하이라이트 · 그림자 · 색온도 · 색조 · 채도 · 생동감 · 페이드 · 선명도 · 흐림 · 비네트 · 도트 · 포스터화 · 하프톤 |
| 필터 | 흑백 · 세피아 · 빈티지 · 도트 · 포스터 · 하프톤 등 13종, 강도 조절 |
| 그리기 | 펜 · 마커 · 붓 · 모자이크 · 직선 · 화살표 · 사각형 · 타원 · 글자 · 채우기 · 스포이트 |
| 지우기 | 투명하게 지우는 지우개 · 되살리기 · 비슷한 색 · 올가미 |
| 설정 | 촬영 · 앨범 · 편집 옵션, 설정과 내 프리셋 `백업 만들기` · `백업에서 복원`, `앱 정보` · `새 버전 받기` · `오픈소스 라이선스` |

화면은 카메라 앱 특성상 어두운 고정 테마.

### 알려진 점

- Galaxy S24+에서만 시험함
- 필터를 켠 미리보기는 저장되는 사진과 색이 조금 다를 수 있음. 해상도도 낮아질 수 있으나 저장 사진에는 영향 없음
- 프리셋 값은 시작값으로, 실제 사진으로 충분히 다듬지 않음
- 필터는 저장 결과에 그대로 적용되며 원본을 따로 남기지 않음
- 2400만 화소가 넘는 사진은 편집할 때 줄여서 열림

버그 · 제안은 [Issues](https://github.com/parkrye/AppProject_EasyDoPhoto/issues)에.

## 개인정보

인터넷 권한 없음 · 광고 없음 · 수집 · 전송 없음.

- 사진은 기기 안에서만 처리. 저장하는 사진에 EXIF · 위치 정보를 넣지 않음(촬영 사진은 방향 정보만)
- 권한은 카메라(촬영)와 사진 읽기(앨범)만 사용. 사진 권한을 거부하면 앱이 저장한 사진만 보임
- 사진 삭제는 항상 시스템 확인 창을 거침
- 설정과 내 프리셋은 기기 안에만 저장. 앱 안 백업(`easydophoto-backup-yyyy-MM-dd.json`)으로 보관

## EasyDo 시리즈

| 앱 | 용도 | 플랫폼 |
|---|---|---|
| [EasyDoDraw](https://github.com/parkrye/MultiProject_EasyDoDraw) | 그림 · 애니메이션 | Android · Windows |
| [EasyDoWrite](https://github.com/parkrye/AppProject_EasyDoWrite) | 소설 · 글쓰기 | Android |
| [EasyDoRead](https://github.com/parkrye/AppProject_EasyDoRead) | 책 · 문서 읽기 | Android |
| [EasyDoShelve](https://github.com/parkrye/AppProject_EasyDoShelve) | 웹 소설 서재 | Android |
| [EasyDoPhoto](https://github.com/parkrye/AppProject_EasyDoPhoto) | 카메라 · 사진 편집 | Android |
| [EasyDoDiet](https://github.com/parkrye/AppProject_EasyDoDiet) | 식단 · 운동 기록 | Android |
| [EasyDoZip](https://github.com/parkrye/AppProject_EasyDoZip) | 파일 · 압축 관리 | Android |
| [EasyDoGame](https://github.com/parkrye/AppProject_EasyDoGame) | 미니 게임 모음 | Android |
| [EasyDoMix](https://github.com/parkrye/AppProject_EasyDoMix) | 영상 · 오디오 편집 | Android |
| [EasyDoRecord](https://github.com/parkrye/AppProject_EasyDoRecord) | 녹음 | Android |
| [EasyDoStudio](https://github.com/parkrye/DesktopProject_EasyDoStudio) | 화면 녹화 · 영상 편집 | Windows |
| [EasyDoMusic](https://github.com/parkrye/MultiProject_EasyDoMusic) | MIDI 연주 · 작곡 | Android · Windows |

## 라이선스

MIT License · © parkrye. 포함된 서드파티 라이브러리 라이선스는 앱 안 `설정 → 앱 정보 → 오픈소스 라이선스`에서 확인.
