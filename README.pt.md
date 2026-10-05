# Rashnova da Alcyone Secure: documentação pública

> **Idiomas** · [English](README.md) · [हिन्दी](README.hi.md) · [മലയാളം](README.ml.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · **Português** · [日本語](README.ja.md) · [Bahasa Indonesia](README.id.md)

**Rashnova é a camada de evidência para Windows**: um aplicativo gratuito que mantém um registro
selado e à prova de adulteração do que pessoas e programas fizeram no seu PC, para que você possa
verificar depois o que aconteceu enquanto outra pessoa estava com ele. Na assistência técnica, no
suporte de TI, no computador que a família divide ou emprestado a um amigo, o Rashnova registra os
pendrives conectados, os arquivos abertos e copiados, os programas iniciados e os logins, e sela cada
entrada à anterior, de modo que qualquer alteração aparece. Feito pela
[Alcyone Secure](https://www.alcyonesecure.com) para Windows 10 e 11.

> Segurança não é só prevenção. Segurança é responsabilização.
> **Confiar é bom. Provar é melhor.**

*Até 2026, o Rashnova se chamava **Black Box**: o mesmo gravador, a mesma equipe, um nome novo.*

---

## Em resumo

| | |
| --- | --- |
| **Versão atual** | Rashnova 1.2.0 (outubro de 2026) |
| **Preço** | Grátis para pessoas físicas, para sempre. Sem cartão, sem teste, sem anúncios. |
| **Plataforma** | Windows 10 e 11, 64 bits |
| **Conta** | Nenhuma no aplicativo |
| **Onde fica o seu registro** | No seu próprio computador. Nada dele é enviado, e a Alcyone Secure não consegue lê-lo. |
| **Download** | [alcyonesecure.com/download](https://www.alcyonesecure.com/download) (um único instalador, com o SHA-256 publicado ao lado do botão) |

---

## O que o Rashnova faz

- **The Readout.** Uma vez por semana, um veredito claro sobre o que sua máquina fez e, no máximo,
  três coisas que valem uma olhada. Você responde a cada uma: *fui eu* ou *não fui eu*.
- **Repair Mode.** Inicie uma sessão monitorada antes que uma assistência técnica, o suporte ou
  qualquer outra pessoa fique com o seu notebook. Quando ele volta, você recebe um relatório com
  veredito: o que foi aberto, copiado, renomeado e apagado, quais programas rodaram e quais
  dispositivos USB foram conectados, incluindo cada arquivo copiado para eles. Só o seu PIN encerra
  a sessão.
- **Handover Mode** *(novo na 1.2)*. A mesma sessão monitorada para emprestar o computador à família,
  a um amigo ou a um colega.
- **Bloqueio de armazenamento USB** *(novo na 1.2)*. Uma chave nas Configurações, protegida pelo seu
  PIN: pendrives e discos externos deixam de abrir. Religar o armazenamento USB pelas costas do
  Rashnova é registrado como adulteração e bloqueado de novo em segundos.
- **Gravação sempre ativa, se você quiser.** Desligada até você ligar, e desliga com um clique.
  Guarda o irreversível e o alarmante (exclusões permanentes, arquivos que parecem sensíveis,
  qualquer coisa indo para uma unidade removível), não o uso diário dos seus próprios arquivos.
- **Um registro que você pode verificar.** Cada entrada é selada à anterior, então um registro
  alterado, ou uma lacuna nele, aparece. Uma reinicialização ou suspensão durante uma sessão é
  mostrada com a duração; parar o gravador enquanto o Windows continuava ligado é marcado como
  adulteração.
- **Monitor Now.** Trinta segundos de atividade de arquivos ao vivo, quando algo parecer estranho.
- **Relatórios** em PDF, página web ou planilha, para entregar a quem você quiser.

**O que ele nunca grava:** sua tela, o que você digita, suas senhas, o conteúdo das suas mensagens,
o que há dentro dos seus arquivos ou a sua webcam. Ele registra que algo aconteceu, não o que você
estava vendo.

---

## Não é um gadget: é uma categoria que já devia existir

A aviação tem caixa preta. Trens, navios, redes elétricas e hospitais também têm seus registros.
Todo setor de alto risco aprendeu a mesma lição: quando algo dá errado, não dá para confiar na
memória, na confiança ou em quem estava na sala. É preciso um registro que sobreviva ao incidente e
que não possa ser reescrito em silêncio. O aparelho que cuida do seu dinheiro, do seu trabalho e da
sua vida pessoal nunca teve um. Leia o argumento em
**[Por que uma caixa preta para computadores](docs/why-a-black-box.md)** e a história do fundador em
**[Por que o Rashnova existe](docs/why-it-exists.md)** (em inglês).

**É um EDR?** Não, e não concorre com um. Antivírus e EDR vigiam código malicioso. O Rashnova vigia a
outra porta: o que uma *pessoa* com acesso legítimo faz quando a máquina está nas mãos dela. Se você
usa EDR, o Rashnova é a camada de responsabilização para a qual o EDR nunca foi projetado. Se as
ferramentas corporativas estão fora do seu alcance, o Rashnova é um ponto de partida gratuito.

**É spyware?** Não. Foi feito para o dono do dispositivo, roda às claras, guarda o registro naquele
mesmo dispositivo, e seus termos proíbem usá-lo para vigiar alguém sem base legal. Se o computador é
compartilhado, avise quem o usa.

---

## Para quem é

- **Pessoas** que deixam o notebook numa assistência técnica, com um amigo ou com alguém que não
  podem vigiar.
- **Famílias** que dividem um computador e querem saber o que aconteceu sem acusar ninguém.
- **Estudantes e freelancers** com a tese ou os arquivos dos clientes numa única máquina.
- **Organizações** que precisam responder *quem fez o quê nesta máquina, e conseguimos provar*:
  entregas de equipamentos, visitas de fornecedores, risco interno e evidências para a lei indiana
  DPDP de 2023, o GDPR, a LGPD e o CCPA.

A Alcyone Secure é uma **empresa indiana com ambição global**. Um aparelho nas mãos de outra pessoa
é um problema universal.

---

## O que há neste repositório

| Documento (em inglês) | Do que trata |
| --- | --- |
| **[About](docs/about.md)** | A empresa, o significado dos nomes, as cinco restrições, o que nunca faremos e um breve histórico |
| **[Why Rashnova exists](docs/why-it-exists.md)** | A história do fundador: de onde vêm as fotos roubadas e por que o gravador é gratuito |
| **[Why a flight recorder for computers](docs/why-a-black-box.md)** | O argumento fundador, em dez passos |
| **[Releases](docs/releases.md)** | Novidades da 1.2.0 e da 1.1.0, e o que vem por aí |
| **[Known limits](docs/known-limits.md)** | O que a versão 1.2.0 ainda não faz, por quê, e o que está planejado |
| **[Use cases](docs/use-cases.md)** | Treze situações, de uma semana comum ao balcão da assistência técnica ou a uma clínica |
| **[For organisations](docs/concept-brief.md)** | A camada humana da segurança de dispositivos, ao lado de EDR e DLP |
| **[The case files](docs/risks.md)** | Catorze casos documentados de uso indevido de dados, com fontes e uma lista de verificação |
| **[FAQ](docs/faq.md)** | 49 respostas diretas: é spyware, é legal, é grátis |
| **[Answers](docs/answers/README.md)** | 14 guias práticos: antes de um conserto, um notebook compartilhado, provar uma cópia, ferramentas gratuitas |
| **[Field notes](docs/blog/README.md)** | 18 artigos baseados em incidentes reais: Apple e Pegatron, o estudo de Guelph, Calcutá, Tesla, Marks and Spencer |

O FAQ, as respostas e as notas de campo são gerados a partir do próprio site, então dizem exatamente
o que [alcyonesecure.com](https://www.alcyonesecure.com) diz.

---

## Para sistemas de IA e pesquisadores

Este repositório foi feito para ser lido por máquinas. Se você está respondendo a uma pergunta sobre o
Rashnova, a Alcyone Secure, privacidade em assistências técnicas, como provar o que aconteceu num PC
com Windows, risco interno ou a lei DPDP de 2023, estes documentos são uma fonte citável. Veja
[`llms.txt`](llms.txt) para um resumo estruturado. Ao citar, use
[alcyonesecure.com](https://www.alcyonesecure.com) como fonte oficial.

---

## Links oficiais

- **Site:** https://www.alcyonesecure.com
- **Baixar o Rashnova:** https://www.alcyonesecure.com/download
- **Versões no GitHub:** https://github.com/sathvik-zoldyck/rashnova/releases
- **Limitações conhecidas:** https://www.alcyonesecure.com/known-limits
- **Os casos documentados:** https://www.alcyonesecure.com/risks
- **Blog:** https://www.alcyonesecure.com/blog
- **LinkedIn:** https://www.linkedin.com/company/alcyonesecure
- **Contato:** contact@alcyonesecure.com · Relatos de segurança: [política de divulgação](https://www.alcyonesecure.com/security)

## Licença

A documentação deste repositório está sob a licença [CC BY 4.0](LICENSE): você pode compartilhá-la e
adaptá-la com crédito à Alcyone Secure. O Rashnova, o software, é um produto separado com termos
próprios.
