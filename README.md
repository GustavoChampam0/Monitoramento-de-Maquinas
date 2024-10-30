Sistema de Acompanhamento de Máquinas 
Este projeto implementa uma interface para monitorar o status de diversas máquinas, simulando a produção de peças, registro de falhas e controle de estoque de materiais. O sistema fornece notificações visuais e sonoras em caso de falhas ou falta de materiais, além de permitir a exportação de relatórios e visualização de gráficos do desempenho das máquinas.

Funcionalidades
Monitoramento de Máquinas: Cada máquina possui estados (funcionando/quebrada), e o sistema verifica automaticamente seu status, gerando uma falha aleatória com 50% de chance a cada verificação.
Gerenciamento de Materiais: Controle de estoque de materiais necessários para a produção de peças. Notificações são geradas caso o estoque fique baixo.
Produção e Refugo de Peças: As máquinas produzem peças ou adicionam ao refugo em caso de falha, com o controle de histórico de peças produzidas e de refugo.
Interface com Tkinter: Exibição visual do status das máquinas com indicadores de cores (verde/vermelho), e gráficos que mostram o histórico de funcionamento e refugo.
Notificações Sonoras e Relatórios: Notificações sonoras são emitidas para alertar sobre falhas. É possível exportar um relatório com o status atual das máquinas e inventário.
Gráficos: Gráficos interativos mostram o histórico de status de funcionamento e peças de refugo.
Requisitos
Python 3.x
Bibliotecas: tkinter, matplotlib, logging, random, deque, winsound
Instalação
Clone o repositório:

bash
Copiar código
git clone https://github.com/seu-usuario/sistema-acompanhamento-maquinas.git
Instale as dependências (se necessário):

bash
Copiar código
pip install matplotlib
Execute o arquivo principal:

bash
Copiar código
python sistema_acompanhamento.py
Como Usar
Monitoramento: A interface principal mostra as máquinas com seus status de funcionamento (indicadores coloridos) e dados de produção.
Recarregar Material: Insira uma quantidade de material e clique em "Recarregar" para adicionar ao estoque.
Exportar Relatório: Clique no botão "Exportar Relatório" para gerar um arquivo .txt com o status atual das máquinas e inventário.
Visualizar Gráficos: A aba de gráficos mostra o histórico de funcionamento e de peças de refugo de cada máquina.
Ajuda: No menu superior, clique em "Ajuda" para visualizar instruções de uso.
Estrutura do Código
Classe SistemaAcompanhamento: Responsável pela lógica de funcionamento do sistema, verificando status, gerenciando estoque, produzindo peças e notificando falhas.
Métodos Principais:
verificar_maquinas(): Atualiza o status das máquinas, produzindo peças ou registrando falhas.
recarregar_material(): Recarrega o estoque de materiais.
exportar_relatorio(): Gera um relatório de acompanhamento das máquinas.
atualizar_interface(): Atualiza a interface gráfica com os dados atuais.
atualizar_graficos(): Atualiza os gráficos de status e refugo.
Contribuição
Contribuições são bem-vindas! Para contribuir, faça um fork do repositório, crie uma branch com sua modificação e envie um pull request.
