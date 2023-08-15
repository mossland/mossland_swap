# 모스랜드 스왑 시스템

모스랜드 스왑 시스템은 모스코인의 거래 수준을 높이기 위하여 루니버스(Luniverse) 네트워크와 이더리움 네트워크 간에 모스코인(MOC)을 교환하는 기능을 제공합니다. 이 기능을 통해 사용자는 두 네트워크 간에 MOC 토큰을 교환하거나 그 반대로 교환할 수 있습니다. 이 스왑 시스템은 다음의 토큰을 지원합니다:
- 루니버스 네트워크의 모스코인(MossCoin, MOC)
- 이더리움 네트워크의 랩트 모스코인(Wrapped MOC, WMOC)

모스랜드 스왑 시스템의 주요 목적은 모스코인의 거래 활성화를 위해 루니버스와 이더리움 네트워크 양쪽에서 사용할 수 있는 기능을 제공함으로써 확장시키는 것입니다. 이러한 네트워크 스왑 기능은 거래 효율성을 향상시키고 사용자들에게 MOC 토큰을 활용하는 더 많은 옵션을 제공하는 것을 목표로 합니다.

모스랜드 스왑 시스템의 목표는 루니버스와 이더리움 네트워크 간의 실시간 스왑 기능을 용이하게 만드는 것입니다. 이 기능은 두 네트워크 간의 간극을 줄여주며 사용자들이 MOC 토큰을 원활하게 변환할 수 있도록 돕는 역할을 합니다. 

- 스왑 시스템: [swap.moss.land](https://swap.moss.land)
- 공시 시스템: [disclosure.moss.land](https://disclosure.moss.land)
- MOC 락업 주소: [0xfb2b78e89be479318b62d94a93c3527ad8f4ff95](https://scan.luniverse.io/accounts/0xfb2b78e89be479318b62d94a93c3527ad8f4ff95)
- WMOC 락업 주소: [0xbee20b9df360b8442534ed8059f3e5baeeb74eaf](https://etherscan.io/token/0xBeE20B9Df360B8442534Ed8059f3e5bAEeB74EaF?a=0xbee20b9df360b8442534ed8059f3e5baeeb74eaf)

## 랩트 모스 코인 (WMOC) 소개

랩트 모스코인(Wrapped MOC, WMOC)은 모스코인(MossCoin, MOC)과 1:1 교환 가능한 이더리움 기반의 ERC-20 토큰입니다. 

- 컨트랙트 주소: [0xBeE20B9Df360B8442534Ed8059f3e5bAEeB74EaF](https://etherscan.io/token/0xBeE20B9Df360B8442534Ed8059f3e5bAEeB74EaF)
- 컨트랙트 소스 코드:
  - [Etherscan](https://etherscan.io/token/0xBeE20B9Df360B8442534Ed8059f3e5bAEeB74EaF#code)
  - [mossland_swap/mosscoin_swap.sol](mosscoin_swap.sol)

## 주요 특징

- **유동성 제공:** WMOC은 모스 코인을 이더리움 네트워크로 확장함으로써 두 네트워크 간의 유동성을 제공합니다.
- **이더리움 기반 활용:** WMOC은 ERC-20 토큰으로 이더리움 생태계에서 다양한 스마트 컨트랙트 및 서비스에 활용할 수 있습니다.
- **네트워크 스왑:** 루니버스 네트워크의 MOC을 WMOC로 교환하거나, 그 반대로 WMOC를 루니버스 네트워크의 MOC로 교환할 수 있습니다.
- **교환 비욜:** MOC와 WMOC 간의 스왑 비율은 1:1입니다. 다만, 스왑 실행 시 이더리움 네트워크의 트랜잭션 수수료를 사용자가 부담해야 합니다.

- 모스랜드 스왑 시스템 기대 효과:
  - 모스 코인의 거래 활성화 증대
  - 크로스 네트워크 호환성을 통한 사용자 기반 확장
  - MOC 토큰의 유동성 및 활용성 강화

- WMOC의 이더리움 네트워크에서 다양한 활용:
  - 탈중앙화 금융(DeFi) 프로젝트 참여
  - 스마트 컨트랙트 기반의 서비스 및 애플리케이션 구축
  - 이더리움 생태계 내의 다른 토큰과 교환 및 거래

## 스왑 과정

### 스왑 순서 설명
1. 사용자가 [모스랜드 스왑 웹사이트](https://swap.moss.land)에서 스왑 절차를 시작합니다.
2. 사용자가 루니버스 네트워크의 MOC을 이더리움 네트워크의 WMOC로 스왑 신청합니다.
3. 해당 양의 MOC이 루니버스 네트워크에서 잠금 처리됩니다.
4. 이에 상응하는 양의 WMOC이 이더리움 네트워크에서 사용자의 지갑으로 지급됩니다.
5. 스왑이 완료되면, 사용자는 WMOC을 이더리움 네트워크의 지갑에서 확인할 수 있습니다.

### 스왑 과정 상세 설명 문서
- [Wrapped MOC(WMOC) 스왑 준비하기 1](https://medium.com/mossland-blog/%EC%A4%80%EB%B9%841-wrapped-moc-wmoc-%EC%8A%A4%EC%99%91%EC%84%9C%EB%B9%84%EC%8A%A4-%EA%B0%80%EC%9D%B4%EB%93%9C-23f06666f2c4)
- [Wrapped MOC(WMOC) 스왑 준비하기 2](https://medium.com/mossland-blog/%EC%A4%80%EB%B9%842-wrapped-moc-wmoc-%EC%8A%A4%EC%99%91%EC%84%9C%EB%B9%84%EC%8A%A4-%EA%B0%80%EC%9D%B4%EB%93%9C-bcc1e8d9e850)
- [Wrapped MOC(WMOC) 스왑 준비하기 3](https://medium.com/mossland-blog/%EC%A4%80%EB%B9%843-wrapped-moc-wmoc-%EC%8A%A4%EC%99%91%EC%84%9C%EB%B9%84%EC%8A%A4-%EA%B0%80%EC%9D%B4%EB%93%9C-f353e57cc926)
- [Wrapped MOC(WMOC) 스왑 가이드 <데스크탑 편>](https://medium.com/mossland-blog/%EB%B3%B8%ED%8E%B8-wrapped-moc-wmoc-%EC%8A%A4%EC%99%91-%EC%84%9C%EB%B9%84%EC%8A%A4-%EA%B0%80%EC%9D%B4%EB%93%9C-2d6d20bc67e0)


## 보안 감사

2023년 8월 16일 현재, 외부 보안 감사가 진행 중입니다.

## 모스코인 유통량과의 관계



## 관련 링크

- [모스코인은 무슨 네트워크일까?](https://medium.com/mossland-blog/%EB%AA%A8%EC%8A%A4%EC%BD%94%EC%9D%B8%EC%9D%80-%EB%AC%B4%EC%8A%A8-%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC%EC%9D%BC%EA%B9%8C-8877360f0da9)
- [Wrapped MOC(WMOC) 탄생](https://medium.com/mossland-blog/wrapped-moc-wmoc-%ED%83%84%EC%83%9D-d76e36a60872)
- [모스코인 스왑 시스템](https://swap.moss.land)
- [모스코인 공시 시스템](https://disclosure.moss.land)

