```mermaid

flowchart LR

%% Colors %%
classDef blue fill:#2374f7,stroke:#000,stroke-width:2px,color:#fff
classDef orange fill:#fc822b,stroke:#000,stroke-width:2px,color:#fff
classDef green fill:#16b552,stroke:#000,stroke-width:2px,color:#fff
classDef pink fill:#ff69b4,stroke:#000,stroke-width:2px,color:#fff
classDef slateblue3 fill:#6959cd,stroke:#000,stroke-width:2px,color:#fff
classDef skyblue fill:#87cefa,stroke:#000,stroke-width:2px,color:#fff
classDef darkblue fill:#000080,stroke:#000,stroke-width:2px,color:#fff
classDef sienna fill:#a0522d,stroke:#000,stroke-width:2px,color:#fff
classDef dimgray fill:#696969,stroke:#000,stroke-width:2px,color:#fff
classDef steelblue fill:#4682b4,stroke:#000,stroke-width:2px,color:#fff
classDef royalblue fill:#4169e1,stroke:#000,stroke-width:2px,color:#fff
classDef lightgreen fill:#90ee90,stroke:#000,stroke-width:2px,color:#fff
classDef teal fill:#008080,stroke:#000,stroke-width:2px,color:#fff
classDef springgreen fill:#00ff7f,stroke:#000,stroke-width:2px,color:#fff
classDef darkseagreen fill:#8fbc8f, stroke:#000, stroke-width:2px,color:#fff
classDef white fill:#ffffff, stroke:#000, stroke-width:2px,color:#fff

A(["raiz do sistema
 / "])
B(/bin):::blue
C(/boot):::green
D(/dev):::royalblue
E(/etc):::teal
F(/home):::sienna
G(/media):::pink
H(/mnt):::darkblue
I(/opt):::skyblue
J(/sbin):::darkseagreen
K(/srv):::orange
L(/tmp):::lightgreen
M(/usr):::springgreen
N(/var):::slateblue3
O(/root):::dimgray
P(/proc):::steelblue

AB(binarios essenciais do usuario)
AC(arquivos estaticos de boot)
AD(arquivos de dispositivos 'devices')
AE(arquivos de configuracao nao especificos)
AF(pastas dos usuarios comuns do sistema)
AG(ponto de montagem temporario para midias removiveis)
AH("`ponto de montagem temporario para sistemas 
de arquivos montados`")
AI(softwares adicionais 'adicionados pelo usuario')
AJ(binarios do sistema)
AK(dados para servicos providos pelo sistema)
AL(arquivos temporarios)
AM(multi-usuario utilitarios e aplicacoes)
AN(arquivos variaveis 'conteudo dinamico')
AO(home do superusuario 'root')
AP("`sistema de arquivos virtual, documentos do kernel e 
status de processos como arquivo de teto`")

A --> B --- AB 
A --> C --- AC
A --> D --- AD
A --> E --- AE
A --> F --- AF
A --> G --- AG
A --> H --- AH
A --> I --- AI
A --> J --- AJ
A --> K --- AK
A --> L --- AL
A --> M --- AM
A --> N --- AN
A --> O --- AO
A --> P --- AP

