# CBRAND-Crawler 배포

CBRAND-Crawler 실행 파일(EXE) 배포 전용 저장소입니다. 소스 코드는 포함되어 있지 않습니다.

## 다운로드
**[Releases](../../releases/latest)** → `CBRAND-Crawler.exe`

- 프로그램의 **[⟳ 업데이트]** 버튼을 누르면 이 저장소의 최신 버전으로 자동 교체됩니다.
- 각 Release에는 무결성 확인용 `CBRAND-Crawler.exe.sha256` 파일이 함께 있으며, 업데이트 시 자동으로 검증합니다.

## 수동 무결성 확인 (선택)
PowerShell:
```powershell
(Get-FileHash .\CBRAND-Crawler.exe -Algorithm SHA256).Hash.ToLower()
```
결과가 Release의 `.sha256` 파일 값과 같으면 정상 파일입니다.

## 처음 실행 시
- 서명되지 않은 프로그램이라 Windows SmartScreen 경고가 표시될 수 있습니다 → **추가 정보 → 실행**
- EXE는 쓰기 권한이 있는 폴더(예: 바탕화면, `D:\Tools`)에 두세요. (`C:\Program Files`에서는 자동 업데이트 불가)
