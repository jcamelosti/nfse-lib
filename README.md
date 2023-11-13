# nfse-lib
Biblioteca para geração e comunicação da NFSe com as Prefeituras.

# php-nfse
**Framework para a integração com os sistemas de Notas Fiscais Eletrônicas de Serviços das Prefeituras Municipais**

# NOTA IMPORTANTE - LEIA COM MUITA ATENÇÃO

### As prefeituras **mudam de modelo de NFSe e alteram seu layout livremente e até a forma de acesso aos webservices**, isso é um FATO !!

>***Porém como nossa lib você não terá surpresar em integrar com os webeservices.***

Entregamos pronta para uso a lib no padrão composer.

**"GARATIMOS O FUNCIONAMENTO DE SUA INTEGRAÇÃO**

## RECOMENDAÇÃO

Entre em contato com nosso suporte de adquira já sua versão customizada - Damos total suporte(Pago).

## DEFINIÇÃO

A Nota Fiscal de Serviços Eletrônica - NFS-e é o documento fiscal de existência apenas digital que substituirá as tradicionais notas fiscais de serviços impressas.
A NFSe, implantada pelas Secretarias Municipais de Finanças, será emitida e armazenada eletronicamente em programa de computador, com o objetivo de materializar os fatos geradores do ISSQN – Imposto Sobre Serviços de Qualquer Natureza, por meio do registro eletrônico das prestações de serviços sujeitas à tributação do ISSQN.
Com a Nota Fiscal Eletrônica de Serviços você terá os seguintes benefícios:
- Redução de custos
- Redução de burocracia
- Incentivo ao relacionamento entre tomador e prestador
- Maior gerenciamento de notas emitidas e recebidas
- Economia de tempo e segurança com documentos de arrecadação

A emissão de NFSe depende de prévio cadastramento do emissor e da disponibilidade de certificado digital do tipo A1 (PKCS#12), emitido por certificadora no Brasil pertencente ao ICP-Brasil.

## PACOTE TESTADO E APROVADO EM VÁRIAS MUNICÍPIOS, totalmente usável!!

## Padrões

Existem muitos "padrões" diferentes para a emissão de NFSe, além disso, cada prefeitura pode fazer alterações no "padrão" escolhido, por isso, cada Prefeitura autorizadora deverá ser claramente identificada para que os códigos corretos sejam utilizados nas chamadas do framework. Fazemos toda a manutenção em seu código.

- Ábaco
- ABRASF
- Ágili
- ArrecadaNet
- Assessor Público
- AWATAR
- **BETHA - BETA-TESTS**
- BOANF
- BSIT-BR
- Cecam
- CENTI
- Comunix
- CONAM
- Consist
- COPLAN
- DB NFSE
- DEISS
- DigiFred
- **DSFNET - ALPHA-TESTS**
- Dueto
- DUETO 2.0
- E-Caucaia
- e-Governe ISS
- E-Nota Portal Público
- e-Receita
- E&L
- eISS
- Elotech
- Equiplano
- ETransparencia
- FacilitaISS
- FGMAISS
- FINTELISS
- FISS-LEX
- Freire
- GENERATIVA
- GINFES
- GLC Consultoria (Sumaré e Monte Mor)
- Goiânia
- Governa
- Governa TXT
- Governo Digital
- Governo Eletrônico
- INFISC
- INFISC – Santiago
- INFISC – Sapucaia
- INFISC Farroupilha
- **IPM - BETA-TESTS**
- ISISS
- ISS Intel
- ISS On-line Supernova
- ISS Online AEG
- ISS Simples SPCONSIG
- ISS4R
- ISSE
- **ISSNET - BETA-TESTS**
- ISSNFe On-line
- ISSWEB Camaçari
- ISSWEB Fiorilli
- JFISS Digital
- JGBAIAO
- Lençóis Paulista
- Lexsom
- Memory
- Metrópolis
- NF-Eletronica
- NF-em
- NFPSe
- NFSE-ECIDADES
- NFSeNET
- NFWEB
- Nota Blu
- **Nota Carioca (derivação ABRASF) - em desenvolvimento**
- Nota Natalense
- **Nota Salvador (derivação ABRASF) - em desenvolvimento**
- PMJP
- PortalFacil
- Prescon
- Primax Online
- **Prodam (NF Paulistana) - BETA-TESTS**
- PRODATA
- **Pública - BETA-TESTS**
- RLZ
- SAATRI
- SEMFAZ
- SH3
- SIAM
- SIGCORP – TXT
- SIGCORP BAURU
- SIGCORP Ivaipora
- SIGCORP Londrina
- SIGCORP Rio Grande
- SIGCORP São Gonçalo
- **SIGISS - BETA-TESTS**
- **SimplISS - Em desenvolvimento**
- SJP
- SMARAPD SIL Tecnologia
- SMARAPD SIL Tecnologia WS
- Solução Pública
- System
- Tecnos
- Thema
- Tinus
- Tinus Upload
- TIPLAN
- Tributos Municipais
- WEBISS

## Municipios atendidos pelo Framework

### ABRASF (BETA-TESTS) 
- Salvador (BA) ABRASF (modificado)
- Rio de Janeiro (RJ) ABRASF (modificado)
- São José dos Campos (SP) GINFESv3
- Limeira (SP) ETransparencia
- Itabira (MG) ABRASF (modificado)
- São Jose dos Pinhais (PR) ABRASF (modificado)

### BETHA (ALPHA-TESTS)
- Cruzeiro do Sul (C)
- Camaçari (BA)
- Quirinópolis (GO)
- Maracaju (MS)
- Cornélio Procópio (PR)
- Fazenda Rio Grande (PR)
- Ortigueira (PR)
- Paranavai (PR) Integrado
- São Mateus do Sul (PR)
- Resende (RJ)
- Rio das Flores (RJ)
- Gramado (RS)
- Lagoa Vermelha (RS)
- Palmeira das Missões (RS)
- Três Passos (RS)
- Biguaçu (SC)
- Canoinhas (SC)
- Criciúma (SC)
- Curitibanos (SC)
- Imbituba (SC)
- Jaraguá do Sul (SC)
- Joaçaba (SC)
- Lages (SC)
- Navegantes (SC)
- São Lourenço do Oeste (SC)
- São José (SC)
- Schroeder (SC)
- Gavião Peixoto (SP)
- Guatapará (SP)
- Jambeiro (SP)
- Monte Alto (SP)
- Orlândia (SP)

### DSFNET (ALPHA-TESTS)
- Campinas (SP)
- São Luis (MA)
- Belem (PA)
- Campo Grande
- Sorocaba (SP)
- Teresina (PI)
- Uberlandia (MG)

### ISSNET (BETA-TESTS)
- Alta Floresta (MT) Nota: incompleto falta URL de produção
- Anapolis (GO) Nota: incompleto falta URL de produção
- Andradina (SP) Nota: incompleto falta URL de produção
- Aparecida de Goiania (GO) Nota: incompleto falta URL de produção
- Aparecida (SP) Nota: incompleto falta URL de produção
- Araguaína (TO) Nota: incompleto falta URL de produção
- Bonito (MS) Nota: incompleto falta URL de produção
- Cascavel (PR) Nota: incompleto falta URL de produção
- Cruz Alta (RS) Nota: incompleto falta URL de produção
- Cuiaba (MT)
- Dourados (MT) Nota: incompleto falta URL de produção
- Itapetininga (SP) Nota: incompleto falta URL de produção
- Jacareí (SP) Nota: incompleto falta URL de produção
- Jaguariuna (SP) Nota: incompleto falta URL de produção
- Juara (MT) Nota: incompleto falta URL de produção
- Lorena (SP) Nota: incompleto falta URL de produção
- Mantena (MG) Nota: incompleto falta URL de produção
- Mogi das Cruzes (SP) Nota: incompleto falta URL de produção
- Naviraí (MS) Nota: incompleto falta URL de produção
- Nobres (MT) Nota: incompleto falta URL de produção
- Nova Alvorada do Sul (MS) Nota: incompleto falta URL de produção
- Nova Olimpia (MT) Nota: incompleto falta URL de produção
- Novo Hamburgo (RS) Nota: incompleto falta URL de produção
- Praia Grande (SP) Nota: incompleto falta URL de produção
- Ribeirão Preto (SP) : ABRASF (modificado)
- Rio Brilhante (MS) Nota: incompleto falta URL de produção
- Santa Maria (RS) Nota: incompleto falta URL de produção
- São Vicente (SP) Nota: incompleto falta URL de produção
- Serrana (SP) Nota: incompleto falta URL de produção
- Sidrolândia (MS) Nota: incompleto falta URL de produção
- Sorriso (MT) Nota: incompleto falta URL de produção
- Três Corações (MG) Nota: incompleto falta URL de produção	
- Várzea Grande (MT) Nota: incompleto falta URL de produção

### IPM (BETA-TESTS)
- COLOMBO (PR)

### PRODAM (BETA-TESTS)
- São Paulo (SP) Nota: não tem ambiente de testes

### Publica (BETA-TESTS)
- Timóteo (MG) 
- Caçador (SC) Integrado
- Chapecó (SC) 
- Itajaí (SC)  

### SIGISS SigCorp (BETA-TESTS) 
- Londrina (PR) SIGISS SigCorp v1.03
- Governador Valadares (MG) Sigicorp

### Simpliss Em desenvolvimento
- São Joao da Boa Vista (SP)

##Contato Técnico
-contato@josuecamelo.com
-(62) - 98401-8589
