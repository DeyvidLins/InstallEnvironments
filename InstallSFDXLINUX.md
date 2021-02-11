Instale a CLI no Linux
A versão Linux do Salesforce CLI é distribuída como um tarball.

Encontre o URL de download para seu tarball neste arquivo de manifesto . o downloads listas de seção de URLs não versionados para os instaladores mais recentes, que são especialmente úteis para casos de uso de CI. Selecione o URL com base em sua plataforma de destino.

    Baixe ou wget um desses tarballs.

        1ª - wget https://developer.salesforce.com/media/salesforce-cli/sfdx-cli/channels/stable/sfdx-linux-amd64.tar.xz

Crie um sfdx diretório .

        2ª - mkdir sfdx

Descompacte o conteúdo de sua versão tarball:

        3ª - tar xJf sfdx-linux-amd64.tar.xz -C sfdx --strip-components 1

-C descompacta o conteúdo no sfdx diretório , enquanto --strip-components 1 remove o componente do caminho raiz.
Execute o script de instalação.

        4ª - ./sfdx/install

O Salesforce CLI é instalado em / usr / local / bin / sfdx . Os instaladores são projetados para fornecer permissões para os diretórios de instalação. Se você receber permissão ou acessar erros que você não pode endereçar usando sudo ou chmod , tente instalar a CLI usando npm. 