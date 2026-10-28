# Western Mainline 모델팩

[![Minecraft](https://img.shields.io/badge/Minecraft-1.7.10-62B47A.svg)](https://www.minecraft.net/)
[![RTM KaizPatchX](https://img.shields.io/badge/RTM_KaizPatchX-1.10.4-blue.svg)](https://github.com/Kai-Z-JP/KaizPatchX)
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.ko)

연합철도 서부간선 WM-160 전동차와 전차선 세트를 담은 RTM 모델팩입니다.

## 지원 환경
- Minecraft 1.7.10
- RealTrainMod KaizPatchX 1.10.4

## 설치
1. `ModelPack_WesternMainline_YYMMDD.zip`을 압축을 풀지 말고 `.minecraft/mods/`에 넣습니다.
2. 주행음을 들으려면 **pc28ksoundlib (revision)** 모델팩도 함께 설치해야 합니다.

## WM-160 전동차
| 편성 | 차량 |
|---|---|
| 4량 | `WM160_1` ~ `WM160_4` |
| 6량 | `WM160_6_1` ~ `WM160_6_6` |

- 1호차부터 순서대로, 모두 같은 방향으로 연결합니다.
- 최고속도는 160 km/h입니다.
- 행선: 표시 없음 / 임평 / 잠원 / 시운전 / 회송
- 기능 버튼 (편성 전체에 적용)
  - **고상홈 / 저상홈 취급**: 저상홈을 고르면 문이 열리기 전에 발판이 나옵니다.
  - **가선 7m / 가선 5.1m**: 팬터그래프가 올라가는 높이입니다.
  - **완행 / 급행**: 측면 행선안내기에 표시됩니다.

## 전차선 세트
열차가 다니는 선로 레일 위에 **서브 레일로 겹쳐서** 설치합니다. 선로의 곡선·높이·캔트를 그대로 따라갑니다.

| 이름 | 설명 |
|---|---|
| `WM_OHLE_Single_L` / `_R` | 단선. 기둥이 선로 왼쪽 / 오른쪽 |
| `WM_OHLE_Double_L` / `_R` | 복선. 두 선로 중 한쪽 레일에만 설치. `_L` = 이 레일이 왼쪽 선로, `_R` = 오른쪽 선로 (다른 선로는 4 m 옆) |

- 왼쪽/오른쪽은 레일을 깐 방향(시작 → 끝) 기준입니다. 반대 방향으로 깐 레일은 L/R을 바꿔 고르세요.
- 기둥은 레일 양 끝과 그 사이에 약 25 m마다 섭니다. 50 m 레일을 쓰는 것을 권장합니다.
- 복선은 레일 아이템의 Height에 3~10을 넣으면 그 값이 선로 중심에서 기둥까지 거리(m)가 됩니다. 기본값은 3 m입니다.
- 복선 곡선에서는 바깥쪽 기둥이 가동브래킷을 지지합니다.
- 분기기 레일에는 전차선이 그려지지 않습니다. 아래 와이어로 직접 이어 주세요.

## 와이어와 연결애자 (분기기 등 수동 가선)
| 이름 | 종류 | 설명 |
|---|---|---|
| `WM_OHLE_End` | 애자 (커넥터) | 투명 연결점 |
| `WM_OHLE_Catenary` | 와이어 | 전차선 + 조가선 + 드로퍼 |
| `WM_OHLE_Feeder` | 와이어 | 급전선 |

1. 전차선 세트가 끝나는 지지점의 가동브래킷 위치에 `WM_OHLE_End`를 놓습니다. 급전선은 급전선 끝 위치에 놓습니다.
2. 와이어 아이템으로 두 연결점을 차례로 우클릭합니다.

- `WM_OHLE_End`를 전차선 끝(또는 급전선 끝)에서 1칸 안에 놓으면 와이어가 그 끝에 정확히 붙습니다.
- RTM 기본 가선 규칙(연결점 = 조가선, 전차선은 0.8125 아래)을 따르므로, 다른 팩의 가동브래킷과도 이어 쓸 수 있습니다.
