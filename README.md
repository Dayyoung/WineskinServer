# Wineskin
Wineskin은 Microsoft Windows 소프트웨어를 macOS로 이식하는 데 사용되는 사용자 친화적인 도구입니다. OS X 10.6 부터 macOS 10.12 까지 (조정 없이) 작동했던 doh123의
원래 Wineskin 프로젝트 와 달리, 이 프로젝트는 macOS 10.15 부터 macOS 14 까지 지원합니다.

<br>

## Want to help support this project?
[![ko-fi](https://img.shields.io/badge/kofi-Donate-blue?style=for-the-badge&logo=ko-fi)](https://ko-fi.com/gcenx)
[![PayPal](https://img.shields.io/badge/PayPal-Donate-blue?style=for-the-badge&logo=paypal)](https://www.paypal.com/paypalme/gcenx)

<br>

## 설치 방법
### [homebrew](https://brew.sh/)
```
brew install --cask --no-quarantine gcenx/wine/wineskin
```

수동 설치 - ( 권장하지 않음! )
Wineskin Winery 다운로드
* 다운로드 후 추출 전 검역소를 제거하고, Keka를 사용하여 추출하지 마세요.
```
/usr/bin/xattr -drs com.apple.quarantine Wineskin.Winery.txz
```

<br>

## DirectX support

__WineD3D__\
DirectX 11 이하를 지원합니다.

OpenGL 백엔드는 DirectX 9 이하에서 사용됩니다.
Vulkan 백엔드는 DirectX 10 및 11에 사용되며
D3DMetal 엔진에서는 사용할 수 없습니다.

__D3DMetal__\
Metal을 통해 64Bit DirectX 11 및 12를 지원합니다.
"게임 포팅 툴킷" 1.0 베타 4 이후 Apple은 이제 상업적 용도가 아닌 재배포를 허용합니다. 여기에서
Apple 문서를 볼 수 있습니다.


__DXVK__\
Vulkan을 통해 DirectX 10 및 11을 지원합니다.
DXVK는 D3DMetal 엔진과 호환되지 않습니다.

__VKD3D__\
제한적 DirectX 12 지원.
WineCX23.x 이상의 엔진이 필요합니다.

<br>

## Hackintosh Support?
AMD 기반 시스템은 macOS에서 32Bit 코드를 실행할 수 없기 때문에 지원되지 않습니다.
Intel 기반 시스템은 문제 없이 작동해야 합니다.

<br>

# FAQ
내 바이러스 백신에서는 바이러스라고 합니다!!!
이를 오탐지로 보고하려면 안티바이러스/안티맬웨어 공급업체에 문의해야 합니다. 이는 와인이 PE 바이너리를 컴파일하기 위해 Mingw-gcc를
사용하게 되면서 시작되었습니다 .

다음 예를 참조하세요.

CrossOver 19 및 바이러스 백신 프로그램
Windows Defender는 Steam Proton 5.0 폴더에서 Occamy.c 트로이 목마를 탐지합니다.

<br>

## License
원본 자료와 동일하게 유지되는 LGPL 2.1이 해당 프로젝트의 라이센스입니다. 이에 대한 자세한 내용은 LICENSE 파일에서 확인할 수 있습니다.

<br>

## Credits
Wineskin 코드베이스 및 ObjectiveC_Extension 현대화를 위한 VitorMM .
지속적인 테스트 데이터와 버그 찾기를 위한 PaulTheTall .
Wineskin을 생성하기 위한 doh123입니다 .
이슈 템플릿, 문서 및 위키에 대해서는 thmrtz를 참조하세요 .
