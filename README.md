# CBRAND-Crawler 배포

CBRAND-Crawler 프로그램 배포 전용 저장소입니다. 소스 코드는 포함되어 있지 않습니다.

## 다운로드·설치
1. **[Releases](../../releases/latest)** → `CBRAND-Crawler.zip` 다운로드
2. 압축을 풀어 생긴 **`CBRAND-Crawler` 폴더**를 쓰기 권한이 있는 위치(예: 바탕화면, `D:\Tools`)에 둡니다.
   - `C:\Program Files`에 두면 자동 업데이트가 동작하지 않습니다.
3. 폴더 안의 `CBRAND-Crawler.exe` 실행
   - EXE만 따로 꺼내면 실행되지 않습니다. 바로가기는 EXE 우클릭 → **바로 가기 만들기**로 만드세요.

이후에는 프로그램의 **[⟳ 업데이트]** 버튼으로 최신 버전으로 자동 교체됩니다.

## 파일 설명
| 파일 | 용도 |
|---|---|
| `CBRAND-Crawler.zip` | 프로그램 (폴더형) |
| `CBRAND-Crawler.zip.sha256` | 무결성 확인용 해시 (업데이트 시 자동 검증) |
| `latest.json` | 업데이트 확인용 버전 정보 |
| `source-commit.txt` | 빌드 기록 |

## 수동 무결성 확인 (선택)
PowerShell:
```powershell
(Get-FileHash .\CBRAND-Crawler.zip -Algorithm SHA256).Hash.ToLower()
```
결과가 Release의 `.sha256` 파일 값과 같으면 정상 파일입니다.

## 처음 실행 시
서명되지 않은 프로그램이라 Windows SmartScreen 경고가 표시될 수 있습니다 → **추가 정보 → 실행**
