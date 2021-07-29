~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Instalando SSH no Ubuntu 20.04 LTS
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


Você pode instalar o openSSH no Ubuntu, Linux Mint, Debian e derivados. Portanto, os comandos e os procedimentos são os mesmos. Se você não está familiarizado com o SSH é importante lembrar que as configurações são realizadas pelo Terminal. Então, o primeiro passo é a instalação, para instalar abra o Terminal e cole os comandos abaixo:

 - sudo apt-get install openssh-server

Agora, vamos ativar o serviço. Lembre-se que nestes comandos estamos usando o sudo. No entanto, em distribuições baseadas puramente no Debian, o sudo não vem habilitado. Assim, você pode realizar a instalação do SSH usando o ROOT. Mais uma vez, para ativar o SSH execute o comando abaixo:

- sudo service ssh status

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Configurações do SSH
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Por padrão você já está com serviço do SSH ativo, mas se por algum motivo você queira alterar as configurações padrão, é possível sim. Porém, saiba o que está fazendo. Para alterar as configurações do SSH execute o comando abaixo, utilizando o editor de sua preferência:

- sudo nano /etc/ssh/sshd_config

E após fazer as alterações é necessário reiniciar o serviço para que as alterações entrem em vigor. Para isso, execute o comando abaixo:

sudo service ssh restart

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Acessando via SSH o Ubuntu
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Agora que já passamos pelo o processo de instalação do SSH no Ubuntu, Debian e derivados, vamos promover o acesso remoto.
A sintaxe do SSH é muito simples, confira:

- ssh usuario@ip-alvo

Perceba que você precisa inserir o nome do usuário e o IP remoto, ou seja, da máquina que você quer acessar. É importante ter o SSH instalado e ativado na outra máquina, ou não vai funcionar. Por padrão a porta do SSH é a 22, mas algumas pessoas alteram a porta e neste caso é preciso informar a porta correta ou não vai funcionar.
A sintaxe do SSH informando a porta destino é:

- ssh usuario@ip-alvo -p numero da porta
