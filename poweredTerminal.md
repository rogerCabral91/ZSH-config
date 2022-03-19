# Tutorial de configuração do terminal

### 1º Instalar [ZSH](https://www.zsh.org/)

`sudo apt-get install zsh`

### 2º Instalar [Oh My ZSH](https://ohmyz.sh/)

- via curl \
  `sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

- via wget \
  `sh -c "$(wget https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"`

### 3º Instalação de NerdFonts

Para melhor desempenho dos temas do ZSH e Oh My ZSH é preciso usar uma Nerd Font, para saber um pouco mais pode olhar esse [vídeo](https://youtu.be/w9wqIEk5Cqo).

Eu costumo usar a [FiraCode](https://github.com/tonsky/FiraCode/releases).

Depois de instalar a fonte é preciso ir no terminal e configurar ele para usar a fonte. Para isso temos que ir em: \
 Editar > Preferências > Aba: Texto > Checkbox: Fonte Personalizada e escolher a fonte. \
![Passo a Passo](/.github/configFont.gif)

### 4º Instalação de um tema

Eu geralmente uso o tema [Spaceship](https://github.com/spaceship-prompt/spaceship-prompt).
* Para instalar primeiro é preciso clonar o repositório: \
`git clone https://github.com/spaceship-prompt/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt" --depth=1`

* Depois precisamos criar um Symlink `spaceship.zsh-theme`: \
`ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"`

* Depois precisamos abrir o arquivo `.zshrc` com algum editor de texto, o Nano por exemplo: \
`sudo nano ~/.zshrc`

* E mudar a configuração para: \
`ZSH_THEME="spaceship"`

### 5º Instalação do [Zinit](https://github.com/zdharma-continuum/zinit)

O Zdharma é o plugin que vai dar o auto-complete e outras funções de produtividades \
`sh -c "$(curl -fsSL https://git.io/zinit-install)"`

### 6º Link do Gist que tem a configuração do meu arquivo .zshrc

[.zshrc](https://gist.github.com/rogerCabral91/b65aa309594eca92d96cf29dcd941aaf)