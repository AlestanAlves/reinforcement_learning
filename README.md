# Deep Reinforcement Learning at USP - Summer Course

- Ativar o ambiente

```
conda activate rlsummer 
``` 


- [x]  Class 1 - 11/02/2020
- [x]  Class 2 - 12/02/2020
- [x]  Class 3 - 13/02/2020
- [x]  Class 4 - 14/02/2020
- [x]  Class 5 - 17/02/2020

### Books 

- [Reinforcement Learning: An Introduction](http://incompleteideas.net/book/RLbook2018.pdf) (Sutton & Barto 2018, 2nd Edition)
- [Deep Learning](https://www.deeplearningbook.org/) (Goodfellow, Bengio and Courville, 2016)

### Links

- OpenAI [Gym](http://gym.openai.com/)
- OpenAI [Spinning Up](https://spinningup.openai.com/en/latest/spinningup/rl_intro.html)
- Tensorflow [Tutorials](https://www.tensorflow.org/tutorials)
- Tensorflow [Probability](https://www.tensorflow.org/probability)
- [Keras](https://keras.io/)
- https://www.3blue1brown.com/neural-networks
- An overview of gradient descent optimization algorithms (https://ruder.io/optimizing-gradient-descent/)

### Papers 

- [Challenges of Real-World Reinforcement Learning](https://arxiv.org/abs/1904.12901) (Dulac-Arnold, Mankowitz, and Hester, 2019)
- [Reinforcement Learning Applications](https://arxiv.org/abs/1908.06973) (Li, 2019)
- [Policy Gradient Methods for Reinforcement Learning with Function Approximation](https://papers.nips.cc/paper/1713-policy-gradient-methods-for-reinforcement-learning-with-function-approximation.pdf) (Sutton, R.S., McAllester, D.A., Singh, S.P. and Mansour, Y., 2000)
- [Deep Learning in Neural Networks: An Overview](https://arxiv.org/abs/1404.7828) (Schmidhuber, 2014)
- [An overview of gradient descent optimization algorithms](https://arxiv.org/abs/1609.04747) (Ruder, 2017)


### Instalando e configurando o ambiente:

Com o intuito de garantir que nossas instalações não conflitem com instalações nativas do python e que tenhamos todos os pacotes necessários
a nossas atividades, elaboramos este tutorial para que todos possam ter ambientes padronizados de desenvolvimento.

Utilizaremos o Miniconda como gerenciador de ambientes. Siga o passo a passo, pulando as etapas que já tiverem sido feitas

Colocar no bash

```export PATH=$HOME/bin:/usr/local/bin:$PATH:~/miniconda3/bin/```

```
# >>> conda initialize >>>
# !! Contents within this block are managed by 'conda init' !!
__conda_setup="$('/home/alestan/miniconda3/bin/conda' 'shell.zsh' 'hook' 2> /dev/null)"
if [ $? -eq 0 ]; then
    eval "$__conda_setup"
else
    if [ -f "/home/alestan/miniconda3/etc/profile.d/conda.sh" ]; then
        . "/home/alestan/miniconda3/etc/profile.d/conda.sh"
    else
        export PATH="/home/alestan/miniconda3/bin:$PATH"
    fi
 ```

1) Instalando o conda:

- Windows:
    Baixe o arquivo: https://repo.anaconda.com/miniconda/Miniconda3-latest-Windows-x86_64.exe
    Execute as etapas de instalação conforme o assitente indicar. Não é necessário marcar nenhuma opção extra

- Linux:
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
    
