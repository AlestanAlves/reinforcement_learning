# Reinforcement Learning

Deep Reinforcement Learning at USP - Summer Course
```
source activate rlsummer 
``` 

- [x]  Class 1 - 11/02/2020
- [x]  Class 2 - 12/02/2020
- [ ]  Class 3 - 13/02/2020
- [ ]  Class 4 - 14/02/2020


### Instalando e configurando o ambiente:

Com o intuito de garantir que nossas instalações não conflitem com instalações nativas do python e que tenhamos todos os pacotes necessários
a nossas atividades, elaboramos este tutorial para que todos possam ter ambientes padronizados de desenvolvimento.

Utilizaremos o Miniconda como gerenciador de ambientes. Siga o passo a passo, pulando as etapas que já tiverem sido feitas

1) Instalando o conda:

- Windows:
    Baixe o arquivo: https://repo.anaconda.com/miniconda/Miniconda3-latest-Windows-x86_64.exe
    Execute as etapas de instalação conforme o assitente indicar. Não é necessário marcar nenhuma opção extra

-Linux:
        Baixe o arquivo: https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
        Abra o terminal e navegue até a pasta onde o script foi baixado
        Rode a seguinte linha de comando: ```bash ./Miniconda3-latest-Linux-x86_64.sh```
        Abra o terminal e rode o comando ```conda init```
        Feche o terminal e o reabra

Caso algo saia errado, por favor verifique instruções em: https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html

2) Criando o ambiente
- Windows:
    Abra o menu Iniciar, busque por Ananconda prompt e abra o programa

- Linux:
    Abra o terminal

- Ambos (após os anteriores):
    ```conda create -n rlsummer python=3.6 --yes```

3) Instalando os pacotes:
    Uma vez no terminal ou prompt do Anaconda, rode os seguintes comandos:
        conda activate rlsummer
        conda install -c conda-forge jupyterlab --yes
        pip install numpy tensorflow-cpu tensorflow-probability streamlit gym bokeh git+https://github.com/eleurent/highway-env pandas seaborn matplotlib pydot graphviz


4) Carregando o ambiente
- Windows:
    Abra o menu Iniciar, busque por Ananconda prompt e abra o programa
    Rode o comando: conda activate rlsummer

- Linux:
    Abra o terminal e rode o comando: ```conda activate rlsummer```
    alternativamente pode ser executado o comando: ```source activate rlsummer```
