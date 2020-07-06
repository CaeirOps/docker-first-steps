# Imagem de referência Python
FROM python:3.7-slim

# Selecionando o diretório do container para a execução dos comandos a seguir
WORKDIR /app

# Copiando o conteúdo do diretório que criamos para dentro do diretório do container
COPY . /app

# Instalando pacotes adicionais informados no arquivo requisitos.txt
RUN pip install --trusted-host pypi.python.org -r requisitos.txt

# Habilitando a porta 80 do container para receber conexões externas
EXPOSE 80

# Definindo variável de ambiente
ENV NAME World

# Executando aplicação Python após inicialização do container
CMD ["python", "app.py"]
