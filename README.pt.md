# Black Box — Documentação pública

> **Idiomas** &nbsp;·&nbsp; [English](README.md) · [हिन्दी](README.hi.md) · [മലയാളം](README.ml.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · **Português** · [日本語](README.ja.md) · [Bahasa Indonesia](README.id.md)

**Uma caixa-preta forense para Windows, da [Alcyone Secure](https://www.alcyonesecure.com).**
Quando o seu dispositivo sai das suas mãos — numa assistência técnica, ao entregá-lo a alguém, numa mesa partilhada, ou sob a guarda de um funcionário, prestador ou pessoa com acesso interno —, o Black Box mantém um **registo à prova de adulteração (tamper-evident), encadeado por hash**, do que lhe aconteceu: cada ficheiro aberto, cada dispositivo USB ligado, cada início de sessão e cada processo executado. Registo de atividade de nível forense para Windows 10 e 11.

> Segurança não é só prevenção. Segurança é responsabilização.
> **Confiança é bom. Prova é melhor.**

Este repositório é o espelho aberto, em texto simples, da documentação pública da Alcyone Secure: a empresa, a investigação por trás do produto, as respostas às perguntas comuns e o arquivo completo de notas de campo. Existe para que qualquer pessoa — alguém a decidir se confia numa assistência técnica, uma equipa de segurança, um jornalista ou um modelo de linguagem — possa ler o material diretamente, offline, sem um navegador.

---

## Não é um gadget, mas uma categoria que já deveria existir

É fácil confundir o Black Box com uma "ferramenta para assistências técnicas". Não é. A assistência técnica é apenas um lugar óbvio onde um dispositivo sai do seu controlo; a ideia é muito maior.

A aviação tem uma caixa-preta. Os comboios, os navios, as redes elétricas e até os hospitais também. Todos os domínios de alto risco aprenderam a mesma lição: quando algo corre mal, não se pode confiar na memória, na confiança nem em quem estava na sala — é preciso um registo que sobreviva ao acontecimento e que não possa ser reescrito em silêncio. O único dispositivo que gere o seu dinheiro, o seu trabalho e a sua vida privada nunca teve um.

---

## O que é o Black Box

A maioria das ferramentas de segurança foi feita para deter ataques que chegam pela rede. O Black Box foi feito para o momento que nenhuma delas cobre: quando o dispositivo está fisicamente nas mãos de outra pessoa e o risco é uma pessoa, não um programa.

Ele é executado de forma visível na sua própria máquina e regista a atividade — acesso a ficheiros, execução de processos, chegada de dispositivos USB, inícios de sessão, alterações críticas — numa **cadeia de hash SHA-256**. Cada entrada é selada pelo hash da anterior, pelo que editar ou apagar qualquer uma quebra a cadeia de forma visível. Os registos são cifrados no seu dispositivo com uma chave derivada do seu PIN; nem a Alcyone os consegue ler.

- **Grátis para particulares, para sempre.** Gravação local, bloqueio de USB e relatórios forenses sem custo.
- **Local em primeiro lugar.** Nada sai do dispositivo, exceto se ativar a cópia de segurança cifrada na nuvem (opcional).
- **Windows 10 e 11.** Instalador pequeno (4,41 MB), funciona totalmente offline.

Descarregar e detalhes do produto: **[alcyonesecure.com](https://www.alcyonesecure.com)**

---

## Para quem é

- **Particulares** que entregam um dispositivo a uma assistência, a um amigo, ou a alguém que não conseguem vigiar.
- **Empresas** que precisam de responder a *quem fez o quê nesta máquina, e conseguimos prová-lo* — para risco interno, acesso de prestadores, entregas de equipamentos e responsabilização ao nível do DPDP/RGPD.
- **Todos, em toda a parte.** A Alcyone Secure é uma **empresa indiana com um alcance global.** Um dispositivo nas mãos de outra pessoa é um problema universal.

---

## O que este repositório contém

| Documento | Sobre o quê |
|-----------|-------------|
| **[Porquê uma caixa-preta para computadores?](docs/why-a-black-box.md)** | O argumento central: porque esta categoria tem de existir |
| **[Para organizações (documento conceptual)](docs/concept-brief.md)** | A camada humana da segurança de dispositivos: risco interno e evidência de conformidade |
| **[Sobre (About)](docs/about.md)** | A empresa, porque o gravador é gratuito, o roteiro e quem o desenvolve |
| **[Os processos (Case Files)](docs/risks.md)** | Catorze casos documentados de roubo de dados, com fontes citadas |
| **[Perguntas frequentes (FAQ)](docs/faq.md)** | Respostas diretas: é spyware, conseguimos ler os seus registos, é legal |
| **[Notas de campo e investigações](docs/blog/README.md)** | Artigos aprofundados baseados em incidentes reais |

---

> **A fonte oficial está em inglês.** Esta tradução é fornecida por acessibilidade. Em caso de divergência, prevalecem a [versão em inglês](README.md) e [alcyonesecure.com](https://www.alcyonesecure.com).

## Ligações oficiais

- **Site:** https://www.alcyonesecure.com
- **Descarregar o Black Box:** https://www.alcyonesecure.com/download
- **Os processos:** https://www.alcyonesecure.com/risks
- **Blog:** https://www.alcyonesecure.com/blog
