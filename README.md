# Verificador de Números Pares e Ímpares

Um programa simples em Java que verifica se um número informado pelo usuário é par ou ímpar, utilizando interface de linha de comando.

## 📋 Funcionalidades

- **Interface de linha de comando**: Interação via terminal/console
- **Entrada de dados**: Solicita um número entre 1 e 10 do usuário
- **Verificação par/ímpar**: Determina se o número é par ou ímpar usando operador módulo
- **Feedback imediato**: Exibe o resultado da verificação instantaneamente
- **Entrada controlada**: Utiliza Scanner para captura segura de dados

## 🚀 Como usar

### Pré-requisitos

- Java JDK 8 ou superior instalado
- Terminal/Prompt de comando

### Compilação

```bash
javac Main.java
```

### Execução

```bash
java Main
```

### Exemplo de uso:

```
Informe um número entre 1 e 10: 7
O número 7 é ímpar.
```

```
Informe um número entre 1 e 10: 4
O número 4 é par.
```

## 📁 Estrutura do projeto

```
projeto/
├── Main.java         # Classe principal com toda a lógica
└── README.md         # Este arquivo
```

## 🔧 Estrutura do Código

### `Main`

Classe principal que contém toda a lógica do programa em um único método `main`.

#### Fluxo de execução:

1. **Criar Scanner**: Instancia objeto Scanner para leitura de entrada
2. **Solicitar entrada**: Exibe mensagem pedindo número entre 1 e 10
3. **Capturar número**: Lê número inteiro digitado pelo usuário
4. **Verificar paridade**: Usa operador módulo (%) para determinar se é par ou ímpar
5. **Exibir resultado**: Mostra se o número é par ou ímpar
6. **Fechar Scanner**: Libera recursos do Scanner

## 💡 Lógica de verificação

### Operador Módulo (%)
O programa utiliza o operador módulo para verificar a paridade:
- **Par**: `numero % 2 == 0` (resto da divisão por 2 é zero)
- **Ímpar**: `numero % 2 != 0` (resto da divisão por 2 é diferente de zero)

### Estrutura condicional:
```java
if (numero % 2 == 0) {
    // Número é par
} else {
    // Número é ímpar
}
```

## 🖥️ Interface de usuário

- **Prompt claro**: "Informe um número entre 1 e 10: "
- **Entrada única**: Solicita apenas um número inteiro
- **Resposta formatada**: Inclui o número informado na resposta
- **Execução única**: Programa termina após mostrar o resultado

## ⚠️ Considerações importantes

- **Range sugerido**: Embora solicite número entre 1 e 10, o programa aceita qualquer inteiro
- **Sem validação**: Não há verificação se o número está no range especificado
- **Tipos de entrada**: Aceita apenas números inteiros (int)
- **Execução única**: Para novo teste, é necessário executar o programa novamente

## 📝 Notas técnicas

- **Scanner**: Utiliza `Scanner(System.in)` para entrada de dados
- **Operador módulo**: Usa `%` para calcular resto da divisão
- **Estrutura condicional**: Implementa `if-else` simples
- **Gerenciamento de recursos**: Chama `scanner.close()` para liberar recursos
- **Saída formatada**: Concatena strings para exibir resultado personalizado


## 🔄 Fluxo do programa

```
Início
  ↓
Criar Scanner
  ↓
Exibir prompt
  ↓
Ler número do usuário
  ↓
Verificar se número % 2 == 0
  ↓
Se SIM → Exibir "é par"
  ↓
Se NÃO → Exibir "é ímpar"
  ↓
Fechar Scanner
  ↓
Fim
```

## 🎯 Casos de teste

| Entrada | Esperado | Motivo |
|---------|----------|---------|
| 2 | "O número 2 é par" | 2 % 2 = 0 |
| 3 | "O número 3 é ímpar" | 3 % 2 = 1 |
| 8 | "O número 8 é par" | 8 % 2 = 0 |
| 9 | "O número 9 é ímpar" | 9 % 2 = 1 |
| 10 | "O número 10 é par" | 10 % 2 = 0 |
