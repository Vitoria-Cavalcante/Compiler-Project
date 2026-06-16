# Compiler-Project
Compilador completo didádico e funcional desenvolvido na matéria de compiladores do sétimo semestre.

MiniLang Compiler
O MiniLang Compiler é um projeto educacional funcional escrito em Python 3.13 que implementa todas as fases clássicas de um compilador para uma linguagem chamada .mini. Desde a análise léxica até a execução em uma Máquina Virtual (VM) de pilha, este projeto demonstra como transformar código-fonte em execução real.

Sobre o Projeto
Este compilador foi construído para ilustrar a engenharia por trás das linguagens de programação. Ele segue um pipeline rigoroso de 6 fases, garantindo que o código seja validado, tipado e traduzido eficientemente.

rquitetura do Pipeline
- Lexer: Tokenização do código bruto.
- Parser: Construção da Árvore Sintática Abstrata (AST).
- Semantic Analyzer: Verificação de tipos e tabela de símbolos.
- IR Generator: Geração de Código de Três Endereços (TAC).
- Code Generator: Tradução para Bytecode de Pilha.
- Virtual Machine: Execução do bytecode.

🛠️ Como Executar
1. Pré-requisitos
Certifique-se de ter o Python 3.13 ou superior instalado no seu sistema.

2. Preparação do Ambiente
O projeto utiliza a biblioteca docx para gerar a documentação técnica automaticamente. Se você não a tiver, instale-a via npm ou pip (ajuste conforme seu ambiente de desenvolvimento):
- Bash:
# Caso esteja rodando o script gerador de docx
npm install docx

3. Rodando o Compilador
Para compilar um arquivo .mini, utilize o arquivo main.py como entrada:
- Bash
python3 main.py seu_arquivo.mini

4. Gerando a Documentação Técnica
O repositório contém um script gerador de documentação que cria um arquivo .docx detalhando toda a arquitetura interna do compilador. Para executá-lo:
- Bash
node gerar_documentacao.js
*(Certifique-se de que os caminhos dos módulos no script estejam apontando corretamente para os arquivos .py conforme sua estrutura local).



Recursos da Linguagem Mini:
A linguagem suporta as construções fundamentais para aprendizado de lógica de programação
- :Tipagem: int, bool, string;
- Controle de Fluxo: if/else e while;
- Interatividade: Comandos read() e print();
- Operadores: Aritméticos, comparativos e lógicos.


📁Estrutura do Repositório (Mapeamento)Devido ao sistema de upload, os arquivos possuem nomes de mapeamento lógico:
Arquivo (Classe)                Responsabilidade
ast_nodes.py                     Definição da hierarquia da AST
lexer.py                         Analisador Léxico
parser.py                        Analisador Sintático (RDP)
semantic.py                      Análise Semântica e Tabelas
ir_generator.py                  Geração de Código Intermediário
code_generator.py                Conversão para Bytecode
vm.py,Máquina                    Virtual de Pilha


Contribuições:
Sinta-se à vontade para abrir Issues ou Pull Requests. Este projeto tem o intuito de ser uma base didática para estudantes de engenharia de software e teoria de compiladores.

Desenvolvido como um exercício de arquitetura de compiladores.

