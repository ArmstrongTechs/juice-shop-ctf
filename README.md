# 🧃 juice-shop-ctf

Deploy OWASP Juice Shop in CTF mode for use with FBCTF, RootTheBox, or CTFd.

```bash
# Setup
mkdir -p /opt && cd /opt
sudo git clone https://github.com/juice-shop/juice-shop.git
sudo chown -R juice:juice /opt/juice-shop
cd /opt/juice-shop

# Install Node.js via NVM
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash
. "$HOME/.nvm/nvm.sh"
nvm install 22

# Install Dependencies
npm install -g npm@11.6.2
npm install -g juice-shop-ctf-cli
export PATH="$PATH:$(npm prefix -g)/bin"

# Run CTF generator
juice-shop-ctf
