~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Instalando SSH no Ubuntu 20.04 LTS
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


Você pode instalar o openSSH no Ubuntu, Linux Mint, Debian e derivados. Portanto, os comandos e os procedimentos são os mesmos. Se você não está familiarizado com o SSH é importante lembrar que as configurações são realizadas pelo Terminal. Então, o primeiro passo é a instalação, para instalar abra o Terminal e cole os comandos abaixo:

 - sudo apt-get install openssh-server

Agora, vamos ativar o serviço. Lembre-se que nestes comandos estamos usando o sudo. No entanto, em distribuições baseadas puramente no Debian, o sudo não vem habilitado. Assim, você pode realizar a instalação do SSH usando o ROOT. Mais uma vez, para ativar o SSH execute o comando abaixo:

- sudo service ssh status
