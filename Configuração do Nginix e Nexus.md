<h3>1ª Vá para a pasta scripts: </h3><br/>
cd scripts:heavy_check_mark:<br/>
<h3>2ª Execute o comando abaixo:</h3><br/>
./nexus-nginxproxy.sh:heavy_check_mark:<br/>
<h3>3ª Insira as informações das credencias que estão nas partes comentadas;</h3><br/>
<h3>4ª Será criado uma pasta chamada certificates;</h3><br/>
<h3>5ª Após ter rodado todo seu código, seu Nexus estará sendo executado na porta 8081:</h3><br/>
http://localhost:8081:heavy_check_mark:<br/>
<h3>6ª Após a porta 8081 funcionando, configure o docker proxy e hosted;</h3><br/>
<h3>7ª De preferência configure o docker proxy para 8082 e o hosted para 8083;</h3><br/>
<h3>8ª Por fim, execute o comando abaixo (Obs. Execute somente o que você deseja realizar o login):</h3><br/>
docker login 8082 para login no proxy;:heavy_check_mark:<br/>
docker login 8083 para login no hosted;:heavy_check_mark:<br/>
<h3>9ª Liste suas images e user o docker tag:</h3><br/>
Ex.: docker tag {NOME_IMAGEM_ANTIGA} {NOME_IMAGEM_NOVA:1.O}(Obs.: Sem as Chaves):heavy_check_mark: 
<h3>10ª Execute o docker push <NOME_IMAGEM_NOVA:1.O>:heavy_check_mark:</h3><br/>
<h3>11ª Pronto</h3><br/>