# 2023년 객체지향 소프트웨어공학 3팀 - 기장군 공영자전거 대여 시스템

## 사용 기술 스택
| 프론트엔드 | 백엔드 | DB |
| -- | -- | -- |
| ![logo-og](https://github.com/KIT-OOSE-23-3team/.github/assets/102248077/6ed92d5f-35dd-4790-adba-5730e7103e8e) | ![thumb](https://github.com/KIT-OOSE-23-3team/.github/assets/102248077/b586cf03-c74d-4d0d-96f7-442068d4881e) | ![1024px-MySQL ff87215b43fd7292af172e2a5d9b844217262571](https://github.com/winteeeee/CreativeProject/assets/102248077/fa1f0082-dbda-44a8-a864-c01043e0332e) |

## 팀 구성
| 인원 | 역할 |
| -- | -- |
| 한성민(구현 팀장) | 전체 시스템 총괄 책임자 |
| 이상헌 | 회원관리, 대여관리 프론트엔드 담당 |
| 김정민 | 운영관리 프론트엔드 담당 |
| 구정훈 | 공지관리 프론트엔드 담당 |
| 이성준 | 이력관리 프론트엔드 담당 |

## 1. 개요
설계 단계에서 작성한 (SDD)에 따라 아래 기준을 준수하여 구현을 실시한다.
* 구현 범위는 지정된 구현범위를 참고한다.
* 구현 환경은 SDD와 PMP에 제시된 내용과 동일해야 한다.
* 구현 기간은 종료보고회 이전에 마쳐야 한다.

구현 팀장은 구현 범위를 취합하고 팀원들의 진도 점검을 1주일 단위로 실시하여 구현진도표를 작성하여 제출한다.

## 2. 구현대상 유스케이스
| 서브시스템 | 구현대상 유스케이스 |
| -- | -- |
| 회원관리 | 회원가입, 회원 개인정보 조회 |
| 대여관리 | 자전거 대여, 자전거 이용 이력 조회(본인) |
| 이력관리 | 결제/환불 이력 조회, 가입자 및 기간별 이용 내역 조회 |
| 공지관리 | 공지사항 등록 / 조회 |
| 운영관리 | 자전거 / 대여소 등록 |

## 3. ERD
![화면 캡처 2023-06-02 203709](https://github.com/KIT-OOSE-23-3team/.github/assets/102248077/dd5a6d93-9f7d-4708-9f2c-6f892ab4eeb0)

## 4. 서브시스템 별 클래스 명세(SDD 기준)
### 4-1. 회원관리
| 바운더리 | 컨트롤 | 엔티티 |
| -- | -- | -- |
| UserHompage | MemberRegistrationControl | Memeber |
| MemberScreen | MemberControl |

### 4-2. 대여관리
| 바운더리 | 컨트롤 | 엔티티 |
| -- | -- | -- |
| RentalBoundary | RentalOfficeStateControl |
| RentalOfficeStateBoundary | RentalControl |
| ShortcutUI |

### 4-3. 이력관리
| 바운더리 | 컨트롤 | 엔티티 |
| -- | -- | -- |
| PaymentDetailBoundary | PaymentDetailControl | PaymentDetail |
| HistoryCheckScreen | HistoryCheckControl | HistoryCheck |

### 4-4. 공지관리
| 바운더리 | 컨트롤 | 엔티티 |
| -- | -- | -- |
| ManagerSupportFormpage | ManagerSupportControl | Post |
| CustomerSupportLookUpPage | CustomerSupportControl | |
| StastisticsManagerPage | StastisticsManagerControl | |
| KakaoTalkComposePage | KakaoTalkMessageControl | |

### 4-5. 운영관리
| 바운더리 | 컨트롤 | 엔티티 |
| -- | -- | -- |
| BicycleManagementScreen | BicycleControl | Bicycle |
| RentalOfficeManagementScreen | RentalOfficeControl | RentalOffice |


