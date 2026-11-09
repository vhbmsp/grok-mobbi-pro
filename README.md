# Mobbi Grok

Modelo público de um Grok Bot que reserva, consulta e cancela lugares de estacionamento no portal MobbiPro de uma empresa (`https://<tenant>.mobbipro.pt`).

## O que faz

O Mobbi Grok trata do estacionamento no portal MobbiPro:

- reserva um lugar (dia inteiro, manhã, tarde ou horário personalizado);
- consulta as reservas (data, horário, zona, tipo de lugar e estado);
- cancela uma reserva concreta, apenas quando o pedido for explícito para essa reserva.

Na primeira conversa, a skill de arranque pede o endereço do portal, o início de sessão (guardado no cofre), a zona predefinida, o tipo de lugar, o veículo, o idioma e, se fizer sentido, uma rotina semanal que reserva esses dias com antecedência.

## O que está no repositório

| Ficheiro | Função |
| --- | --- |
| `skills/mobbipro-getting-started/SKILL.md` | Primeira conversa: endereço do portal, início de sessão no cofre, zona predefinida, tipo de lugar, veículo, idioma e rotina semanal opcional. |
| `skills/book-mobbipro-parking/SKILL.md` | Reservar, consultar e cancelar lugares no portal. |
| `LICENSE` | Licença MIT. Copyright 2026 Vasco Pinheiro. |

## Como usar

1. Crie um bot novo no Grok Bot com o nome **Mobbi Grok**.
2. Adicione as duas skills deste repositório como skills do bot:
   - `skills/mobbipro-getting-started/SKILL.md`
   - `skills/book-mobbipro-parking/SKILL.md`
3. Inicie a primeira conversa. A skill `mobbipro-getting-started` pergunta, um ponto de cada vez:
   - o endereço do portal;
   - o início de sessão, num formulário seguro, para ficar guardado no cofre (vault) do bot;
   - a zona predefinida;
   - o tipo de lugar;
   - o veículo;
   - o idioma;
   - se reserva os mesmos dias todas as semanas e, nesse caso, uma rotina semanal opcional que os reserva automaticamente com antecedência.

Depois disso, peça em linguagem natural para reservar, consultar ou cancelar um lugar.

## Credenciais e dados pessoais

Este repositório é um modelo partilhável. Não inclui credenciais nem dados pessoais. Guarde os inícios de sessão no cofre do bot, nunca neste repositório.

---

# English

## What the bot does

Mobbi Grok is a public, shareable Grok Bot template. It books, checks and cancels parking spots on a company's MobbiPro portal (`https://<tenant>.mobbipro.pt`).

## What's in the repo

| File | Role |
| --- | --- |
| `skills/mobbipro-getting-started/SKILL.md` | First chat: portal address, login saved in the vault, default zone, spot type, vehicle, language, and an optional weekly booking routine. |
| `skills/book-mobbipro-parking/SKILL.md` | Book, check and cancel parking spots. |
| `LICENSE` | MIT License. Copyright 2026 Vasco Pinheiro. |

## How to use it

1. Create a new bot in Grok Bot and name it **Mobbi Grok**.
2. Add the two skills in this repository as the bot's skills:
   - `skills/mobbipro-getting-started/SKILL.md`
   - `skills/book-mobbipro-parking/SKILL.md`
3. Start the first chat. The getting-started skill asks, one item at a time, for:
   - the portal address;
   - the login, through a Secure Form, so it is saved in the bot's vault;
   - the default zone;
   - the spot type;
   - the vehicle;
   - the language;
   - whether the same days are booked every week and, if so, an optional weekly routine that books them automatically ahead of time.

After that, ask in plain language to book, check or cancel a spot.

## Credentials and personal data

This template includes no credentials and no personal data. Save logins in the bot's vault, never in the repo.
