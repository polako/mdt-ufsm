# mdt-ufsm
Estilo conforme regras da UFSM para trabalhos acadêmicos.

## Requisitos

abntex2

## Como utilizar

Colocar o arquivo na raíz e importar no preâmbulo:

> \usepackage{ufsm}

## Configurar

Em \documentoclass, setar os seguintes parâmetros:

    \documentclass[
        % -- opções da classe memoir --
        12pt,				    % tamanho da fonte
        openright,			% capítulos começam em pág ímpar (insere página vazia caso preciso)
        oneside,			  % para impressão em recto e verso. Oposto a oneside
        a4paper,			  % tamanho do papel. 
        % -- opções da classe abntex2 --
        chapter=TITLE,		% títulos de capítulos convertidos em letras maiúsculas
        section=TITLE,		% títulos de seções convertidos em letras maiúsculas
        % -- opções do pacote babel --
        english,			% idioma adicional para hifenização
        french,				% idioma adicional para hifenização
        spanish,			% idioma adicional para hifenização
        brazil				% o último idioma é o principal do documento
        ]{abntex2}

## Figuras

Necessário colocar fonte nas figuras.


    \begin{figure}[h]
        \centering
        \caption{Descriço da imagem.}
        \includegraphics[width=1\linewidth]{imgs/project_goal}
        \legend{Fonte: prórprio autor.}
        \label{fig:projectgoal}
    \end{figure}
