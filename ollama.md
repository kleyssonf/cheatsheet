# Ollama  

`curl -fsSL https://ollama.com/install.sh | sh`  
Roda script de instalação do ollama  

`ollama --version`  
preciso nem explicar  

`ollama serve`  
inicia o server do ollama, mas bloqueia o terminal e é preciso abrir outro terminal  

`ollama run llama3`  
baixo o modelo de linguagem llama3. É necessário o server estar rodando  
Para iniciar o ollama outras vezez  

`ls -l /dev/dxg`  
Se aparecer algo como  `crw-rw-rw- 1 root root...`  o WSL enxerga a VGA  

`sudo apt install -y mesa-va-drivers`  
Instalar bibliotecas para trabalhar com VGA da AMD  

`nohup ollama serve > ollama.log 2>&1 &`  
Executa o serviço ollama em sgunda instância  

`sudo systemctl start ollama`  
Inicia o Ollama em modo serviço, dispensando o comando acima  