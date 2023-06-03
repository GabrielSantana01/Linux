# Linux
ocorreu uma pequena mudança na estrutura do estudo. e agora iremos aprender linux para uso dentro da AWS. porem usando o WSL vamos criar todas a estrutura no vscode no windows e assim teremos o terraform e ansible para nos auxiliar.

-- acredito que essa parte abaixo não perdeu a importancia...
usamos( su ) para virar adm e colocamos a senha.
-- aqui é informado que a melhor maneira de instalar algo no linux é acessando o site do fabricante e instalando a versão pretendida. pois usando o sudo vamos instalar
somente a versão disponivel padrão. tenho que ver como vai ser feito usando o wsl e vscode.
-- não vamos instalar o vscode dentro do linux. mas iremos usar uma estrutura de pastas pelo wsl. e arquivos .py com isso devemos aprender os comandos linux para criar um ambiente de desenvolvimento python.

a melhor estrutura encontrada no momento foi instalar o windows terminal pelo windows store, acessar o wsl pelo WT. e la instalar um shell conhecido como zsh(z shell)
ele é responsavel por ter mais opções e temas coloridos. 
atraves desse shell podemos chamar o vscode digitando code no zsh.
esse terminal tb esta disponivel pelo vscode. nosso objetivo inicial é criar um ambiente virtual e o pip.

-- no inicio não estava conseguindo instalar o python.. ai mandei essa sequencia de comando:
sudo apt-get install software-properties-common
sudo apt-add-repository universe
sudo apt-get update
sudo apt-get install python3-pip

--------------------------------------------------------------------------------------------
https://www.alura.com.br/artigos/oh-my-zsh-melhorando-produtividade-terminal?gclid=CjwKCAjwscGjBhAXEiwAswQqNMEt90Y2oiFBJC3I-i1K2NxL52NmTvuNnnK7013uBBDhVgxa7YlAThoCkuEQAvD_BwE

istalar o zsh: sudo apt-get install zsh 
colocar o zsh como shell padrão: chsh -s $(which zsh)
instalar o ohMyZsh(os temas):sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
corretor de comando do zsh:git clone https://github.com/zsh-users/zsh-autosuggestions \$ZSH_CUSTOM/plugins/zsh-autosuggestions
autocompleta do comando: git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
perquisa arquivo pelo terminal: git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf && ~/.fzf/install

para configura o zsh: usando o editor nano do linux. sudo nano ~/.zshrc
existe um atalho que abre o zsh em outro editor linux:zshconfig "mate ~/.zshrc"
temas: https://github.com/ohmyzsh/ohmyzsh/wiki/Themes
para carregar uma nova versao do terminal: source ~/.zshrc

----------------------------------------------------------------------
instalar o venv: sudo apt install python3-venv
criar ambiente virtual: python3 -m venv ambienteVirtual
----------------------------------------------------------------------
para instalar o pandas no unbuntu:
sudo apt install python3-pandas



em seguida instalaremos o pip:

sudo apt-get install python3-pip

instalando o git: sudo apt-get install git
intalando o pylint: sudo pip3 install pylint
