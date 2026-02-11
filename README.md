# MovieProjectWrapper

MovieProjectWrapper jest repozytorium nadrzędnym, które zawiera wszystkie submodule projektu:

- `MovieWorkspace` – workspace z kodem źródłowym i demoapp.
- `MovieNetworkDataProviderSPM` – paczka SPM z gotowym xcframework.
- `fastlane` – skrypty automatyzujące budowę frameworka i push do wrappera.

## Jak sklonować repozytorium

Repozytorium używa submodule, dlatego po klonowaniu należy użyć:

```bash
git clone --recurse-submodules git@github.com:ogrodowski-tomasz/MoviesProjectWrapper.git
```
lub jeśli repo zostało już sklonowane:

```bash
git submodule update --init --recursive
```

Struktura

fastlane/ – skrypty Fastlane do budowy i publikacji frameworka.

MovieWorkspace/ – repozytorium z kodem źródłowym i demo.

MovieNetworkDataProviderSPM/ – repozytorium z paczką SPM.

MovieProjectWrapper/ – nadrzędne repo, utrzymujące submodule i konfiguracje.

