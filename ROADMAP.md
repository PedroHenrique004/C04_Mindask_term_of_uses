# Roadmap de Futuro: MindAsk 🚀

Este documento contém ideias e sugestões estratégicas de implementação para as próximas versões do aplicativo **MindAsk** (1.1, 2.0+), baseadas nas tecnologias mais recentes e recomendadas do ecossistema Apple.

> [!NOTE]
> Estas implementações foram pensadas para aumentar o engajamento do usuário, dar mais visibilidade ao aplicativo na tela inicial e garantir a segurança dos dados.

---

## 1. Widgets Interativos (Home Screen e Lock Screen)
A primeira coisa que os usuários pedem em apps de produtividade são Widgets para acesso rápido sem precisar abrir o aplicativo.

* **Widget de Foco/Rotina:** Um widget que mostra a próxima tarefa do dia. Com o iOS 17+, os widgets são **interativos**, permitindo que o usuário dê um "Check" na tarefa direto da tela inicial.
* **Widget de Reflexão:** Um widget na Tela de Bloqueio ou Inicial exibindo o último insight gerado pela Inteligência Artificial ou uma citação/reflexão rápida.

## 2. Live Activities e Dynamic Island (Atividades ao Vivo)
Ideal para a seção de execução e acompanhamento de tarefas (como a view `StartTask`).

* Quando o usuário inicia uma tarefa com duração, uma **Live Activity** pode ser disparada.
* O cronômetro ou status da tarefa fica visível o tempo todo na **Dynamic Island** (em iPhones mais novos) e na Tela de Bloqueio. 
* Isso passa um visual premium e ajuda muito no foco do usuário (estilo Pomodoro).

## 3. Sincronização em Nuvem (CloudKit + SwiftData)
Para evoluir de um aplicativo puramente local para uma experiência multi-dispositivo segura.

> [!IMPORTANT]
> Esta é provavelmente a feature técnica mais importante para evitar que o usuário perca seu histórico de diário e anotações.

* A transição do SwiftData local para usar o **iCloud (CloudKit)**.
* Garante backup automático das tarefas e reflexões.
* Permite que o MindAsk no futuro tenha versões para iPadOS e macOS com sincronização instantânea.

## 4. Gráficos de Autoconhecimento (Apple Charts)
O grande diferencial do MindAsk é unir produtividade e saúde mental. Essa funcionalidade conectaria os dois mundos visualmente.

* Usando o framework **SwiftUI Charts**.
* Criação de uma aba de **Progresso** ou **Estatísticas**.
* Mostrar gráficos cruzando dados: *Ex: Nos dias em que o humor é classificado como "Excelente", a taxa de conclusão de tarefas aumenta em 40%.* 

## 5. Gamificação de Hábitos (Streaks)
Para estimular o usuário a entrar no aplicativo todos os dias e criar a rotina de reflexão diária.

* Uma seção de **Ofensiva (Streak)** mostrando quantos dias seguidos o usuário realizou suas anotações e avaliou o dia.
* Pode incluir micro-recompensas, como a troca do ícone do aplicativo ou temas visuais ao atingir marcas de 7, 30, ou 100 dias seguidos.

> [!TIP]
> Projetos que utilizam a fundo as mais novas tecnologias da Apple (como Live Activities e SwiftData) possuem uma probabilidade muito maior de serem destacados na aba "Hoje" da App Store.
