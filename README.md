# Guia de Clãs — LimboMC

Tudo sobre clãs começa com **`/clan`**. Esse comando abre um **menu** onde dá para fazer quase tudo com cliques.
Os comandos abaixo são os mesmos que o menu usa. *(Valores como custos, tempos e limites são os padrões e a staff pode ajustar.)*

---

## 1. Começando

### Criar seu clã
```
/clan criar <nome> <tag>
```
Exemplo: `/clan criar Fenix FNX`
- **Nome:** 3 a 16 letras, números ou `_`.
- **Tag:** 2 a 5 letras ou números (aparece ao lado do nome).
- Nomes e tags não podem repetir, nem conter palavras proibidas.
- Se você saiu ou dissolveu um clã, há uma espera (padrão: 1 hora) para criar outro.

### Entrar em um clã
Um líder ou membro autorizado te convida. Você recebe uma mensagem clicável, e o convite **vale por 2 minutos**:
```
/clan aceitar <clã>        (ou clique na mensagem)
/clan recusar <clã>
/clan convites             (lista seus convites no menu)
```

### Ver informações
```
/clan info            seu clã
/clan info <clã>      outro clã
/clan membros         lista de membros e cargos
/clan top             ranking dos clãs
```

---

## 2. Cargos

| Cargo | Resumo do que pode |
|---|---|
| **Líder** | tudo (e é o único que dissolve o clã ou transfere a liderança) |
| **Vice-líder** | quase tudo: convidar, expulsar, promover, sacar, melhorias, guerra, invasão, território |
| **General** | convidar, expulsar, definir home, guerra, reivindicar território, depositar |
| **Capitão** | convidar, usar home, depositar, construir |
| **Membro** | usar home, depositar, construir, chat do clã |

Regras importantes:
- Você só pode **expulsar ou promover quem tem cargo menor que o seu**.
- Ninguém vira líder por promoção: a liderança é só por transferência.
- Quem gerencia: `/clan promover <jogador>`, `/clan rebaixar <jogador>`.

---

## 3. Cofre do clã

O cofre é o dinheiro compartilhado do clã. Ele paga **melhorias** (e, se a staff ativar, claims e homes).
```
/clan cofre                  mostra o saldo e a capacidade
/clan depositar <valor>      todos podem
/clan sacar <valor|tudo>     só cargos autorizados
/clan extrato                últimas movimentações
```
- Valores aceitam `10k` (10 mil) e `2m` (2 milhões). Só números inteiros.
- Há um **depósito mínimo**, um **limite por saque** e a **capacidade máxima** depende do nível (e da melhoria *Cofre*).
- Toda movimentação fica registrada no extrato.

---

## 4. Home (base do clã)

```
/clan sethome [nome]      define a base onde você está (cargos autorizados)
/clan home [nome]         teleporta
/clan homes               lista as bases
/clan delhome <nome>      apaga
```
- Ao usar `/clan home` há uma **contagem de alguns segundos**: se você **se mexer ou levar dano, cancela**.
- Existe um tempo de espera entre usos.
- **Durante uma guerra, a home fica bloqueada.**
- Quantas homes o clã tem depende do **nível** e da melhoria *Homes* (começa com 1).

---

## 5. Níveis e XP

```
/clan nivel
```
- O clã sobe de nível ganhando **XP**, principalmente em **guerras** e **invasões** (vitória, participação e eliminações válidas).
- Cada nível libera mais **membros, homes, capacidade de cofre e territórios**, e dá uma **recompensa única** em dinheiro para o cofre.
- No menu **Níveis** você vê a barra de progresso e o que cada nível dá.

## 6. Melhorias

```
/clan melhorias                       lista, com custo e nível necessário
/clan melhorias comprar <id>          compra (paga com o cofre)
```
Ou use o menu **Melhorias** (pede confirmação antes de comprar).

| Melhoria | O que dá |
|---|---|
| Membros | mais vagas no clã |
| Homes | mais bases |
| Cofre | mais capacidade de saldo |
| Experiência | mais XP (bônus limitado) |
| Defesa | invasores precisam de mais pontos para tomar seu território |
| Guerra | mais participantes e organização de batalhas |
| Personalização | libera **cores hexadecimais** |
| Território | mais chunks reivindicáveis |
| Comunicação | libera `/clan anuncio` |

Nenhuma melhoria dá bônus de dano ou resistência.

---

## 7. Personalizar o clã

```
/clan nome <novo nome>         (espera de 24 h entre trocas de nome/tag)
/clan tag <nova tag>
/clan cor <cor>                ex.: /clan cor &c  |  /clan cor &#B026FF (hex: VIP + melhoria)
/clan descricao <texto>
/clan lider <jogador> confirmar   transfere a liderança
/clan anuncio <texto>          avisa todo o clã (precisa da melhoria Comunicação)
```
No menu **Configurações** dá para trocar a cor com um clique, sair do clã ou dissolver (sempre com confirmação).

## 8. Chat do clã

```
/clan chat            liga/desliga: suas mensagens vão só para o clã
/clan chat <texto>    manda uma mensagem só para o clã
```

---

## 9. Territórios

Reivindique **chunks** (blocos de 16×16, de cima a baixo) para proteger sua base.
```
/clan territorio reivindicar     o chunk onde você está
/clan territorio abandonar
/clan territorio info            de quem é o chunk atual
/clan territorio lista
/clan territorio tudo confirmar  abandona todos
```
- Ao reivindicar aparece um **contorno de fumaça** em volta do chunk por 5 segundos.
- Regras: longe do spawn, afastado de outros clãs, e os novos chunks precisam **encostar nos que você já tem**.
- O limite de chunks depende do nível e da melhoria *Território*.
- Dentro do território, **só membros (e aliados, se permitido) mexem em blocos, baús e portas**. Explosões, fogo e pistões vindos de fora são bloqueados.
- Sem punição de grief: o plugin protege, não destrói nada.

## 10. Alianças

```
/clan aliados                          lista aliados e pedidos
/clan aliados convidar <clã>
/clan aliados aceitar <clã>
/clan aliados remover <clã>
```
Aliados **não pontuam** eliminações entre si, não podem guerrear nem invadir um ao outro, e podem ter permissões no território (a staff define).

---

## 11. Guerras

Guerra é clã contra clã, com placar.
```
/clan guerra desafiar <clã>      (cargos autorizados)
/clan guerra aceitar <clã>       /clan guerra recusar <clã>
/clan guerra status              situação atual
/clan guerra cancelar            só antes da preparação
/clan guerra desistir confirmar  entrega a vitória ao adversário
/clan guerra ranking             /clan guerra historico
```
**Como funciona:**
1. O clã desafiado tem **10 minutos** para aceitar.
2. A guerra é **agendada**, passa por uma **preparação** e começa.
3. Cada **eliminação válida** de um membro do clã inimigo vale pontos. Vence quem chegar primeiro à pontuação-alvo ou quem tiver mais pontos quando o tempo acabar.
4. Ao final, o clã ganha **XP**, e o vencedor ganha **dinheiro para o cofre** e pontos de temporada.

**Regras antiabuso (resumo para os jogadores):**
- Matar o **mesmo jogador repetidamente** não pontua além de um limite (e há um intervalo mínimo entre as mortes).
- **Contas do mesmo IP**, membros muito recentes, colegas de clã e aliados **não pontuam**.
- **Sair do jogo em combate** pode dar pontos ao adversário.
- **Durante a guerra não dá para sair, ser expulso nem dissolver o clã**, nem usar a home.
- Existem limites de recompensas por dia e esperas entre guerras dos mesmos clãs.
- A staff recebe alertas de comportamento suspeito e investiga manualmente.

## 12. Invasões

Invasão é a tomada do **território** de outro clã por **objetivo**, sem destruir blocos.
```
/clan invasao declarar <clã>
/clan invasao cancelar           só antes de começar
/clan invasao status             /clan invasao historico
```
- O clã atacante precisa de nível mínimo e de membros; o defensor precisa ter território.
- Na hora marcada, os atacantes **ficam dentro do território do defensor** acumulando pontos de captura. Se houver **defensores na área, a captura para** (eles estão contestando).
- Atacantes vencem ao atingir a pontuação-alvo; senão, os defensores vencem quando o tempo acaba.
- Depois de invadido, o defensor ganha um **escudo** por algumas horas. Não dá para abandonar territórios no meio de uma invasão.

---

## 13. O menu `/clan`

Sem clã: *Criar clã (como fazer)*, *Convites*, *Ranking*, *Ajuda*.
Com clã: **Perfil, Membros, Convites, Cofre, Home, Níveis, Melhorias, Guerras, Invasões, Territórios, Aliados, Ranking, Configurações e Ajuda.**

- Clique **esquerdo/direito** nos itens; ações importantes pedem **confirmação**.
- Não dá para tirar nem mover itens do menu.
- Se clicar rápido demais, o clique é ignorado de propósito (evita compras e saques em duplicidade).

## 14. Para os líderes: primeiros passos recomendados

1. `/clan criar <nome> <tag>` e `/clan descricao <texto>`.
2. Convide seus amigos (`/clan convidar <jogador>`) e promova quem você confia.
3. Defina a base: `/clan sethome`.
4. Peça aos membros para **depositarem** no cofre (`/clan depositar`).
5. Compre as primeiras **melhorias** (Membros, Homes, Território).
6. Reivindique o terreno da sua base: `/clan territorio reivindicar`.
7. Quando estiver forte, desafie outro clã: `/clan guerra desafiar <clã>`.

## 15. Perguntas rápidas

| Pergunta | Resposta |
|---|---|
| Não consigo criar outro clã | Há uma espera depois de sair/dissolver; a mensagem diz quanto tempo falta |
| Convite não funciona | Expira em 2 min e só vale uma vez; peça outro |
| Não consigo sacar | Seu cargo não tem permissão, ou passou do limite por saque/diário |
| `/clan home` não funcionou | Você se mexeu, levou dano, está em guerra ou em espera |
| Meu clã está cheio | Suba de nível ou compre a melhoria *Membros* |
| Posso recuperar o clã dissolvido? | Não. A dissolução apaga tudo, por isso pede confirmação |
| Suspeita de abuso/bug | Chame a staff com o horário e o que aconteceu |
