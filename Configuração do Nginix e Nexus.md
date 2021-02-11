1ª Vá para a pasta scripts: <br/>
cd scripts:heavy_check_mark:<br/>
2ª Execute o comando abaixo:<br/>
./nexus-nginxproxy.sh:heavy_check_mark:<br/>
3ª Insira as informações das credencias que estão nas partes comentadas;<br/>
4ª Será criado uma pasta chamada certificates;<br/>
5ª Após ter rodado todo seu código, seu Nexus estará sendo executado na porta 8081:<br/>
http://localhost:8081:heavy_check_mark:<br/>
6ª Após a porta 8081 funcionando, configure o docker proxy e hosted;<br/>
7ª De preferência configure o docker proxy para 8082 e o hosted para 8083;<br/>
8ª Por fim, execute o comando abaixo (Obs. Execute somente o que você deseja realizar o login):<br/>
docker login 8082 para login no proxy;:heavy_check_mark:<br/>
docker login 8083 para login no hosted;:heavy_check_mark:<br/>
9ª Liste suas images e user o docker tag:<br/>
Ex.: docker tag <NOME_IMAGEM_ANTIGA> <NOME_IMAGEM_NOVA:1.O>:heavy_check_mark:<br/>
10ª Execute o docker push <NOME_IMAGEM_NOVA:1.O>:heavy_check_mark:<br/>
11ª Pronto<br/>