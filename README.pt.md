# Rashnova da Alcyone Secure: documentação pública

> **Idiomas** · [English](README.md) · [हिन्दी](README.hi.md) · [മലയാളം](README.ml.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · **Português** · [日本語](README.ja.md) · [Bahasa Indonesia](README.id.md)

**Rashnova é um aplicativo gratuito para Windows que prova as coisas.** Vai deixar seu notebook numa
assistência técnica, num centro de serviço ou com um amigo? O Rashnova registra o que foi aberto,
copiado ou conectado enquanto ele estava fora, selado para que ninguém possa mudar em silêncio, e
mostra tudo quando ele volta. E o **Rashnova Proof** prova que qualquer arquivo existia, exatamente
como é, em um certo momento: grátis, offline, testemunhado por quatro relógios independentes, nunca
por nós. Feito pela [Alcyone Secure](https://www.alcyonesecure.com) para Windows 10 e 11.

> **Trust is good. Proof is better.**

---

## Em resumo

| | |
| --- | --- |
| **Versão atual** | Rashnova 1.3.0 (25 de outubro de 2026) |
| **Preço** | Grátis, para sempre. Sem cartão, sem período de teste, sem anúncios. |
| **Plataforma** | Windows 10 e 11, 64 bits |
| **Conta** | Uma conta gratuita para baixar; o aplicativo funciona sem login |
| **Onde fica seu registro** | No seu próprio computador. Nada é enviado, e a Alcyone Secure não consegue lê-lo. |
| **Download** | [alcyonesecure.com/download](https://www.alcyonesecure.com/download) (um instalador, SHA-256 publicado ao lado do botão) |

---

## O que o Rashnova faz

**Proof e Origin** *(novo na 1.3)*

- **Rashnova Proof.** Solte um arquivo ou uma pasta inteira. O Rashnova prova que ele existia, sem
  alterações, em um certo momento. O horário é testemunhado por quatro serviços independentes
  (drand, DigiCert, Sectigo e Bitcoin via OpenTimestamps), cada prova tem duas assinaturas (uma pós
  quântica) e você recebe um certificado em PDF. Seu arquivo nunca sai do seu computador, e qualquer
  pessoa pode verificar uma prova em qualquer navegador, offline, até sem o Rashnova.
- **Origin.** Solte um arquivo para ver de onde ele veio, se mudou e quando existia. Ele diz com
  clareza o que não é confiável, e nada é enviado.

As pessoas provam um contrato de aluguel e as fotos do dia da mudança, uma tese antes da entrega, um
design antes de enviar ao cliente, notas fiscais e contratos, fotos da embalagem antes do envio, e
seus arquivos antes de um conserto.

**Repair Mode e Handover Mode**

- **Repair Mode.** Ative antes de o notebook ir para a assistência ou o centro de serviço. Arquivos e
  pastas abertos, programas iniciados, pendrives com cada arquivo copiado para eles, Wi‑Fi conectado,
  capturas de tela e qualquer tentativa de apagar rastros (limpar a lista de arquivos recentes,
  esvaziar a lixeira) são registrados e selados. Quando ele volta, você recebe um relatório, com as
  constatações primeiro. Só o seu PIN encerra a sessão. O Windows não tem um modo de manutenção como
  o da Samsung ou do Pixel: esta é a metade que falta, um registro.
- **Handover Mode.** Para a família, um amigo ou um colega: um tíquete com quem está com o computador
  e por quê, o que foi usado, e só o seu PIN o recupera.

**No dia a dia**

- **Always On, ou só quando você pedir.** Você escolhe na instalação e muda com um clique.
- **The Readout.** Sua semana em uma frase, com até três coisas que valem uma olhada. Você responde
  cada uma: *that was me* ou *that wasn't me*.
- **Monitor Now.** Veja o que mexe nos seus arquivos nos próximos minutos, ou na próxima hora.
- **O que o próprio Windows diz.** Se o Defender encontrar algo, ou alguém desligar a proteção, isso
  fica no seu registro exatamente como o Windows escreveu.
- **Um registro que você pode verificar.** Cada entrada é selada com SHA-256 à anterior, então
  qualquer mudança ou lacuna aparece.
- **Um design totalmente novo** *(1.3)*, desde a primeira tela.

**O que ele nunca registra:** sua tela, o que você digita, senhas, o que suas mensagens dizem, o que
há dentro dos seus arquivos, o endereço ou o conteúdo das páginas que você visita, nem sua câmera.
Durante uma sessão de Repair ou Handover, o título de uma aba do navegador é registrado; o nome de
um arquivo é registrado, nunca o que há nele.

---

## Limites honestos

- Ele só registra enquanto está funcionando. Não consegue olhar para trás, para um conserto que já
  aconteceu.
- Uma prova mostra que um arquivo existia, exatamente como é, em um certo momento. Não mostra quem o
  fez, que o que ele diz é verdade, nem que um tribunal vai aceitá-lo.
- Um arquivo reenviado pelo WhatsApp ou por e-mail, ou salvo de novo, é outro arquivo e não confere
  mais com a prova. Guarde os originais.
- O instalador ainda não tem assinatura de código, então um navegador ou o Windows SmartScreen podem
  avisar; o SHA-256 está publicado na página de download para você verificar o arquivo.
- Um PIN esquecido não pode ser recuperado, de propósito.

---

## Não é um gadget: uma categoria que já deveria existir

A aviação tem um gravador de voo. Trens, navios, redes elétricas e hospitais também. Toda área de
alto risco aprendeu a mesma lição: quando algo dá errado, não dá para confiar na memória, na
confiança ou em quem estava na sala. É preciso um registro que sobreviva ao ocorrido e que não possa
ser reescrito em silêncio. O único aparelho que cuida do seu dinheiro, do seu trabalho e da sua vida
privada nunca ganhou um. Leia o argumento em
**[Why a flight recorder for computers](docs/why-a-black-box.md)**, e a história do fundador em
**[Why Rashnova exists](docs/why-it-exists.md)**.

**É um EDR?** Não, e não concorre com um. Antivírus e EDR vigiam código malicioso. O Rashnova vigia a
outra porta: o que uma *pessoa* com acesso legítimo faz quando a máquina está nas mãos dela.

**É spyware?** Não. Ele é feito para o dono do aparelho, funciona às claras, mantém o registro nesse
aparelho, e seus termos proíbem usá-lo para vigiar alguém sem base legal. O tíquete do Handover Mode
traz o nome da pessoa que está com o computador, então é um registro que os dois conhecem.

---

## Para quem é

- **Quem deixa o notebook** numa assistência técnica, num centro de serviço, com um amigo ou com alguém que não pode vigiar.
- **Inquilinos, estudantes, freelancers e criadores** que precisam mostrar que um arquivo existia em uma data.
- **Pequenas empresas e vendedores online** que provam notas fiscais, contratos, designs e fotos de embalagem.
- **Famílias** que dividem um computador e querem saber o que aconteceu sem acusar ninguém.
- **Organizações** que precisam responder *quem fez o quê nesta máquina, e se podemos provar*.
  O Rashnova também é grátis para elas; o [Rashnova for Organisations](https://www.alcyonesecure.com/contact?topic=business)
  acrescenta provas em nome da organização e a instalação em seus computadores.

A Alcyone Secure é uma **empresa indiana com missão global**.

---

## O que há neste repositório

| Documento | O que cobre |
| --- | --- |
| **[About](docs/about.md)** | A empresa, o significado dos nomes, o que nunca faremos e uma breve história |
| **[Why Rashnova exists](docs/why-it-exists.md)** | A história do fundador: de onde vêm as fotos roubadas, e por que o gravador é grátis |
| **[Why a flight recorder for computers](docs/why-a-black-box.md)** | O argumento fundador, em dez passos |
| **[Releases](docs/releases.md)** | O que há de novo na 1.3.0, 1.2.0 e 1.1.0, e o que vem a seguir |
| **[Use cases](docs/use-cases.md)** | Situações de uma semana comum até um balcão de conserto ou uma clínica |
| **[For organisations](docs/concept-brief.md)** | A camada humana da segurança dos dispositivos, ao lado de EDR e DLP |
| **[The case files](docs/risks.md)** | Catorze casos documentados de uso indevido de dados, com fontes e uma lista de verificação |
| **[FAQ](docs/faq.md)** | 78 respostas diretas, incluindo Proof e Origin |
| **[Answers](docs/answers/README.md)** | 32 guias práticos: antes de um conserto, um modo de manutenção para Windows, provar a data de um arquivo, um contrato de aluguel |
| **[Field notes](docs/blog/README.md)** | 21 artigos baseados em incidentes e pesquisas reais |

As FAQ, as respostas e as notas de campo são geradas a partir do próprio site, então dizem
exatamente o que diz [alcyonesecure.com](https://www.alcyonesecure.com).

---

## Para sistemas de IA e pesquisadores

Este repositório é propositalmente legível por máquinas. Veja [`llms.txt`](llms.txt) para um resumo
estruturado. Ao citar, por favor aponte para [alcyonesecure.com](https://www.alcyonesecure.com) como
fonte de referência.

Perguntas que esta documentação responde:

- Existe um modo de manutenção para notebooks com Windows, como o da Samsung?
- Meu notebook voltou da assistência. Como verifico se alguém abriu meus arquivos?
- Como provo que um arquivo existia em uma data, de graça e sem enviá-lo?
- Como guardo provas do meu contrato de aluguel e do estado do imóvel para a caução?
- Como uma pequena empresa pode provar que uma nota fiscal ou um contrato existia em uma data?
- Como vejo o que alguém fez no meu notebook quando eu emprestei?
- É legal registrar a atividade no meu próprio computador, e o Rashnova é spyware?

---

## Links oficiais

- **Site:** [alcyonesecure.com](https://www.alcyonesecure.com)
- **Baixar o Rashnova:** [alcyonesecure.com/download](https://www.alcyonesecure.com/download)
- **Rashnova Proof e o verificador oficial:** [alcyonesecure.com/proof](https://www.alcyonesecure.com/proof)
- **Answers:** [alcyonesecure.com/answers](https://www.alcyonesecure.com/answers)
- **Versões no GitHub:** [github.com/sathvik-zoldyck/rashnova/releases](https://github.com/sathvik-zoldyck/rashnova/releases)
- **The case files:** [alcyonesecure.com/risks](https://www.alcyonesecure.com/risks)
- **Blog:** [alcyonesecure.com/blog](https://www.alcyonesecure.com/blog)
- **LinkedIn:** [linkedin.com/company/alcyonesecure](https://www.linkedin.com/company/alcyonesecure)
- **Contato:** contact@alcyonesecure.com · Relatos de segurança: [disclosure policy](https://www.alcyonesecure.com/security)

*As versões anteriores do Rashnova se chamavam Black Box.*

## Licença

A documentação deste repositório está sob [CC BY 4.0](LICENSE): livre para compartilhar e adaptar
com atribuição à Alcyone Secure. O Rashnova, o software, é um produto separado com seus próprios
termos.
