# beomzh/homebrew-tap

[PolyMac](https://github.com/beomzh/PolyMac)을 Homebrew로 설치하는 개인 저장소입니다.

```bash
brew tap beomzh/tap
```

```bash
brew trust --cask beomzh/tap/polymac
```

```bash
brew install --cask beomzh/tap/polymac
```

Homebrew 7부터는 공식 저장소가 아닌 cask를 쓰기 전에 `brew trust`로 한 번 믿는다고 등록해야 합니다 (`~/.homebrew/trust.json`에 이 cask 하나만 들어갑니다).

PolyMac은 Apple 공증을 받지 않고 자체 인증서로 서명해, 그냥 받으면 macOS가 "손상됨"으로 막습니다. 이 cask는 설치한 앱의 다운로드 표시(quarantine)를 지워 바로 열리게 합니다. ([자세히](https://github.com/beomzh/PolyMac/blob/main/docs/SECURITY.md))

업데이트: `brew upgrade --cask polymac`, 또는 앱의 메뉴바 아이콘 › 업데이트 확인…

cask 원본은 PolyMac 저장소의 `packaging/homebrew/polymac.rb`에 있고, 릴리즈할 때 여기로 옮깁니다.
