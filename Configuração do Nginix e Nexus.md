1ª Vá para a pasta scripts: 
   cd scripts
2ª Execute o comando abaixo:
    ./nexus-nginxproxy.sh
3ª Insira as informações das credencias que estão nas partes comentadas;
4ª Será criado uma pasta chamada certificates;
5ª Após ter rodado todo seu código, seu Nexus estará sendo executado na porta 8081:
    http://localhost:8081
6ª Após a porta 8081 funcionando, configure o docker proxy e hosted;
7ª De preferência configure o docker proxy para 8082 e o hosted para 8083;
8ª Por fim, execute o comando abaixo (Obs. Execute somente o que você deseja realizar o login):
    docker login 8082 para login no proxy;
    docker login 8083 para login no hosted;
9ª Liste suas images e user o docker tag:
    Ex.: docker tag <NOME_IMAGEM_ANTIGA> <NOME_IMAGEM_NOVA:1.O>
10ª Execute o docker push <NOME_IMAGEM_NOVA:1.O>
11ª Pronto