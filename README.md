# Teste de Sistemas Operativos - Módulo 3

Faz *fork* do repositório para teres a tua cópia.

Preenche o ficheiro README diretamente no GitHub. A partir da página principal do repositório, clica em "Edit File" (ícone representando um lápis).

Escreve as respostas dentro dos blocos correspondentes. Substitui as reticências pelo que é pedido em cada pergunta. Não desformates o documento.

Quando acabares, carrega no botão "Commit Changes".

## Informação do aluno

    Nome: Bohdan Radchik

## P1 - Para as seguintes questões, assinala a opção correta: (2.5v)

  1. Qual das seguintes afirmações caracteriza melhor um SO servidor?

    a) Projetado para computação de uso geral
    b) Otimizado para alta disponibilidade e confiabilidade
    c) Destinado a usuários individuais
    d) Usado principalmente para jogos
    
    Resposta: b

  2. Das seguintes, qual é a função mais apropriada para um SO servidor?

    a) Executar aplicações de desktop
    b) Desenvolver aplicações móveis
    c) Fornecer software de entretenimento
    d) Gerir recursos e serviços de rede
    
    Resposta:d 
   
  3. Qual dos seguintes é um sistema operativo servidor popular?

    a) Windows 11
    b) macOS Big Sur
    c) Ubuntu Server
    d) Android
    
    Resposta: c

  4. Qual é o papel de um servidor num modelo cliente-servidor?

    a) Consumir recursos fornecidos pelos clientes
    b) Fornecer recursos e serviços aos clientes
    c) Atuar como uma estação de trabalho independente
    d) Facilitar a comunicação ponto a ponto
    
    Resposta: b

  5. Qual dos seguintes protocolos é mais usado para aceder remotamente a servidores?

    a) FTP
    b) HTTP
    c) SSH
    d) SMTP
    
    Resposta: c

## P2 - Indica, sequencialmnente, os comandos para realizar as seguintes instruções: (7.5v)

  1. Cria um diretório com o nome "ex1", entra no mesmo, e cria 3 ficheiros vazios com os nomes "f1", "f2", "f3". No fim, lista os conteúdos do diretório atual.

    Resposta:
    mkdir ex1            
    cd ex1               
    touch f1 f2 f3       
    ls   
    
  2. Assumindo que estás no diretório "ex1", renomeia os ficheiros "f1" e "f2" para que acabem com "_antigo", e cria cópias dos mesmos.

    Resposta:
    mv f1 f1_antigo     
    mv f2 f2_antigo     
    cp f1_antigo f1      
    cp f2_antigo f2

  3. Assumindo que estás no diretório "ex1", cria o diretório "ex2", e move os ficheiros copiados no exercício anterior para o novo diretório. Seguidamente, apaga os ficheiros originais.

    Resposta:
    mkdir ex2              
    mv f1 f2 ex2/           
    rm f1_antigo f2_antigo

  4. Atualiza os repositórios de *packages* para garantir acesso às *packages* mais recentes, e instala o serviço **htop**.

    Resposta:
    sudo apt update              
    sudo apt install htop        


  5. Cria um novo utilizador com o teu primeiro nome, e com o diretório "/home/nome_de_utilizador". Mostra a informação (ID) do utilizador criado.

    Resposta:
    ...

## P3 - Realiza os seguintes exercícios, com respostas detalhadas: (6v)

  1. Indica alguns aspetos que diferenciam um SO cliente de um SO servidor.

    Resposta:
    Recursos e Capacidades:
    Cliente: Suporte a multimídia e uma ampla gama de periféricos; foco na experiência do usuário final.
    Servidor: Otimizado para alta carga de trabalho, com suporte a grandes quantidades de memória, processamento e armazenamento.
    Segurança:
    Cliente: Medidas de segurança básicas focadas na proteção contra malware e acessos não autorizados.
    Servidor: Segurança robusta com firewalls, sistemas de detecção de intrusão, políticas restritas de acesso e criptografia, devido à exposição a ameaças mais complexas.

     
  2. Explica a importância de otimizar um sistema operativo servidor, com exemplos de técnicas para otimização.

    Resposta:
    A otimização de um sistema operacional de servidor é essencial para melhorar a eficiência, o desempenho e a segurança, além de garantir o uso eficaz dos recursos de hardware. 

  3. Descreve o processo de instalar e configurar um servidor web num SO servidor, incluindo as etapas necessárias.

    Resposta:
    1. Preparação do Sistema
    Antes de instalar qualquer software, é importante garantir que o sistema operacional esteja atualizado.
    2. Instalação do Servidor Web
    O Apache pode ser facilmente instalado através do gerenciador de pacotes.
    3. Configuração Inicial
    Após a instalação, é importante verificar se o Apache está funcionando corretamente.
    4. Configuração de Hospedagem de Sites
    Para hospedar vários sites, o Apache utiliza uma abordagem baseada em virtual hosts.
    5. Testando o Servidor Web
    Você pode testar o servidor acessando o endereço IP do servidor ou o nome de domínio configurado em um navegador web para verificar se o site está sendo servido corretamente.
    6. Manutenção e Segurança
    Finalmente, é crucial manter o servidor seguro e atualizado. Isso inclui instalar certificados SSL/TLS para segurança HTTPS, configurar restrições de diretório e monitorar os logs de acesso e erros.


## P4 - Indica os comandos **git** para realizar as seguintes operações: (4v)

  1. Considera que estás no ramo 'master' de um repositório git criado localmente. Associa este repositório ao repositório remoto contido no url 'https://github.com/SO/OMeuRepositorioRemoto'. Altera o nome do ramo atual para 'main', e envia os *commits* já feitos localmente para o repositório remoto.

    Resposta:
    git remote add origin https://github.com/SO/OMeuRepositorioRemoto
    git branch -m master main
    git push -u origin main


  2. Considera que estás na pasta raiz do teu repositório local, onde atualizaste um ficheiro de nome 'index.html'. Envia **apenas** esta atualização para o teu repositório remoto, com uma mensagem de commit apropriada.

    Resposta:
    git add index.html
    git commit -m "Update index.html with new content"
    git push



