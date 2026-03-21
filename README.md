# Guia de Instalação do Gentoo Linux com Cinnamon

Este repositório armazena o arquivo HTML contendo o guia de instalação passo a passo do Gentoo Linux focado no ambiente gráfico Cinnamon. O material foi elaborado para o site Viva o Linux por Xerxes Lins.

## Objetivo

O foco deste guia é a praticidade e a comodidade. A compilação de pacotes a partir do código-fonte é reduzida ao adotar pacotes binários pré-compilados (`getbinpkg`) sempre que disponibilizados pelos repositórios oficiais.

## Componentes da Instalação

O roteiro aborda a configuração dos seguintes elementos:

* Identificação automatizada de discos para manipulação de strings (NVMe ou SATA).
* Particionamento em padrão UEFI.
* Criptografia de disco (LUKS2 com Argon2id), mantendo `/boot` e `EFI` fora do contêiner criptografado.
* Sistema de arquivos Btrfs estruturado em subvolumes (`@`, `@home`, `@snapshots`).
* Sistema de inicialização `systemd`.
* Áudio gerenciado via PipeWire e WirePlumber.
* Otimização de rede sem fio utilizando `iwd` integrado ao NetworkManager.
* Gerenciamento de memória em bloco comprimido com `zram`.
* Configuração de autologin no gerenciador de sessão LightDM.
* Sincronização da árvore do Portage via repositório Git.

## Como acessar o guia

O roteiro de instalação encontra-se no arquivo `guia_gentoo_cinnamon.html`. Os blocos de comando possuem botões de cópia nativos para facilitar a execução no terminal.

Para ler o guia diretamente no navegador com a formatação correta, acesse a página gerada pelo GitHub Pages:

* **https://xerxeslins.github.io/guia-gentoo-cinnamon/guia_gentoo_cinnamon.html**
