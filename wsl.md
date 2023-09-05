para instalar o wsl2 precisa verificar a versão do windows tem que ser acima do 10 versão: Build 19041.
com windows atualizado e com a instalação do windows terminal, pelo windows store, vamos usar o sequinte comando no powershell:

wsl --install -d nome_distro

wsl -l -o #mostra as distros disponiveis para serem instaladas.
wsl -l -v #mostra as distros ja instaladas
apos instalar uma distribuição atualize-a:
sudo apt update && sudo apt upgrade
