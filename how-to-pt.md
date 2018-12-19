##############################################

01 -------------------------------------------

  baixe o arquivo *IntelliJ-IDEA-$VERSION.tar*.gz no site
  
02--------------------------------------------

  abra o terminal (ou precione ctrl+Alt+T)
  e vá até a pasta /opt/  com o seguinte código:
  
    $ cd /opt/
    
03--------------------------------------------

  extraia o arquivo baixado, digitando o código:
  
    $ sudo tar -xvzf ~/Downloads/idea-$VERSION_BUILD.tar.gz
  
  // substitua "idea-$VERSION_BUILD.tar.gz" pelo nome correto
  // de seu arquivo baixado
  
04--------------------------------------------

  // nessa etapa você pode fazer de duas formas.
  // manualmente, ou pelo terminal, você escolha
  // como achar melhor
  
  04.1------------------ manual -------------
  
    abra sua pasta local e crie um novo arquivo de nome:
    "intellij-idea.desktop"
    
  04.1.1---------------------------------------
  
    em seguida cole o texto abaixo e salve. 
    (substitua "idea-Ic.183.4886.37" pelo nome sua pasta)
    // execute o código em um terminal para ver 
    //    {~$ cd /opt/}
    //    {~$ ls }
    
    
    [Desktop Entry]
    Name=IntelliJ IDEA
    Type=Application
    Exec=/opt/idea-Ic-183.4886.37/bin/idea.sh
    Terminal=false
    Icon=/opt/idea-Ic.183.4886.37/bin/idea.png
    Comment=Integrated Development Environment
    NoDisplay=false
    Categories=Development;IDE;
    Name[en]=IntelliJ IDEA
    Name[en_US]=IntelliJ IDEA
    Name[pt-BR]=IntelliJ IDEA
    
  04.1.2-------------------------------------------------
  
04.2- via terminal (ignore caso fez o passo manual) -----
    
   abra um novo terminal (ou Ctrl+Alt+T)
   digite:
   
    $ nano intellij-idea.desktop
    
    e digite o seguinte script, substituindo "idea-ic-183.4886.37"
    pelo nome de sua pasta atual (//check o passo 04.1.1//: 


      [Desktop Entry]
      Name=IntelliJ IDEA
      Type=Application
      Exec=/opt/idea-Ic-183.4886.37/bin/idea.sh
      Terminal=false
      Icon=/opt/idea-Ic.183.4886.37/bin/idea.png
      Comment=Integrated Development Environment
      NoDisplay=false
      Categories=Development;IDE;
      Name[en]=IntelliJ IDEA
      Name[en_US]=IntelliJ IDEA
      Name[pt-BR]=IntelliJ IDEA
      
  04.2.2--------------------------------------------------
  
    pressione as teclas ctrl+x para sair do modo de edição;
    
    pressione s e enter para confirmar e salvar.
    
 05.------------------------------------------------------
 
  digite o codigo para iniciar a instalação
  
    ~$ sudo desktop-file-install intellij-idea.desktop
    
  pronto, agora é só proceder a instalação da IDE.
  as shotcuts e icones de inicialização do applicativo foram adicionados
  
  lembrando que o mesmo serve para instalar o Android Studio e adicionar
  icone de atalho Click-once para inicializar nas distros linux, basta 
  adaptar os diretórios e nomes de arquivos.
