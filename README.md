# Docker Compose - Apache
Projeto de criação de um container Apache em um servidor Ubuntu Linux usando Docker, Git e Apache

# ⚙️ Configurações
Para este arquivo YML criar um container corretamente é preciso realizar algumas configurações em seu servidor Linux:
* I. Instalar o Docker, Zip e Git com os comandos:
  
    ``` 
      apt-get update
      apt-get upgrade
      apt-get install docker
      apt-get install docker-compose
      apt-get install zip
      apt-get install git
   ```
    
* II. Agora precisamos clonar o projeto dentro do diretório /data/apache:
    * Crie o diretório /data/apache com:
      ``` mkdir /data/apache ```
      
    * Acesse o diretório e clone os arquivos do projeto:
      ``` git clone https://github.com/GuilhermeNSousa/Apache-Compose.git ```
      
    * Acesse o diretório Apache-Compose:
      ``` cd Apache-Compose ```
      
    * Mova os arquivos para o diretório anterior:
      ``` cp -r Site-Spotify/ .. ```

    * Executar o Docker Compose para criar o container e rodá-lo em background:
      ``` docker-compose up -d ```
    
# 🛠️ Acessando o projeto na web
Para Acessar o projeto na web basta digitar o ip do seu servidor e colocar a porta HTTP no link. Exemplo: "192.168.2.3:80"

# ✔️ Tecnologias utilizadas:
* Linux
* Docker
* Apache
* Git
