# Simulação no Cisco Packet Tracer

## Arquivo principal

- `infraestrutura-contabilidade.pkt` — arquivo da simulação lógica da infraestrutura de rede proposta para o escritório de contabilidade.

## Como abrir

1. Instale e abra o Cisco Packet Tracer.
2. Baixe o arquivo `infraestrutura-contabilidade.pkt` deste repositório.
3. No Packet Tracer, selecione **File > Open** e escolha o arquivo.
4. Aguarde o carregamento dos dispositivos e examine a topologia e as configurações.

O funcionamento do arquivo pode variar conforme a versão do Packet Tracer utilizada.

## Escopo da simulação

A simulação representa a infraestrutura lógica proposta, incluindo os dispositivos de rede e os segmentos definidos no projeto. Consulte o relatório acadêmico para obter o detalhamento da topologia, do endereçamento IP, das VLANs e dos serviços previstos.

Entre as configurações documentadas no projeto estão:

- Segmentação da rede por VLANs.
- Roteamento entre VLANs.
- Pools DHCP para as redes configuradas.
- Serviço DNS e acesso ao endereço `intranet.contabilidade.local`.
- Regras ACL para restringir o acesso à rede de gerenciamento e isolar a rede de visitantes.

A lista acima descreve o escopo do projeto; consulte `Testes/resultados.md` para verificar quais itens foram efetivamente validados e quais continuam pendentes.

## Arquivos relacionados

- `../Documentacao/` — relatório, planta física e diagrama do rack.
- `../ACLs/` — objetivos, configurações e vídeos das ACLs.
- `../Testes/` — evidências e resultados dos testes.

## Observação

O arquivo `.pkt` é o artefato principal para explorar a simulação. Não considere uma funcionalidade aprovada apenas por estar configurada: confira o resultado dos testes registrados na documentação.
