# Mobbi Grok

Modelo público de um Grok Bot que reserva, consulta e cancela lugares de estacionamento no portal MobbiPro de uma empresa (`https://<tenant>.mobbipro.pt`).

> **🎙️ 🚗 As reservas podem ser feitas por voz no Grok Bot. Nos carros Tesla, a reserva pode ser feita diretamente a partir do carro.**

## O que faz

O Mobbi Grok trata do estacionamento no portal MobbiPro:

- reserva um lugar (dia inteiro, manhã, tarde ou horário personalizado);
- consulta as reservas (data, horário, zona, tipo de lugar e estado);
- cancela uma reserva concreta, apenas quando o pedido for explícito para essa reserva.

Na primeira conversa, a skill de arranque pede o endereço do portal e o início de sessão (guardado no cofre). A zona, o tipo de lugar, o veículo e o idioma são opcionais, porque o portal já assume as predefinições da conta. Se fizer sentido, pergunta também por uma rotina semanal que reserva esses dias com antecedência.

## O que está no repositório

| Ficheiro | Função |
| --- | --- |
| `skills/mobbipro-getting-started/SKILL.md` | Primeira conversa: endereço do portal e início de sessão no cofre. Zona, tipo de lugar, veículo e idioma são opcionais, porque o portal já assume as predefinições da conta. Rotina semanal opcional. |
| `skills/book-mobbipro-parking/SKILL.md` | Reservar, consultar e cancelar lugares no portal. |
| `LICENSE` | Licença MIT. Copyright 2026 Vasco Pinheiro. |

## Como usar

### Opção 1 — Instalar diretamente pelo link

**[Importar o Mobbi Grok no Grok Bot](https://x.ai/bot/ZkYt-p7_BweHRkUoqUD_d)**

Ao abrir o link, o Mobbi Grok é importado para o Grok Bot. A primeira conversa pede o endereço do portal e o início de sessão. A zona, o tipo de lugar, o veículo e o idioma são opcionais, porque o portal já assume as predefinições da conta.

### Opção 2 — Instalação manual a partir do repositório

1. Crie um bot novo no Grok Bot com o nome **Mobbi Grok**.
2. Adicione as duas skills deste repositório como skills do bot:
   - `skills/mobbipro-getting-started/SKILL.md`
   - `skills/book-mobbipro-parking/SKILL.md`
3. Inicie a primeira conversa. A skill `mobbipro-getting-started` pergunta, um ponto de cada vez:
   - o endereço do portal;
   - o início de sessão, num formulário seguro, para ficar guardado no cofre (vault) do bot;
   - opcionalmente, a zona, o tipo de lugar, o veículo e o idioma, porque o portal já assume as predefinições da conta;
   - se reserva os mesmos dias todas as semanas e, nesse caso, uma rotina semanal opcional que os reserva automaticamente com antecedência.

Depois disso, peça em linguagem natural para reservar, consultar ou cancelar um lugar.

## Credenciais e dados pessoais

Este repositório é um modelo partilhável. Não inclui credenciais nem dados pessoais. Guarde os inícios de sessão no cofre do bot, nunca neste repositório.

---

# English

## What the bot does

Mobbi Grok is a public, shareable Grok Bot template. It books, checks and cancels parking spots on a company's MobbiPro portal (`https://<tenant>.mobbipro.pt`).

> **🎙️ 🚗 Bookings can be made by voice in Grok Bot. In Tesla cars, the booking can be made directly from the car.**

## What's in the repo

| File | Role |
| --- | --- |
| `skills/mobbipro-getting-started/SKILL.md` | First chat: portal address and login saved in the vault. Zone, spot type, vehicle and language are optional, because the portal already assumes the account's defaults. Optional weekly booking routine. |
| `skills/book-mobbipro-parking/SKILL.md` | Book, check and cancel parking spots. |
| `LICENSE` | MIT License. Copyright 2026 Vasco Pinheiro. |

## How to use it

### Option 1 — Install directly from the link

**[Import Mobbi Grok into Grok Bot](https://x.ai/bot/ZkYt-p7_BweHRkUoqUD_d)**

Opening it imports Mobbi Grok into Grok Bot. The first conversation asks for the portal address and the login. Zone, spot type, vehicle and language are optional, because the portal already assumes the account's defaults.

### Option 2 — Manual installation from the repository

1. Create a new bot in Grok Bot and name it **Mobbi Grok**.
2. Add the two skills in this repository as the bot's skills:
   - `skills/mobbipro-getting-started/SKILL.md`
   - `skills/book-mobbipro-parking/SKILL.md`
3. Start the first chat. The getting-started skill asks, one item at a time, for:
   - the portal address;
   - the login, through a Secure Form, so it is saved in the bot's vault;
   - optionally, the zone, spot type, vehicle and language, because the portal already assumes the account's defaults;
   - whether the same days are booked every week and, if so, an optional weekly routine that books them automatically ahead of time.

After that, ask in plain language to book, check or cancel a spot.

## Credentials and personal data

This template includes no credentials and no personal data. Save logins in the bot's vault, never in the repo.
