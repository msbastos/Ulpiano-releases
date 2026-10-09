# Ulpiano — instalador para Windows

Instalador do **Ulpiano**, que prepara o dossiê de decisão a partir do PDF dos autos (PJe) e o leva ao Claude para a minuta. Desenvolvido e mantido pelo Juiz do Trabalho Maurício Schmidt Bastos (TRT4).

**Baixar:** [Ulpiano-Setup.exe](https://github.com/msbastos/Ulpiano-releases/releases/latest/download/Ulpiano-Setup.exe) (uns 140 MB; sempre a versão mais recente). Para conferir o arquivo, compare o SHA-256 com o `SHA256SUMS.txt` da [página da release](https://github.com/msbastos/Ulpiano-releases/releases/latest).

Este repositório só distribui as versões liberadas. O desenvolvimento acontece em outro lugar. O programa é software livre (AGPL-3.0); o código-fonte Python segue dentro do próprio instalador, na pasta de instalação, junto do `LICENSE` e dos créditos.

---

# Ulpiano — manual de instalação

Este manual é para quem vai instalar o Ulpiano no próprio computador. Não
exige conhecimento de informática: cada tela do instalador é descrita pelo
que ela diz.

## 1. O que você precisa

- **Windows 10 ou 11**, de 64 bits (qualquer computador dos últimos anos).
- Uma **assinatura paga do Claude** (Pro, Max, Team ou Enterprise), com o uso
  dos seus dados em treinamento desligado.
- Para a leitura das páginas digitalizadas dos autos pela Mistral, uma
  **conta na Mistral** com pagamento por uso e a coleta de dados desligada.
  O Ulpiano explica como, na hora certa.
- Internet só para baixar o instalador e, se você quiser, o Claude Code.

**Você não precisa de administrador** e não precisa instalar mais nada: o
instalador já traz tudo o que o Ulpiano usa.

## 2. Baixar

O link que você recebeu abre a página do instalador. Clique em
**`Ulpiano-Setup.exe`** (uns 140 MB). O navegador pode avisar que "este
arquivo não é baixado com frequência": escolha **manter** o arquivo.

## 3. Abrir o instalador

Dê um duplo clique no arquivo baixado.

Se o Windows mostrar **"O Windows protegeu o computador"**, não é defeito: o
aviso aparece porque o instalador ainda não tem assinatura de editor, e o
Windows desconfia de todo programa novo. Clique em **Mais informações** e,
depois, em **Executar assim mesmo**.

## 4. As telas do instalador

1. **Boas-vindas.** Diz que o Ulpiano prepara o dossiê de decisão a partir do
   PDF dos autos e o leva ao seu Claude; que será instalado só para você,
   sem precisar de administrador; e que nada é baixado da internet agora,
   exceto o Claude Code, se você marcar a opção. Clique em **Avançar**.
2. **Licença.** O resumo, em português, da licença do programa (AGPL-3.0).
   Para continuar, aceite-a.
3. **Aviso de proteção dos dados.** Leia com atenção: o aviso diz o que sai
   do computador (trechos dos autos com os nomes trocados por códigos e, na
   leitura pela Mistral, as imagens das páginas digitalizadas) e o que a sua
   assinatura precisa garantir. Marque **Li e estou ciente** e avance. Sem a
   marca, o instalador não segue.
4. **Claude Code.** O Claude Code, da Anthropic, é o ajudante que escreve as
   minutas sozinho, com a sua assinatura paga do Claude. A caixa **"Baixar e
   instalar o Claude Code agora"** já vem marcada (leva uns 2 minutos e
   precisa de internet). Desmarque se não quiser agora ou se estiver sem
   internet; sem ele, você copia um pedido curto e cola no aplicativo Claude,
   o fluxo de sempre. Esta é a única coisa que o instalador baixa da
   internet. Se o Claude Code já estiver instalado, esta tela não aparece.
5. **Atalhos.** **Criar um atalho na Área de Trabalho** (opcional).
6. **Pronto para instalar.** Um resumo das suas escolhas. Clique em
   **Instalar**.
7. **Instalando.** Os arquivos são copiados (um minuto ou pouco mais; se você
   marcou o Claude Code, a tela diz "Baixando e instalando o Claude Code").
8. **Final.** O Ulpiano está instalado. A caixa **Abrir o Ulpiano agora**
   vem marcada; clique em **Concluir**.

## 5. Primeiros passos

Ao abrir, o Ulpiano aparece no navegador, numa janela só dele, e conduz os
**Primeiros passos**, na ordem:

1. **Gabinete** — o nome e a região, que dão título aos seus Entendimentos.
2. **Pastas** — onde ficam os autos, o acervo e a Pasta do Claude (a tela
   explica as regras dessa última). Com os campos em branco, a tela sugere
   as pastas `Processos_Novos`, `Acervo` e `Claude` no disco do Windows
   (mais a pasta Downloads do Windows, que continua como está): **Usar estas
   pastas** cria as que ainda não existem e preenche os campos; só o
   **Continuar** grava.
3. **Ciência** — o aviso de proteção dos dados. Como você já deu a ciência
   no instalador, este passo mostra **"Ciência registrada"**; clique em
   **Continuar**.
4. **Leitura dos autos** — a chave da Mistral, testada e guardada com
   segurança no Gerenciador de Credenciais do Windows.
5. **Claude** — as quatro skills que você envia à sua conta do Claude e, se
   não o instalou antes, o botão **Instalar o Claude Code**.
6. **Entendimentos** — como você quer as minutas: agora ou depois.
7. **Tudo pronto** — o ciclo de cada processo, em seis passos.

Leva uns 10 minutos, e cada passo fica guardado ao avançar: dá para parar e
continuar depois, abrindo o Ulpiano pelo atalho ou pelo menu Iniciar.

## 6. Se algo der errado

- **Apareceu "Ulpiano - nota para a TI.txt" na Área de Trabalho.** O Windows
  da sua rede barrou o programa (é uma regra de segurança do tribunal ou da
  empresa, não um defeito). Envie o arquivo à equipe de TI; ele diz o que
  liberar. Depois da liberação, abra o Ulpiano pelo atalho.
- **"O Claude Code não pôde ser instalado agora."** O Ulpiano funciona sem
  ele. Para tentar de novo, use **Primeiros passos › Claude › Instalar o
  Claude Code**.
- **Precisa de ajuda.** Depois de concluir os Primeiros passos, abra a página
  **Sobre** e clique em **Gerar pacote de diagnóstico** (o botão só existe
  a partir daí). Ele cria um arquivo `.zip`, sem chaves, sem números de
  processo e sem o seu nome de usuário. Envie-o a quem dá suporte.

## 7. Atualizar

Quando houver versão nova, uma faixa no alto do Ulpiano avisa e traz o link.
Baixe o novo `Ulpiano-Setup.exe` e rode-o **com o Ulpiano fechado**. As suas
configurações e os seus Entendimentos ficam.

## 8. Desinstalar

Abra as configurações do Windows, vá em **Aplicativos**, escolha **Ulpiano**
e clique em **Desinstalar** (ou use o atalho **Desinstalar o Ulpiano** do
menu Iniciar). O desinstalador pergunta se deve apagar também as
configurações, os Entendimentos, os registros e as chaves; as pastas dos
processos (caixa, acervo e Pasta do Claude) nunca são apagadas.

## 9. Onde fica cada coisa

| O quê | Onde |
|---|---|
| O programa | `%LOCALAPPDATA%\Programs\Ulpiano` |
| Configurações, registros e Entendimentos | `%LOCALAPPDATA%\Ulpiano` |
| As chaves (Mistral e outras) | Gerenciador de Credenciais do Windows |
| Os processos | nas pastas que você escolheu nos Primeiros passos |
