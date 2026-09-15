# NFSe Lib

## Biblioteca PHP para integração com NFS-e — Nota Control / ISSNET

Biblioteca PHP para **geração, assinatura, transmissão, consulta e integração de NFS-e (Nota Fiscal de Serviço Eletrônica)** utilizando os serviços disponibilizados pela **Nota Control / ISSNET**, com suporte completo ao **Padrão Nacional da NFS-e**.

A `nfse-lib` foi desenvolvida para facilitar a integração de sistemas ERP, sistemas financeiros, plataformas SaaS, sistemas de gestão e aplicações próprias aos ambientes de NFS-e.

> **Status atual:** 16 municípios implementados para Nota Control / ISSNET e implementação pronta para o **Padrão Nacional da NFS-e**.

---

## 🚀 Status do projeto

### ✅ Nota Control / ISSNET

A biblioteca possui implementação para **16 municípios atualmente atendidos pela Nota Control / ISSNET**.

### ✅ Padrão Nacional da NFS-e

A biblioteca está **totalmente pronta para trabalhar com o Padrão Nacional da NFS-e**, incluindo a estrutura necessária para geração e processamento dos documentos conforme o modelo nacional.

A implementação considera os principais conceitos e estruturas do padrão, incluindo:

- DPS — Declaração de Prestação de Serviço;
- NFS-e;
- prestador;
- tomador;
- serviço;
- valores;
- tributação;
- retenções;
- códigos de serviço;
- informações municipais;
- informações nacionais;
- endereços no Brasil;
- endereços no exterior;
- comércio exterior;
- assinatura digital;
- geração de XML;
- validação estrutural;
- comunicação com os serviços correspondentes.

---

# 📋 Sobre o projeto

A emissão de NFS-e no Brasil possui um cenário de integração bastante fragmentado.

Mesmo com a existência de padrões nacionais, os municípios e provedores podem possuir particularidades relacionadas a:

- layouts XML;
- versões de schemas;
- regras de validação;
- autenticação;
- certificados digitais;
- assinatura XML;
- endpoints;
- ambientes de homologação e produção;
- códigos de serviço;
- regras tributárias;
- métodos de consulta;
- métodos de cancelamento;
- mensagens e códigos de retorno.

A `nfse-lib` tem como objetivo concentrar essa complexidade em uma biblioteca específica de integração fiscal.

Dessa forma, o sistema que utiliza a biblioteca pode trabalhar com uma estrutura de dados organizada, enquanto a `nfse-lib` fica responsável pela comunicação e pelas particularidades da integração.

---

# 🎯 Objetivos

Os principais objetivos da biblioteca são:

- simplificar a integração com NFS-e;
- reduzir código específico dentro do ERP;
- centralizar a geração dos XMLs;
- centralizar a assinatura digital;
- padronizar os dados fiscais;
- facilitar a comunicação com WebServices;
- tratar respostas dos provedores;
- permitir expansão para novos municípios;
- manter separadas as regras de negócio e as regras de integração fiscal;
- oferecer uma base preparada para o Padrão Nacional da NFS-e.

---

# 🏛️ Nota Control / ISSNET

A biblioteca possui foco atual nas integrações disponibilizadas pela **Nota Control / ISSNET**.

Mesmo utilizando o mesmo provedor, municípios diferentes podem possuir configurações e comportamentos próprios.

Por esse motivo, a biblioteca trabalha considerando o município como parte importante da configuração da integração.

O **código IBGE** é utilizado como uma das principais referências para identificação do município.

Exemplo:

```php
$municipio = '5201108'; // Anápolis/GO
```

ou:

```php
$municipio = '5208707'; // Goiânia/GO
```

---

# 🗺️ Municípios atendidos

Atualmente existem **16 municípios implementados** para Nota Control / ISSNET.

## 🇧🇷 AP — Amapá

| Município | Código IBGE | Provedor |
|---|---:|---|
| [Macapá](https://portalnotafacil.com.br/municipio-atendido/macapa-ap) | `1600303` | Nota Control / ISSNET |

## 🇧🇷 DF — Distrito Federal

| Município | Código IBGE | Provedor |
|---|---:|---|
| [Brasília](https://portalnotafacil.com.br/municipio-atendido/brasilia-df) | `5300108` | Nota Control / ISSNET |

## 🇧🇷 GO — Goiás

| Município | Código IBGE | Provedor |
|---|---:|---|
| [Anápolis](https://portalnotafacil.com.br/municipio-atendido/anapolis-go) | `5201108` | Nota Control / ISSNET |
| [Aparecida de Goiânia](https://portalnotafacil.com.br/municipio-atendido/aparecida-de-goiania-go) | `5201405` | Nota Control / ISSNET |
| [Goiânia](https://portalnotafacil.com.br/municipio-atendido/goiania-go) | `5208707` | Nota Control / ISSNET |

## 🇧🇷 MG — Minas Gerais

| Município | Código IBGE | Provedor |
|---|---:|---|
| [Itaúna](https://portalnotafacil.com.br/municipio-atendido/itauna-mg) | `3133808` | Nota Control / ISSNET |

## 🇧🇷 MT — Mato Grosso

| Município | Código IBGE | Provedor |
|---|---:|---|
| [Cuiabá](https://portalnotafacil.com.br/municipio-atendido/cuiaba-mt) | `5103403` | Nota Control / ISSNET |

## 🇧🇷 PA — Pará

| Município | Código IBGE | Provedor |
|---|---:|---|
| [Barcarena](https://portalnotafacil.com.br/municipio-atendido/barcarena-pa) | `1501303` | Nota Control / ISSNET |
| [Oriximiná](https://portalnotafacil.com.br/municipio-atendido/oriximina-pa) | `1505304` | Nota Control / ISSNET |

## 🇧🇷 RJ — Rio de Janeiro

| Município | Código IBGE | Provedor |
|---|---:|---|
| [Casimiro de Abreu](https://portalnotafacil.com.br/municipio-atendido/casimiro-de-abreu-rj) | `3301306` | Nota Control / ISSNET |
| [Duque de Caxias](https://portalnotafacil.com.br/municipio-atendido/duque-de-caxias-rj) | `3301702` | Nota Control / ISSNET |

## 🇧🇷 RS — Rio Grande do Sul

| Município | Código IBGE | Provedor |
|---|---:|---|
| [Cruz Alta](https://portalnotafacil.com.br/municipio-atendido/cruz-alta-rs) | `4306106` | Nota Control / ISSNET |
| [Santa Maria](https://portalnotafacil.com.br/municipio-atendido/santa-maria-rs) | `4316907` | Nota Control / ISSNET |

## 🇧🇷 SP — São Paulo

| Município | Código IBGE | Provedor |
|---|---:|---|
| [Dracena](https://portalnotafacil.com.br/municipio-atendido/dracena-sp) | `3514403` | Nota Control / ISSNET |
| [Ribeirão Preto](https://portalnotafacil.com.br/municipio-atendido/ribeirao-preto-sp) | `3543402` | Nota Control / ISSNET |
| [São Vicente](https://portalnotafacil.com.br/municipio-atendido/sao-vicente-sp) | `3551009` | Nota Control / ISSNET |

---

# 📊 Resumo

| UF | Municípios |
|---|---:|
| AP | 1 |
| DF | 1 |
| GO | 3 |
| MG | 1 |
| MT | 1 |
| PA | 2 |
| RJ | 2 |
| RS | 2 |
| SP | 3 |
| **Total** | **16** |

---

# 🇧🇷 Padrão Nacional da NFS-e

## Suporte completo

A `nfse-lib` está **totalmente pronta para o Padrão Nacional da NFS-e**.

O objetivo dessa implementação é permitir que sistemas possam trabalhar com uma estrutura nacional de NFS-e sem precisar espalhar regras de geração de XML, assinatura e comunicação fiscal pela aplicação principal.

A arquitetura contempla a separação entre:

```text
Dados da aplicação
        │
        ▼
      DTO
        │
        ▼
Regras fiscais
        │
        ▼
Geração XML
        │
        ▼
Assinatura Digital
        │
        ▼
Comunicação
        │
        ▼
NFS-e
```

---

# 📄 DPS — Declaração de Prestação de Serviço

A biblioteca possui estrutura específica para trabalhar com a **DPS — Declaração de Prestação de Serviço**.

Os dados fiscais podem ser organizados através de DTOs antes da geração do XML.

Exemplo conceitual:

```php
$dps = new DPSDataDTO([
    // Prestador
    // Tomador
    // Serviço
    // Valores
    // Tributação
    // Município
]);
```

Depois, a estrutura pode ser encaminhada ao componente responsável pela geração da DPS.

---

# 🧱 DTO — Data Transfer Object

A utilização de DTOs permite separar os dados fiscais da representação XML.

Isso evita que a aplicação tenha regras como:

```php
$xml->Prestador->CNPJ = $cnpj;
$xml->Tomador->CPF = $cpf;
$xml->Servico->Valor = $valor;
```

espalhadas por controllers e regras de negócio.

A ideia é trabalhar com:

```text
Application
     │
     ▼
    DTO
     │
     ▼
 NFSe Lib
     │
     ├── XML
     ├── Assinatura
     ├── Provedor
     └── Comunicação
```

---

# 🧾 Dados do prestador

A estrutura está preparada para informações como:

- CPF/CNPJ;
- inscrição municipal;
- regime tributário;
- Simples Nacional;
- endereço;
- município;
- códigos fiscais;
- informações tributárias.

---

# 👤 Dados do tomador

Podem ser tratados dados como:

- CPF;
- CNPJ;
- identificação estrangeira;
- nome/razão social;
- endereço;
- município;
- país;
- telefone;
- e-mail;
- informações complementares.

---

# 🛠️ Serviço

A estrutura pode contemplar informações relacionadas ao serviço prestado:

- código do serviço;
- código tributário;
- descrição;
- valor do serviço;
- descontos;
- deduções;
- município de incidência;
- tributação;
- retenções.

---

# 🌎 Tomador no exterior

A biblioteca está preparada para operações com **tomadores localizados no exterior**.

Podem ser representadas informações como:

- país;
- código do país;
- identificação estrangeira;
- nome/razão social;
- endereço no exterior;
- cidade;
- estado/província;
- código postal;
- informações de comércio exterior.

---

# 🌐 Comércio Exterior

A implementação do Padrão Nacional contempla estruturas necessárias para operações que envolvam **comércio exterior**.

Isso permite que aplicações possam diferenciar operações nacionais de operações envolvendo tomadores, endereços e informações internacionais.

---

# 🔐 Certificado Digital

As integrações que exigem certificado digital podem trabalhar com **certificado A1**, normalmente disponibilizado nos formatos:

```text
.pfx
.p12
```

Exemplo:

```php
$certificado = [
    'arquivo' => storage_path('certificados/certificado.pfx'),
    'senha'   => env('NFSE_CERTIFICADO_SENHA'),
];
```

### Segurança

**Nunca versione certificados digitais, senhas ou chaves privadas no Git.**

Utilize variáveis de ambiente:

```env
NFSE_CERTIFICADO_PATH=/certificados/certificado.pfx
NFSE_CERTIFICADO_SENHA=********
```

Recomenda-se também utilizar:

```gitignore
*.pfx
*.p12
*.pem
*.key
```

---

# 🔏 Assinatura Digital

A emissão de documentos fiscais pode exigir assinatura digital do XML.

A biblioteca possui estrutura para tratar a assinatura conforme as exigências do padrão utilizado.

Fluxo:

```text
Dados fiscais
     │
     ▼
Geração XML
     │
     ▼
XML
     │
     ▼
Assinatura Digital
     │
     ▼
XML Assinado
     │
     ▼
WebService
```

---

# 🔌 Comunicação com a Nota Control / ISSNET

A biblioteca concentra a comunicação com os serviços do provedor, abstraindo da aplicação detalhes como:

- SOAP;
- XML;
- namespaces;
- envelopes;
- headers;
- certificados;
- assinatura;
- endpoints;
- requisições;
- respostas;
- códigos de retorno;
- tratamento de erros.

---

# 🔄 Fluxo de emissão

Um fluxo típico pode ser representado por:

```text
┌─────────────────────────┐
│ Dados da empresa        │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│ Dados do tomador        │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│ Dados do serviço        │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│ Tributação              │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│ DPSDataDTO              │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│ Geração do XML          │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│ Assinatura Digital      │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│ Nota Control / ISSNET   │
└────────────┬────────────┘
             │
             ▼
┌─────────────────────────┐
│ Retorno da Prefeitura   │
└─────────────────────────┘
```

---

# 🧪 Homologação e Produção

## Homologação

O ambiente de homologação deve ser utilizado para:

- desenvolvimento;
- testes;
- validação do XML;
- testes de assinatura;
- testes de comunicação;
- validação dos dados;
- testes de emissão.

## Produção

O ambiente de produção é utilizado para emissão efetiva dos documentos fiscais.

> A disponibilidade e as características de cada ambiente dependem do município e do provedor.

---

# ⚠️ Particularidades municipais

Mesmo dentro da Nota Control / ISSNET, podem existir particularidades municipais.

Por isso, a biblioteca não deve considerar apenas o provedor, mas também o município.

Exemplo:

```text
Nota Control / ISSNET
        │
        ├── Anápolis
        │
        ├── Goiânia
        │
        ├── Cuiabá
        │
        ├── Brasília
        │
        └── demais municípios
```

Cada configuração deve respeitar as regras e características disponibilizadas pelo município.

---

# 🧪 Validação

Antes de utilizar uma integração em produção, recomenda-se validar:

- CPF/CNPJ;
- inscrição municipal;
- código IBGE;
- código do serviço;
- tributação;
- alíquotas;
- valores;
- retenções;
- dados do tomador;
- endereço;
- certificado;
- assinatura;
- XML;
- ambiente;
- comunicação com o provedor.

---

# 🔎 Tratamento de erros

A comunicação com serviços fiscais pode retornar diversos tipos de erro.

A aplicação deve estar preparada para tratar:

- erros de validação;
- erros de certificado;
- erros de assinatura;
- erros de comunicação;
- timeout;
- indisponibilidade;
- XML inválido;
- campos obrigatórios;
- códigos tributários inválidos;
- erros retornados pelo município;
- erros retornados pelo provedor.

Exemplo:

```php
try {

    $resultado = $nfse->emitir($dps);

} catch (\Throwable $e) {

    logger()->error('Erro na emissão da NFS-e', [
        'message' => $e->getMessage(),
    ]);

    throw $e;
}
```

---

# 📦 Instalação

A biblioteca utiliza o Composer.

```bash
composer require jcamelosti/nfse-lib
```

Ou através do código-fonte:

```bash
git clone https://github.com/jcamelosti/nfse-lib.git

cd nfse-lib

composer install
```

---

# 💻 Requisitos

Requisitos recomendados:

- PHP 8.1 ou superior;
- Composer;
- OpenSSL;
- DOM;
- XML;
- SOAP;
- cURL;
- certificado digital A1 quando exigido.

As extensões necessárias podem variar conforme o município, provedor e operação utilizada.

---

# 🏗️ Integração com Laravel

A biblioteca pode ser utilizada em aplicações Laravel.

Exemplo conceitual:

```php
use NfseLib\DTO\DPSDataDTO;
use NfseLib\Services\NfseService;

$dps = new DPSDataDTO([
    // dados da DPS
]);

$service = new NfseService();

$resultado = $service->emitir($dps);
```

Uma aplicação Laravel pode utilizar a `nfse-lib` como camada fiscal, mantendo as regras de negócio separadas da comunicação com os provedores de NFS-e.

---

# 🗂️ Arquitetura recomendada

Uma aplicação pode ser organizada da seguinte maneira:

```text
Laravel
│
├── Models
│   ├── Empresa
│   ├── Pessoa
│   ├── NotaEmitida
│   └── Certificado
│
├── DTO
│   └── DPSDataDTO
│
├── Services
│   └── NfseService
│
└── NFSe Lib
    ├── DTO
    ├── XML
    ├── Signer
    ├── Providers
    ├── NotaControl
    └── Nacional
```

---

# 🛠️ Adicionando novos municípios

A arquitetura permite expandir a biblioteca para novos municípios.

Para uma nova implementação normalmente são necessários:

1. Município;
2. UF;
3. código IBGE;
4. provedor;
5. documentação técnica;
6. URL de homologação;
7. URL de produção;
8. operações disponíveis;
9. regras de autenticação;
10. certificado digital;
11. estrutura XML;
12. regras de assinatura;
13. códigos de retorno;
14. testes de emissão;
15. testes de consulta;
16. testes de cancelamento.

---

# 🤝 Contribuições

Contribuições são bem-vindas.

Para contribuir:

```bash
git clone https://github.com/jcamelosti/nfse-lib.git

cd nfse-lib

composer install
```

Crie uma branch:

```bash
git checkout -b feature/novo-municipio
```

Faça as alterações, adicione os testes necessários e envie um Pull Request.

Ao adicionar um município, procure fornecer:

- município;
- UF;
- código IBGE;
- provedor;
- documentação;
- URL de homologação;
- URL de produção;
- operações disponíveis;
- exemplos de XML;
- exemplos de retorno;
- regras de assinatura;
- particularidades da integração.

---

# ⚠️ Responsabilidade fiscal

A `nfse-lib` é uma biblioteca de **integração tecnológica**.

A correta definição dos dados fiscais depende da operação realizada, da legislação aplicável e da situação tributária da empresa.

A biblioteca não substitui:

- contador;
- consultor tributário;
- legislação municipal;
- legislação federal;
- documentação oficial do município;
- orientação fiscal.

Os dados tributários devem ser definidos de acordo com a realidade de cada operação.

---

# 📚 Documentação

A documentação oficial do município, da Nota Control / ISSNET e do Padrão Nacional deve sempre ser considerada como referência para validação das integrações.

Os serviços fiscais podem sofrer alterações de:

- layout;
- endpoints;
- certificados;
- regras;
- schemas;
- métodos;
- autenticação;
- respostas.

Recomenda-se acompanhar as atualizações oficiais antes de realizar alterações em uma integração de produção.

---

# 📈 Roadmap

O projeto pode evoluir continuamente com:

- novos municípios;
- melhorias no Padrão Nacional;
- novos campos fiscais;
- novos métodos de consulta;
- cancelamento;
- substituição;
- consulta por RPS;
- consulta por NFS-e;
- melhorias de validação;
- melhorias na assinatura digital;
- novos testes automatizados;
- suporte a novos provedores quando necessário.

---

# ⭐ Por que utilizar a NFSe Lib?

A principal vantagem da biblioteca é concentrar a complexidade da integração fiscal em uma camada específica.

### Sem a biblioteca

```text
ERP
 │
 ├── SOAP
 ├── XML
 ├── Assinatura
 ├── Certificado
 ├── ISSNET
 ├── Regras municipais
 ├── Tratamento de erros
 └── Padrão Nacional
```

### Com a biblioteca

```text
ERP
 │
 ▼
NFSe Lib
 │
 ├── Nota Control / ISSNET
 │
 └── Padrão Nacional
```

Isso permite que o sistema principal permaneça mais simples, organizado e desacoplado das particularidades da integração fiscal.

---

# 🏆 Cobertura atual

## Nota Control / ISSNET

**16 municípios implementados**

- 🇧🇷 AP — 1
- 🇧🇷 DF — 1
- 🇧🇷 GO — 3
- 🇧🇷 MG — 1
- 🇧🇷 MT — 1
- 🇧🇷 PA — 2
- 🇧🇷 RJ — 2
- 🇧🇷 RS — 2
- 🇧🇷 SP — 3

## Padrão Nacional da NFS-e

**✅ Implementação pronta**

---

# 📞 Suporte técnico

Para informações técnicas, implantação, customizações e desenvolvimento de novas integrações:

**E-mail:** contato@josuecamelo.com

**WhatsApp:** (62) 98401-8589

---

# 💼 Integração personalizada

Caso sua empresa necessite integrar um município ainda não disponível, entre em contato para avaliação da implementação.

Podem ser desenvolvidas integrações personalizadas para:

- ERP;
- sistemas financeiros;
- plataformas SaaS;
- sistemas contábeis;
- emissão de NFS-e;
- integração com APIs;
- integração SOAP;
- certificado digital;
- automação fiscal;
- Padrão Nacional;
- novos municípios;
- novos provedores.

---

# 📄 Licença

Consulte o arquivo [`LICENSE`](LICENSE) deste repositório para obter informações sobre os termos de utilização e distribuição.

---

# ⭐ Apoie o projeto

Se a `nfse-lib` foi útil para seu projeto, considere deixar uma ⭐ no GitHub.

Contribuições, sugestões, correções e novas implementações são bem-vindas.

---

**NFSe Lib**

Biblioteca PHP para integração de NFS-e com **Nota Control / ISSNET** e **Padrão Nacional da NFS-e**.

Desenvolvido por **Josué Camelo**.
