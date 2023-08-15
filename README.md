![header](https://user-images.githubusercontent.com/75381985/219609891-932a76c6-b85d-44d2-b5a9-82e5b0841ad2.jpg)

## AlwaysFine
**AlwaysFine**은 미세먼지와 초미세먼지 정보를 바탕 화면에 표시하는 [Rainmeter](https://www.rainmeter.net/) 스킨입니다. 대한민국 내 모든 측정소를 지원하며, 누구나 쉽고 빠르고 정확하게, 직관적으로 미세먼지와 초미세먼지 정보를 확인할 수 있습니다.

Windows 10 이상에서 작동하며, [한국환경공단 에어코리아 대기오염정보 오픈 API](https://www.data.go.kr/data/15073861/openapi.do) 키가 필요합니다.

[이전 버전\(4.x) 스킨 보기](https://github.com/Doiram/AlwaysFine/tree/08fc0554353d3b64ec0ebb01d77568ae9ac6dd05)

## 제작 동기
2022년 2학기, 학급에서 미세먼지 수치를 매일 측정하고 이를 칠판에 기록하는 역할을 담당했는데 그게 귀찮아서 만들었습니다. 사실 봉사 시간을 받아야 해서 이후에도 계속 칠판에 기록하긴 했지만.. 애플리케이션 개발이 귀찮기도 하고 빠르게 만들고 싶어서 Rainmeter를 사용했는데, 그냥 처음부터 네이티브 애플리케이션으로 만들 걸 그랬습니다.

## 기능
 * 대한민국 환경부, WHO 기준보다 엄격한 자체 기준 사용
 * 측정소 변경 및 저장 기능 지원
 * 깔끔하고 단순한 디자인 및 UI
 * 1시간 단위 자동 갱신
 * 자동 업데이트 지원

## 이용 범위
AlwaysFine은 GNU Lesser General Public License v2.1 라이선스로 배포됩니다. 자세한 내용은 [LICENSE](/LICENSE)를 참조하세요.

## 사용 방법
![1](https://github.com/Doiram/AlwaysFine/assets/75381985/91a61dbf-6e06-4dce-ae0b-9c8b024f7c93)

스킨을 실행하면 미세먼지, 초미세먼지의 수치가 나오고, 등급에 따라 이모티콘과 배경이 바뀝니다. 측정소는 송현 측정소(제물포고등학교와 가장 가까운 측정소)가 기본이며, 등급은 매우 좋음, 좋음, 양호, 보통, 나쁨, 매우 나쁨, 최악으로 총 7단계입니다.

![2](https://github.com/Doiram/AlwaysFine/assets/75381985/e81bc074-0a4f-485e-8301-3888dd93e164)

미세먼지와 초미세먼지 수치에 마우스를 올리면 해당 등급의 범위와 행동 지침을 볼 수 있습니다.

![3](https://github.com/Doiram/AlwaysFine/assets/75381985/851de94a-97f7-496f-ae4b-94f40d5c4a49)

설정 버튼을 누르면 설정 창이 나옵니다. 아무 곳이나 눌러 닫을 수 있으며, 입력창에 원하는 측정소의 이름을 입력한 후 엔터를 누르면 측정소가 변경됩니다. 변경한 측정소 정보는 계속 유지되며, 기본값은 송현입니다.

오른쪽에 있는 텍스트는 버전 정보입니다. 마우스를 올리면 자세한 내용을 확인할 수 있습니다. 자동 업데이트가 지원되기 때문에 특별한 문제가 없는 한 최신 버전으로 나오는 것이 일반적입니다.

측정소 목록과 깃허브 링크 버튼은 각각 미세먼지 측정소 목록과 현 깃허브 페이지로 연결되는 버튼입니다.

## 업데이트
 * 이전 업데이트 내역은 기록이 없어 기록하지 않았습니다.
 * 2023-05-08 4.0.3
     * 송림 측정소 가동 중단으로 송현 측정소로 변경
 * 2023-05-11 4.0.4
     * 업데이트 과정 중 생성되는 다운로드 폴더 삭제
 * 2023-05-12 4.0.5
     * 업데이트 스크립트를 인라인으로 실행하여 속도 향상, 업데이트 이후 무한 루프 발생하는 버그 수정
     * 폰트 기본 탑재 및 설치 후 스킨이 자동으로 로드되지 않는 버그 수정
 * 2023-08-11 5.0.0
     * 스킨 리팩토링 (불필요한 코드, 변수 정리 및 최적화, 약 Ln 600 > 400)
     * 업데이트 구조 변경으로 안정성 향상
        * 파일 다운로드 구조 변경
        * 파일 무결성 검증 진행
        * 호환성 문제로 요구 버전 윈도우 10으로 상향
        * 오류 방지를 위해 다시 시작 시 업데이트 반영
     * 스킨 디자인 및 폰트 변경
     * 변경한 측정소 정보가 저장되도록 변경
     * 스킨 로드 시 레이아웃 및 설정 자동 적용
     * 오픈 소스로 스킨 배포
     * 기존 8단계 등급에서 7단계로 변경 (심각 삭제)
 * 2023-08-12 5.1.0
     * 업데이트 스크립트 버그 수정
 * 2023-08-12 5.1.1
     * 레거시 스킨의 호환을 위해 버전 유지
 * 2023-08-12 5.1.2
     * 업데이트 스크립트 버그 수정
     * 미세먼지 측정 시간이 잘못 나오는 버그 수정
 * 2023-08-12 5.1.3
     * 버전 정보가 잘못 나오는 버그 수정
     * 버전 로드 실패 시 오류 메시지 출력
 * 2023-08-14 5.2.0
     * 더 효율적인 구조를 적용하여 불필요한 함수, 변수 정리
     * 코드 리팩토링, 최적화 진행
 * 2023-08-15 5.3.0
     * 코드 리팩토링, 최적화 진행
        * 기능이 중복되는 함수 통합
        * 불필요한 변수 삭제
        * 함수, 변수명 정리
        * 데이터 갱신 주기 처리 구조 변경
        * 그 외 유지보수를 위한 구조 변경
        * 불필요한 속성값을 제거하여 최적화
     * 가독성을 위해 고정폭 폰트(Pretendard GOV)로 변경
     * 미세먼지 등급의 글자 수가 다른 경우 간격을 조정하여 가독성 향상
     * 측정소 한 곳이 점검 중이어도 말풍선에 다른 측정소 정보가 나오게 변경
     * 인터넷 문제 혹은 잘못된 측정소 입력 시 상황에 따라 적절한 문구가 나오게 변경
     * 설정 창 페이드 인, 아웃 효과 적용
     * 설정 창의 배경이 실시간으로 변경되지 않던 문제 해결

## 기타
 * Rainmeter는 HiDPI를 지원하지 않아 일부 환경에서 설치 후 스킨이 흐릿하게 나옵니다. 이를 해결하려면 Rainmeter가 설치된 폴더(Program Files/Rainmeter)에서 Rainmeter.exe 우클릭 후 차례대로 "호환성", "높은 DPI 설정 변경"을 누른 뒤, "높은 DPI 조정 동작을 재정의합니다."를 활성화하세요.