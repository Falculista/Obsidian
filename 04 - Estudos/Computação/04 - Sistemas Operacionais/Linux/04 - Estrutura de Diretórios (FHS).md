---
Title: Estrutura de Diretórios em Linux
Data: 2025-08-26
tags:
  - Linux
  - Sistemas_Operacionais
  - Computação
  - FHS
---
# O que é Estrutura de Diretórios
Os sistemas operacionais possuem pastas/diretórios padrões que já estão lá desde a criação do disco. No caso do Windows, quando baixamos algo no disco (normalmente C:) os arquivos são direcionados para pastas sem um padrão definido pelo próprio sistema, sendo que toda vez você deverá "reaprender" aonde está cada arquivo que você baixa. Agora, no caso de sistemas Unix-Like (como o Linux), eles usam uma padronização nessa estrutura chamado de FHS, que facilita diversas manipulações de arquivos.
# O FHS (Filesystem Hierarchy Standard)

![[Pasted image 20250826221133.png|center|600]]

Como vimos, o Linux (não todos, existem exceções como o GoboLinux), diferentemente do Windows, usa uma padronização de estrutura de diretórios chamada de FHS, que possui o objetivo de facilitar o uso do sistema com uma boa organização de diretórios. Os principais diretórios são:

- **_/_** ---> Barra/Raiz: é onde fica todo o nosso sistema (usuários, diretórios, subdiretórios, etc.)
- **_/proc_** ---> Processos: dentro da nossa diretório raiz (/), temos um diretório chamado de proc, onde estão localizados os processos da nossa máquina.
- **_/dev_** ---> Dispositivos: aqui está localizado todos os arquivos de dispositivos ligados na máquina, como é o caso de HD's externos, pendrives, etc.
- **_/boot_** ---> Kernel/initdr: todas as informações do Kernel ficam nessa pasta, como o GRUB e etc.
- **_/bin_** ---> Binários: aqui ficam os binários essenciais para o funcionamento do sistema, como os que mantém os códigos funcionando.
- **_/sbin_** ---> Binários adm: aqui ficam os binários também essenciais mas que só podem ser acessados pelo usuário root, pois são binários mais sensíveis usados na administração do sistema operacional.
- **_/lib_** ---> Bibliotecas: aqui ficam as bibliotecas que os binários acima utilizam.
- **_/etc_** ---> Configurações: aqui se localiza todas as informações a respeitos das configurações do sistema.
- **_/media_** ---> Removíveis: quando se conecta algum dispositivo no computador, o sistema não o reconhece até que seja montado, e o media justamente monta dispositivos removíveis automaticamente.
- **_/mnt_** ---> Temporário: similar ao media, o mnt serve como um ponto de montagem temporário para sistemas de arquivos. A única diferença deste para o media é que este é usado para montar manualmente os sistemas de arquivos (que podem ser mídias removíveis ou até partições de discos rígidos por exemplo).
-  **_/root_** ---> Usuário root: aqui fica todos os diretórios do usuário root, também chamado de super usuário, o qual pode realizar qualquer tipo de ação no sistema.
-  **_/home_** ---> Usuários: aqui ficam os diretórios de todos os usuários.
-  **_/tmp_** ---> Temporários: aqui ficam os arquivos temporários criados pelos aplicativos utilizados.
-  **_/var_** ---> Variável: aqui ficam armazenados os dados que mudam constantemente, como logs (registros de eventos). 
- **_/usr_**---> É aqui que ficam os executáveis e bibliotecas de todos os principais programas.
	- **_/usr/bin_** ---> Arquivos binários que não são necessárias pro funcionamento do sistema.
	- **_/usr/sbin_** ---> Arquivos binários administrativos, também não essenciais pro funcionamento do sistema.
	- **_/usr/lib_** ---> Aqui ficam as bibliotecas que dependem do sistema.
	- **_/usr/share_** ---> Aqui nesse diretório ficam os arquivos independentes da arquitetura do sistemas - sabemos que arquivos binários são executáveis que são feitos para tipos específicos de arquiteturas, como x86, ao contrário dos arquivos independentes, que funcionam em qualquer tipo de arquitetura. Segue exemplos abaixo:
		- **_/usr/share/doc_** ---> Aqui ficam as documentações de programas, e é claro que isso tinha de ser independente da arquitetura do sistema para funcionar.
		- **_/usr/share/man_** ---> Os manuais dos programas - a maioria dos programas tem, e precisa ser independente do sistema, claro.