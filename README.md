# 🔒 Operação Enigma: A Fuga do Bunker
### Jogo Digital Escape Room de Análise Combinatória — Projeto 2 (Matemática Discreta)

## 1. Sobre o Projeto
**Operação Enigma: A Fuga do Bunker** é um jogo digital interativo no estilo *Escape Room* desenvolvido para o ensino e avaliação de **Análise Combinatória** (nível de Ensino Médio e 1º semestre de graduação). O jogador assume o papel de um especialista preso em um bunker subterrâneo controlado por uma IA em confinamento e deve destravar 5 portas de segurança resolvendo 12 problemas matemáticos.

## 2. Estrutura das Fases e Requisitos Atendidos
| Fase | Cenário | Nível | Acertos Exigidos | Banco de Questões | Conteúdos Foco |
|---|---|---|---|---|---|
| **1** | Porta de Entrada Blindada | Fácil | 1 | 10 questões | Princípio Fundamental da Contagem (PFC) |
| **2** | Arquivo Criptografado | Básico | 2 | 10 questões | Permutação Simples e Arranjo Simples |
| **3** | Laboratório Bioquímico | Intermediário | 2 | 10 questões | Permutação com Repetição e Combinação Simples |
| **4** | Sala dos Servidores | Avançado | 3 | 10 questões | Problemas com Restrições (Juntos/Separados, Posições) |
| **5** | Núcleo do Reator Quântico | Difícil | 4 | 10 questões | Divisão em Casos, Tabuleiros e Combinação Completa |
| **Total** | **5 Ambientes** | **Progressivo** | **12 acertos** | **50 questões** | **Todos os tópicos obrigatórios** |

## 3. Funcionalidades Implementadas
* **Sorteio Aleatório sem Repetição:** As questões são sorteadas aleatoriamente dentro de cada fase e não se repetem durante a mesma partida (`Set` de controle de IDs).
* **Manutenção de Progresso ao Errar:** Ao errar uma questão, o jogador mantém os acertos já conquistados na fase e recebe uma nova questão do mesmo nível, perdendo apenas 1 tentativa (vida).
* **Condições de Vitória e Derrota:** O jogador possui **5 vidas** e um cronômetro regressivo de **15 minutos**. Concluir os 12 acertos leva à tela de Vitória; zerar as vidas ou o tempo leva à tela de Derrota.
* **Efeitos Sonoros Sintetizados (Web Audio API):** Sons de acerto, erro e avanço de fase gerados nativamente pelo navegador sem depender de arquivos externos pesados.
* **Feedback Matemático Imediato:** Após responder cada questão, o jogo exibe a resolução matemática passo a passo.

## 4. Como Publicar no GitHub Pages (Geração do Link do Jogo)
1. Crie um novo repositório público no GitHub (ex.: `escape-room-combinatoria`).
2. Faça o upload dos arquivos deste pacote (`index.html`, `questions.json`, `README.md`).
3. No repositório do GitHub, acesse **Settings** > **Pages**.
4. Em **Branch**, selecione `main` (ou `master`) e clique em **Save**.
5. Em 1 minuto, o link oficial do jogo estará ativo em `https://seu-usuario.github.io/escape-room-combinatoria/`.
