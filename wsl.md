para instalar o wsl2 precisa verificar a versão do windows tem que ser acima do 10 versão: Build 19041.
com windows atualizado e com a instalação do windows terminal, pelo windows store, vamos usar o sequinte comando no powershell:

wsl --install -d nome_distro

wsl -l -o #mostra as distros disponiveis para serem instaladas.
wsl -l -v #mostra as distros ja instaladas

podemos alterar a distribuição padrao do nosso windows, usando o comando abaixo:
wsl -s <DistributionName> ou wsl --setdefault <DistributionName>

apos instalar uma distribuição atualize-a:
sudo apt update && sudo apt upgrade

configurando o seu ambiente wsl pode-se exportado, atraves de uma compactação da partição em formato tar 
 wsl --export <Distro> <FileName> ex: wsl --export Ubuntu ambiente1

 para importar o arquivo usamos o:
 wsl --import <Distro> <InstallLocation> <FileName>

 
 
