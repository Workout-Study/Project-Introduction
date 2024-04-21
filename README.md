# FITMATE [Android Application]
![initial](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Ffitmate_mainphoto.png?alt=media&token=fd41b4b0-303c-4047-8c43-8ce09acf75ee)
- 당신의 건강 여정을 위한 동료를 만나보세요. 운동은 우리 모두의 약속 입니다.
- FITMATE의 투표는 더 큰 목표를 위한 약속입니다. 벌금을 통한 페널티는 운동을 위한 감시의 끈 입니다.
- 운동을 하지 않으면 여러분의 지갑이 가벼워질거에요!



## Application Demonstration Video

해당 이미지를 클릭 시 영상으로 이동합니다.

[![FITMATE Demo Video](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Fyoutube_screenshot.png?alt=media&token=e047ec98-4205-431b-9ec9-8d1b666586ed)](https://www.youtube.com/watch?v=hU05MZoTvVI)



## Team FITMATE

| 팀원   | 역할         | 작업 내용                                       | GitHub Link                                   |
| ------ | ------------ | :---------------------------------------------- | --------------------------------------------- |
| 김성호 | 기획, 백엔드 | 실시간 단체 채팅                                | [kimsunfang](https://github.com/kimsunfang)   |
| 정정일 | 백엔드       | 운동 인증, 그룹 관리                            | [12OneTwo12](https://github.com/12OneTwo12)   |
| 박찬규 | 백엔드       | 로그인, 사용자 정보 관리                        | [chan0966](https://github.com/chan0966)       |
| 서경원 | 안드로이드   | 모듈 설계, 디자인, 채팅, 로그인, 통신           | [woojugoing](https://github.com/woojugoing)   |
| 강현구 | 안드로이드   | 아키텍처 설계, 디자인, 인증, 운동기록 정보 관리 | [Ganghyungoo](https://github.com/Ganghyungoo) |



## Project Planning

#### 1. 기획 의도

- "벌금을 전제로 하여 진행하는 운동 소모임" 이라는 행위를 대표적인 SNS 플랫폼인 **카카오톡**을 통하여 진행하고 있었음.
- 해당 모임을 지속적으로 진행하던 중, 추가적으로 있었으면 좋겠다고 생각한 기능들과 **채팅**, **기록** 에 중점을 두어 애플리케이션을 제작하게 되었음.



#### 2. 세부 기획 설계

##### [1] 운동 인증 방식

- 인증은 누가봐도 완벽하게 운동을 했다고 생각할 수 있는 방식을 채용해야 함.

- 디테일 하면서도 정확한 방식을 채용하기 위하여 신중하고 정확한 방식을 선택해야 함.
- **Application 내부에 운동 시간 타이머, 시작과 끝에 사진을 받아와서 저장하여 기록하는 방식 채택**
- **사용자가 해당 기록 인증 시, 다른 그룹 내의 사용자들이 투표를 하여 해당 운동에 대한 공정성 처리**

##### [2] 벌금 제도

- 적당한 선의 금액으로 벌금을 책정해야 제도를 무시하는 사람에 대한 대처가 가능함.
- **버전 1.0.0 에서는 개발의 용이성 및 확정성을 위해서 5,000 원으로 고정**
- **추후 업데이트를 통해서 5,000 원과 50,000 원의 범위로 그룹 내 리더가 설정 가능하게 변경 할 예정**

##### [3] 벌금에 대한 금전거래 방식

- 사업자 등록이 되기 전에는 결제 시스템이 사용 불가하여 제한적인 사항에서 결정해야 함.
- **FitLeader 가 모임 개설 시 계좌 인증을 통하여 등록 후 Clipboard 복사 후 송금하는 방식**
- 금전 거래에 대하여 1차적인 책임은 해당 FitMate에 있는 것을 전제 하에 진행 할 예정
- 1차적 책임은 지지 않으나, 법적 문제가 발생하였을 경우 채팅 내역과 계좌 정보 등은 제공해 주는 것으로 예정



## Service Architecture

![service_architecture](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Farchitecture_2.png?alt=media&token=1deda73c-d54a-4d2c-a18f-076bbb049a92)



## Event Sourcing Architecture

![architecture_2](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Farchitecture_1.png?alt=media&token=79dc6259-7126-42c6-abae-eb491328bf99)

## Application Screen

|                       스플래시 스크린                        |                        온보딩화면 - 1                        |                        온보딩화면 - 2                        |                        온보딩화면 - 3                        |                        권한 요구 화면                        |
| :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| ![splash](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Fsplash.png?alt=media&token=18d5ed5d-0fce-4d2f-810c-7c9e7654eddd) | ![onboarding_1](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Fonboard_1.png?alt=media&token=617f0fd9-61d2-43ff-a689-76eba8a5b836) | ![onboarding_2](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Fonboard_2.png?alt=media&token=890e2fbc-9b66-476d-84a0-d0cd17d7f0a4) | ![onboarding_3](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Fonboard_3.png?alt=media&token=89106848-baf7-4e1a-8440-510af561b68c) | ![permission](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Fpermission.png?alt=media&token=06430974-ed9c-4ae5-bcb1-80b184a5ad4d) |

|                         로그인 화면                          |                       닉네임 설정 화면                       |                          메인 화면                           |                        그룹 열람 화면                        |                      그룹 상세정보 화면                      |
| :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| ![login_main](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Flogin_main.png?alt=media&token=1834a867-6ec4-4d6d-9cb1-11f3585d52f7) | ![login_nickname](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Flogin_nickname.png?alt=media&token=a536cd3d-a4aa-4bba-9263-ec8cf49e6b70) | ![home_main](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Fhome_main.png?alt=media&token=fa6bba79-ad51-4f12-a870-3e27a0ec1bb8) | ![home_category](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Fhome_category.png?alt=media&token=be304be0-f000-4e5b-9dc1-e399c7ae3784) | ![home_group](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Fhome_group.png?alt=media&token=adfae553-1775-4585-8402-c4b62e2834cd) |

|                      내 운동 정보 화면                       |                        운동 기록 화면                        |                        채팅 목록 화면                        |                        채팅 내부 화면                        |                  채팅 드로어 레이아웃 화면                   |
| :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| ![fit_main](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Ffit_main.png?alt=media&token=52fcd78f-eb4b-4642-9773-e84abcbb8fc6) | ![fit_certificate](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Ffit_certificate.png?alt=media&token=93975774-8302-4f27-b5f2-8fe64203aebd) | ![chat_group](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Fchat_group.png?alt=media&token=d8f32b8f-a951-4294-b495-99490ff753d1) | ![chat_main](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Fchat_main.png?alt=media&token=9d7ebe4a-b827-41f7-b57d-5680ddf6c3ab) | ![chat_drawer](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Fchat_drawer.png?alt=media&token=4b2ed25e-f3ef-49d3-9282-fbb95c7f7a4d) |

|                       그룹 진척도 화면                       |                     그룹 투표 현황 화면                      |                     그룹 벌금 내역 화면                      |                         내 정보 화면                         |                      오픈소스 고지 화면                      |
| :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
| ![chat_progress](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Fchat_progress.png?alt=media&token=a2a25c35-d41a-4ba6-a825-869a9c63ff9f) | ![chat_vote](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Fchat_vote.png?alt=media&token=302ae983-62a3-4db7-b1be-67e0f45748cf) | ![chat_fine](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Fchat_fine.png?alt=media&token=da5ecf3e-d7bc-4843-a3bc-de0a0528e843) | ![mypage_main](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Fmypage_main.png?alt=media&token=62397221-cc06-466b-9eae-1bbe21e08b01) | ![mypage_license](https://firebasestorage.googleapis.com/v0/b/fitmate-e2b03.appspot.com/o/fitmate_images%2Fmypage_license.png?alt=media&token=c229444c-fdfc-4ae9-9ce6-e2d48c13b6c6) |



## 
(https://www.youtube.com/watch?v=hU05MZoTvVI)
