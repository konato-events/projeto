TheConf - Projeto
=================

Repositório dos arquivos de documentação geral do projeto.
Contém os arquivo LaTeX necessários para gerar o documento formal de especificação inicial do sistema.

Instalação dos componentes necessários
--------------------------------------

Segue aqui o passo-a-passo de instalação do TeX e dos pacotes necessários no projeto. Ele é necessário para evitar gastar mais de 3.5GB de espaço somente com o LaTeX. A instalação final fica com menos de 500MB.

1. [Baixar o TeX Live](https://www.tug.org/texlive/acquire.html). Eu baixei a ISO grande, mas acredito que o instalador via web também sirva.
2. Instalar o Perl-Tk: `sudo apt-get install perl-tk`
3. Executar o instalador: `sudo ./install-tk -gui`
4. Alterar a opção chamada "Selected Scheme" para "basic scheme"
5. Selecionar as seguintes collections, na opção abaixo:
    - Essential programs and files
    - TeX auxilliary programs
    - Recommended Fonts
    - Graphics and font utillities
    - Generic recommended packages
    - US and UK English
    - Portuguese
    - LaTeX fundamental packages
    - LaTeX recommended packages
    - Graphics, pictures, diagrams
6. Desabilitar instalação de documentação e sources, clicando no "Toggle" dos respectivos "Install font/macro doc tree" e "Install font/macro source tree".
7. Habilitar a opção "Create symlinks in system directories", clicando no botão "Change" e marcando a checkbox do diálogo que aparecer - os valores que aparecerem nas caixas de texto podem ser deixados conforme o default.
8. Verifique a necessidade de atualizar o gerenciador de pacotes do TeX antes de prosseguir: `sudo tlmgr update --self`
9. Agora, prossiga instalando os seguintes pacotes restantes: `sudo tlmgr install abntex2 enumitem csquotes etoolbox sidecap nowidow footmisc fmtcount multirow biblatex logreq`

Pronto! O LaTeX e todos os pacotes necessários estão instalados. Recomendo a utilização do TeX Studio ou Texmaker para edição do projeto.