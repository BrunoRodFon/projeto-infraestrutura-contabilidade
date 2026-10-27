# Resultados dos Testes de Infraestrutura

## 1. Endereçamento IP e DHCP

**Procedimento:** configurar um dispositivo final para obter endereço IP por DHCP e verificar os parâmetros recebidos.

**Parâmetros esperados:** endereço IP da VLAN correspondente, máscara `/24`, gateway padrão e servidor DNS configurado.

**Resultado:** registrar após a verificação das evidências no Packet Tracer.

## 2. Comunicação entre VLANs

**Procedimento:** executar comandos `ping` entre dispositivos de VLANs distintas, utilizando endereços de origem e destino conhecidos.

**Critério de validação:** a comunicação deve corresponder às regras de roteamento e às ACLs aplicadas. Destinos autorizados devem responder quando os serviços e dispositivos estiverem disponíveis; destinos bloqueados devem respeitar a política de segurança.

**Resultado:** registrar após a verificação das evidências no Packet Tracer.

## 3. DNS e acesso à intranet

**Procedimento:**
1. Verificar a configuração do serviço DNS no servidor `10.50.70.10`.
2. Confirmar a resolução de `intranet.contabilidade.local`.
3. Testar a conectividade com o servidor.
4. Acessar a intranet pelo navegador do dispositivo simulado.

**Critério de validação:** o nome deve ser resolvido para o endereço configurado e a página HTTP deve estar acessível conforme as permissões da rede.

**Resultado:** a resolução do nome, a resposta aos testes de conectividade e o acesso à página de boas-vindas foram observados durante a simulação.

## 4. Segmentação e enlaces trunk

**Procedimento:** executar os comandos de inspeção das VLANs, das portas e dos enlaces trunk nos switches.

**Critério de validação:** verificar as VLANs cadastradas, as portas associadas, as VLANs permitidas nos trunks e o estado de encaminhamento.

**Resultado:** foi identificada anteriormente uma condição de enlace trunk sem encaminhamento de VLANs. A configuração deve ser revisada e validada antes da aprovação definitiva desse teste.

## 5. Isolamento da rede de visitantes

**Procedimento:**
1. Conectar um cliente à rede de visitantes.
2. Confirmar o recebimento de endereço da faixa `10.50.100.0/24`.
3. Testar o acesso aos serviços necessários, como DHCP e DNS.
4. Executar tentativas de acesso a recursos internos que devem estar bloqueados, incluindo o servidor `10.50.70.10` e a rede de gerenciamento.

**Critério de validação:** o visitante deve utilizar os serviços autorizados sem obter acesso indevido às redes internas.

**Resultado:** o funcionamento deve ser confirmado pelas evidências posteriores à correção da porta do access point da recepção e pela verificação das ACLs.

## 6. Considerações finais

A conclusão dos testes deve se basear nos resultados observados e documentados. As pendências de configuração devem ser resolvidas antes de declarar a infraestrutura integralmente validada.

Os serviços de internet, compartilhamento de arquivos e backup deverão ser testados caso sejam implementados e estejam disponíveis no escopo da simulação.
