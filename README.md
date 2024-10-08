## Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO.

# Resumo do lab Armazenamento

Serviços de armazenamento
Opções de redundância
Gerenciamento e migração de arquivos
Identificar opções para mover arquivos, AzCopy, o Gerenciador de Armazenamento do Azure e a Sincronização de Arquivos do Azure.
Redundância de armazenamento

## 
A redundância de armazenamento no Azure é uma opção que permite manter várias cópias de uma conta de armazenamento para garantir a disponibilidade e durabilidade dos dados, mesmo em caso de falhas.
* Armazenamento com redundância de zona geográfica (GZRS)
* Armazenamento com redundância geográfica (GRS)
* Armazenamento com redundância de zona (ZRS)
* Armazenamento com redundância local (LRS)
* LRS
A opção de menor custo, que replica os dados de forma síncrona três vezes em um único local físico na região primária
* ZRS
Replica os dados de forma síncrona em três zonas de disponibilidade do Azure na região primária.
* GRS
Replica os dados de forma síncrona na região primária e de forma assíncrona em uma região secundária.
* GZRS
Uma opção de redundância geográfica.

Blob do Azure: otimizado para o armazenamento de quantidades massivas de dados não estruturados.

Disco do Azure: fornece discos para máquinas virtuais, aplicativos e outros serviços acessarem e utilizarem.

Fila do Azure: serviço de armazenamento de mensagens que fornece armazenamento e recuperação para grandes quantidades de mensagens, cada uma com até 64 KB.

Arquivos do Azure: configura um compartilhamento de arquivos de rede altamente disponível que pode ser utilizado usando o protocolo Bloco de Mensagens do Servidor.

Tabelas do Azure: fornece uma opção de chave/atributo para o armazenamento de dados estruturados não relacionais com um design sem esquema.

## Quais são as camadas de acesso
* Quente: Ideal para dados que são acessados com frequência, como imagens de um site ou arquivos de log. Oferece o menor tempo de latência e o maior desempenho.
* Fria: Indicada para dados que são acessados raramente e armazenados por pelo menos 30 dias, como backups ou arquivos históricos. É a camada mais econômica.
* Frequente: Uma opção intermediária entre quente e fria, ideal para dados que são acessados com frequência moderada.
* Arquivos: Projetada para armazenar grandes volumes de dados não estruturados, como arquivos de mídia e backups.

## Opções de gerenciamento de arquivos
* Azure Files:
Compartilhamentos de arquivos SMB gerenciados totalmente na nuvem.
Acesso consistente de máquinas virtuais Windows e Linux, bem como aplicativos.
Ideal para compartilhamento de arquivos entre diferentes máquinas e aplicativos.
* Azure Blob Storage: Armazenamento de objetos não estruturados, como arquivos de imagem, vídeo, áudio e dados.
Escalabilidade e desempenho elevados para grandes volumes de dados.
Diversas camadas de acesso (quente, fria, arquivada) para otimizar custos.
* Azure Storage Explorer: Ferramenta gratuita para gerenciar todos os seus recursos do Azure Storage a partir de uma interface gráfica.
Permite visualizar, copiar, mover e excluir arquivos e containers.
* AzCopy é uma ferramenta de linha de comando poderosa e versátil, fornecida pela Microsoft, que permite copiar dados para e de contas de armazenamento do Azure de forma rápida e eficiente.


