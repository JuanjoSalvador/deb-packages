# Personal packages repository

## Usage

```bash
curl -s --compressed "https://jsalvador.me/packages/KEY.gpg" | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/jsalvador-packages.gpg > /dev/null
sudo curl -s --compressed -o /etc/apt/sources.list.d/jsalvador-packages.list "https://jsalvador.me/packages/packages.list"
sudo apt update
```