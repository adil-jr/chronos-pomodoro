# Chronos Pomodoro

Aplicação web de gerenciamento de produtividade baseada na Técnica Pomodoro, com funcionalidades personalizadas e interface moderna.

## Sobre o Projeto

O **Chronos Pomodoro** é uma aplicação que implementa a Técnica Pomodoro criada por Francesco Cirillo, permitindo dividir o trabalho em blocos de tempo intercalados com pausas para manter o foco e evitar o cansaço mental.

### Diferenciais

- Personalização completa dos tempos de foco e descanso
- Sistema de ciclos organizados automaticamente
- Visualização intuitiva dos ciclos com indicadores coloridos
- Histórico automático de todas as tarefas
- Interface moderna com paleta de cores vibrante
- Suporte a tema claro e escuro

## Funcionalidades

### Personalização de Tempos
Configure o tempo de foco, descanso curto e descanso longo de acordo com suas preferências através da página de configurações.

### Sistema de Ciclos
- **Ciclos ímpares** (1, 3, 5, 7...): Trabalho (foco)
- **Ciclos pares** (2, 4, 6...): Descanso curto
- **Ciclo 8** (e múltiplos): Descanso longo especial

### Visualização dos Ciclos
Os ciclos são representados por indicadores coloridos:
- **Âmbar**: Ciclo de trabalho (foco)
- **Azul royal**: Descanso curto
- **Azul brilhante**: Descanso longo

### Histórico Automático
Todas as tarefas e ciclos concluídos são salvos automaticamente no histórico, com status de completas ou interrompidas, permitindo acompanhar sua evolução ao longo do tempo.

## Tecnologias Utilizadas

- **React 19** - Biblioteca JavaScript para construção de interfaces
- **TypeScript** - Superset JavaScript com tipagem estática
- **Vite** - Build tool moderna e rápida
- **React Router 7** - Roteamento para aplicações React
- **date-fns** - Biblioteca para manipulação de datas
- **react-toastify** - Notificações toast elegantes
- **lucide-react** - Ícones modernos e customizáveis
- **CSS Modules** - Estilização com escopo local

## Paleta de Cores (Imowash Theme)

A aplicação utiliza a paleta **Imowash**, com tons azuis vibrantes e modernos:

| Cor | Hex Code | Uso |
|-----|----------|-----|
| Azul vibrante/elétrico | `#040DBF` | Hover e elementos ativos |
| Azul royal profundo | `#032CA6` | Cor principal |
| Azul médio brilhante | `#1F64BF` | Realces suaves |
| Azul extremamente escuro | `#010326` | Fundo principal |
| Branco suave | `#F2F2F2` | Texto |

### Cores de Alerta
- **Sucesso**: `#10b981` (Verde menta)
- **Alerta**: `#f59e0b` (Âmbar)
- **Erro**: `#ef4444` (Vermelho suave)
- **Info**: `#1F64BF` (Azul médio brilhante)

## Como Executar

### Pré-requisitos
- Node.js (versão 18 ou superior)
- npm ou yarn

### Instalação

1. Clone o repositório
```bash
git clone <url-do-repositorio>
cd chronos-pomodoro
```

2. Instale as dependências
```bash
npm install
```

3. Execute o projeto em modo de desenvolvimento
```bash
npm run dev
```

4. Acesse a aplicação em `http://localhost:5173`

### Scripts Disponíveis

- `npm run dev` - Inicia o servidor de desenvolvimento
- `npm run build` - Gera a build de produção
- `npm run preview` - Visualiza a build de produção localmente
- `npm run lint` - Executa o linter para verificar o código

## Estrutura do Projeto

```
chronos-pomodoro/
├── src/
│   ├── components/        # Componentes reutilizáveis
│   ├── contexts/          # Contextos React (TaskContext)
│   ├── pages/             # Páginas da aplicação
│   │   ├── AboutPomodoro/ # Página sobre a técnica
│   │   ├── History/       # Histórico de tarefas
│   │   ├── Home/          # Página principal
│   │   ├── NotFound/      # Página 404
│   │   └── Settings/      # Configurações
│   ├── styles/            # Estilos globais e temas
│   ├── templates/         # Templates de layout
│   ├── utils/             # Funções utilitárias
│   └── main.tsx           # Ponto de entrada
├── public/                # Arquivos estáticos
└── package.json           # Dependências e scripts
```

## Páginas

- **/** - Página inicial com timer Pomodoro
- **/about-pomodoro** - Explicação detalhada da Técnica Pomodoro
- **/history** - Histórico de tarefas completadas e interrompidas
- **/settings** - Configurações de tempos personalizados
- **/404** - Página de erro para rotas não encontradas

## Licença

Este projeto foi desenvolvido como parte do curso de React 19 e Next 15 - Luiz Otávio Miranda.
