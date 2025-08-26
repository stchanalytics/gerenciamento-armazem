# Projeto de Gerenciamento de Armazém

Este projeto de banco de dados relacional foi desenvolvido para gerenciar e otimizar as operações de um armazém. A estrutura foi projetada para lidar com um sistema complexo de fornecedores, peças, departamentos e projetos, demonstrando um conhecimento aprofundado em modelagem de dados e integridade referencial.
Tecnologias Utilizadas

    SQL (Linguagem de Definição e Manipulação de Dados): Usado para criar a estrutura do banco de dados e as consultas.

    MySQL: Sistema de gerenciamento de banco de dados (SGBD) utilizado para hospedar a base de dados.

Estrutura do Banco de Dados

A arquitetura do banco de dados segue a normalização para garantir a consistência e a robustez dos dados. Ele é composto pelas seguintes tabelas:

    DDD: Armazena os códigos DDD e suas respectivas regiões, garantindo a validação de telefones.

    FORNECEDOR: Lista todos os fornecedores do sistema.

    DEPARTAMENTO: Contém a hierarquia de setores da empresa.

    FUNCIONARIO: Armazena as informações dos funcionários, incluindo o salário e a data de início.

    TELEFONE: Lida com os números de telefone de funcionários e fornecedores, associando-os a um DDD.

    PROJETO: Registra os projetos com seus orçamentos.

    FUNCIONARIO_PROJETO: Tabela de junção que gerencia o relacionamento muitos-para-muitos (N:N) entre FUNCIONARIO e PROJETO, registrando as horas trabalhadas.

    DEPOSITO: Tabela que lista os depósitos da empresa.

    ENDERECO: Armazena os endereços de fornecedores e depósitos em uma tabela separada para otimização.

    PECA: Registra as peças com peso e cor, garantindo que o peso seja um valor positivo.

    PECA_FORNECEDOR: Tabela de junção para o relacionamento entre PECA e FORNECEDOR.

    FORNECEDOR_PROJETO: Tabela de junção para gerenciar os materiais fornecidos por cada fornecedor para projetos específicos.

Funcionalidades da Estrutura

Este banco de dados foi projetado para suportar as seguintes operações e consultas complexas:

    Integridade Referencial: Relações bem definidas entre tabelas para evitar dados órfãos e garantir a precisão das informações.

    Rastreamento de Recursos: Acompanhamento detalhado de peças e materiais, incluindo seu peso, cor e a qual depósito pertencem.

    Gerenciamento de RH e Projetos: Capacidade de associar funcionários a projetos, registrar horas trabalhadas e gerenciar salários.

    Controle de Fornecedores: Rastreamento de materiais fornecidos por cada fornecedor e seu envolvimento em diferentes projetos.

    Otimização de Consultas: A estrutura permite a execução de consultas complexas, como listar fornecedores que participam de múltiplos projetos ou a média salarial de funcionários.

Como Usar

Para configurar o banco de dados localmente, siga estes passos:

    Certifique-se de ter um servidor MySQL instalado e em execução em sua máquina.

    Copie o conteúdo do arquivo SQL (projeto_armazem.sql ou similar) que define a estrutura do banco de dados.

    Abra um cliente MySQL (como MySQL Workbench, DBeaver ou a linha de comando) e execute o script SQL.

Isso criará o banco de dados industria e todas as tabelas, deixando a estrutura pronta para ser populada com dados.
