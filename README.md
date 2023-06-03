# Personal packages repository

## Structure
```
root
├── pool
    ├── InRelease
    ├── Release
    ├── main
    |   └── Packages.gz
    └── durango
        └── Packages.gz
```

## Usage

```bash
curl -s --compressed "https://jsalvador.me/deb-packages/KEY.gpg" | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/jsalvador-packages.gpg > /dev/null
sudo curl -s --compressed -o /etc/apt/sources.list.d/jsalvador-packages.list "https://jsalvador.me/deb-packages/packages.list"
sudo apt update
```
