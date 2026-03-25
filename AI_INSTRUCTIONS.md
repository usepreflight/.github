# The Swarm Constitution (Governança Guiada por I.A)

Este arquivo atua como o **Master System Prompt Baseline** de qualquer Agente de Inteligência Artificial atuando sobre os repositórios da Organização `usepreflight`. Humanos também devem ler-lo.

## 1. Princípios de Arquitetura Limpa
- **Extrema Modularidade:** O código deve ser quebrado em funções atômicas menores que 50 linhas se possível.
- **Fail-Fast:** Não mascare Exceptions críticas no Backend (Python) com `try-except pass`. Deixe a máquina explodir nos logs para facilitar o rastreio.

## 2. Restrições do Design System (Frontend)
- Utilize **SEMPRE** TailwindCSS de forma nativa e classes utilitárias curtas.
- O Tema Central da marca é o `Hacker Dark Mode`. Jamais insira sombras opacas (Drop-Shadows estilo Material). Use sempre bordas sutis (`border-white/10`) e `Bg-Blur` nos fundos como sinalização de elevação.
- A Tipografia técnica para Dados e Logs deve ser irrevogavelmente **Monospaced** (`JetBrains Mono` ou `Fira Code`).

## 3. Protocolos de Integração e PRs
- Nenhuma Inteligência ou Dev abre um `Pull Request` sem antes criar a respectiva *Issue* detalhada no backlog.
- Cada Commit deve seguir a semântica nativa global: `feat:`, `chore:`, `fix:`, `docs:`, ou `refactor:`.
- Zero tolerância para jargões não técnicos nos comentários do código. O fluxo de raciocínio é binário, direto e pragmático.