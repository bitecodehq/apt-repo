# APT Repository

Debian and Ubuntu packages for Bitecode software, served at https://apt.bitecode.ltd.

## Usage

```bash
curl -fsSL https://apt.bitecode.ltd/pubkey.gpg | sudo gpg --dearmor -o /usr/share/keyrings/bitecode.gpg
echo "deb [signed-by=/usr/share/keyrings/bitecode.gpg] https://apt.bitecode.ltd stable main" | sudo tee /etc/apt/sources.list.d/bitecode.list
sudo apt update
sudo apt install zone
```

Packages are signed by `Bitecode Ltd (APT signing) <zone@bitecode.ltd>`, fingerprint `2865 757B 747B B1E8 1053  687D 96FB 1C31 AF1E D36C`.
