# DJform

C# Windows Forms 기반의 2덱 DJ 믹싱 프로그램입니다.

## 프로젝트 개요
- 개발 기간: 2026.08.10 ~ 2026.08.21
- 팀 프로젝트: 총 5명 (일부 역할 겸임)
- 최종현: 팀장 및 디제잉 폼 공동 개발 (3인)
- 역할 구성: 디제잉 폼 제작 3명, 데이터베이스 2명, 스트리밍 사이트 1명
- 최종현: 팀장 및 디제잉 폼 공동 개발

이 저장소에는 팀 프로젝트 중 디제잉 폼 소스가 포함되어 있습니다.
데이터베이스와 스트리밍 사이트 소스는 포함하지 않습니다.
아래 기능은 디제잉 폼 공동 개발 결과를 설명합니다.

## 주요 기능
- 좌우 덱에 MP3/WAV 불러오기, 개별 재생·일시정지·정지
- 덱별 볼륨과 크로스페이더를 통한 실시간 믹싱
- BPM 분석, 목표 BPM 조절 및 마스터 BPM에 맞추기
- 반음 단위 피치 조절
- Bass/Mid EQ와 저역·고역 통과 필터
- Stutter, Crush, Echo, Flanger 음향 효과
- 1/8박~32박 자동 루프
- 파형·재생 시간 표시와 턴테이블 드래그를 통한 재생 위치 제어
- 믹싱 결과 녹음 및 MP3 저장

## 개발 환경
- C#, .NET 6, Windows Forms, Visual Studio, GDI+
- NAudio 2.3.0 / SoundTouch.Net 2.3.2

## 실행 방법
Windows에서 .NET 6 SDK 및 Windows Forms 개발 환경을 준비하고
Visual Studio에서 DJform.sln을 열어 NuGet 패키지를 복원한 뒤 실행합니다.

```powershell
dotnet restore DJform.csproj
dotnet run --project DJform.csproj
```

사용할 음원은 실행 후 각 덱의 Music Load 버튼으로 선택합니다.
음원 파일, 빌드 결과물, 개인 IDE 설정은 저장소에서 제외했습니다.

## 검증 상태
소스와 이미지 리소스 참조를 확인했습니다. 현재 작업 환경에서
빌드 및 실제 오디오 재생 검증은 완료하지 못했습니다.

