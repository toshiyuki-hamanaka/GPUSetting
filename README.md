# GPUSetting

リカバリディスクでリストア
端末立ち上げて
$ Python -V

# Default install
sudo apt-get update
sudo apt-get upgrade
sudo apt-get emacs
sudo apt-get install aptitude
apt-get install tetex-*
apt-get install texlive
apt-get install texlive-lang-cjk
apt-get install xdvik-ja
sudo apt-get install mecab libmecab-dev mecab-ipadic mecab-ipadic-utf8

# Install pyenv-virtual
sudo apt-get install -y make build-essential libssl-dev zlib1g-dev libbz2-dev wget curl llvm libncurses5-dev libncursesw5-dev libpng-dev
git clone https://github.com/yyuu/pyenv.git ~/.pyenv
git clone https://github.com/yyuu/pyenv-virtualenv.git ~/.pyenv/plugins/pyenv-virtualenv
echo -e "\n# `date '+%Y/%m/%d'` H.Seshime" >> ~/.bashrc
echo "## Setting pyenv, pyenv-virtualenv ##" >> ~/.bashrc
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bashrc 
echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bashrc 
echo 'eval "$(pyenv init -)"' >> ~/.bashrc
echo 'eval "$(pyenv virtualenv-init -)"' >> ~/.bashrc
source ~/.bashrc

# python virtual env.
pyenv install 3.6.2
pyenv virtualenv 3.6.2 py36
pyenv global py36
pyenv i
