# 🧃 juice-shop-ctf

Deploy OWASP Juice Shop in CTF mode for use with FBCTF, RootTheBox, or CTFd.

### Setup
```bash
mkdir -p /opt && cd /opt
sudo git clone https://github.com/juice-shop/juice-shop.git
sudo chown -R juice:juice /opt/juice-shop
cd /opt/juice-shop
```

### Install Node.js via NVM
```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash
. "$HOME/.nvm/nvm.sh"
nvm install 22
```

### Install Dependencies
```bash
npm install -g npm@11.6.2
npm install -g juice-shop-ctf-cli
export PATH="$PATH:$(npm prefix -g)/bin"
```
### Run CTF generator
```bash
juice-shop-ctf
```
### 📚 References

* [Node.js (Current Version)](https://nodejs.org/en/download/current)
* [OWASP Juice Shop CTF Mode Guide](https://help.owasp-juice.shop/part1/ctf.html)
* [juice-shop-ctf-cli (npm)](https://www.npmjs.com/package/juice-shop-ctf-cli)
* [OWASP Juice Shop (GitHub)](https://github.com/juice-shop/juice-shop)
* [Docker Post-install Steps for Linux](https://docs.docker.com/engine/install/linux-postinstall/)
