# 🎮 Desafio de Nivelamento – League of Legends Manager (Java Puro)

## 🎯 Objetivo

Criar um sistema de gerenciamento de Campeões inspirado no universo de League of Legends utilizando **apenas Java puro**, sem frameworks ou bibliotecas externas.

Este desafio tem como objetivo avaliar:

- Organização de código
- Separação de responsabilidades
- Lógica de programação
- Modelagem orientada a objetos
- Tomada de decisão
- Clareza e legibilidade

---

## ⚠️ Regras Obrigatórias

- ❌ Não utilizar frameworks (Spring, Hibernate, etc.)
- ❌ Não utilizar banco de dados real
- ❌ Não utilizar bibliotecas externas
- ✅ Utilizar apenas Java puro
- ✅ Aplicar separação em camadas (MVC)
- ✅ Simular persistência com estrutura estática em memória

---

## 🏗️ Cenário

Você foi contratado para criar um sistema simples de gerenciamento de campeões para uma organização fictícia de eSports.

O sistema deve permitir:

1. Cadastrar campeão
2. Atualizar campeão
3. Buscar campeão por ID
4. Listar campeões
5. Remover campeão

---

## 🧱 Modelo do Campeão

Cada campeão deve possuir:

- id (gerado automaticamente)
- nome
- classe (Ex: Mago, Lutador, Atirador, Tank, Suporte)
- danoBase
- vidaBase
- dificuldade (1 a 5)

---

## 🧠 Regras de Negócio

1. Não permitir cadastro de campeão com nome vazio.
2. Não permitir danoBase ou vidaBase negativos.
3. Dificuldade deve estar entre 1 e 5.
4. Não permitir dois campeões com o mesmo nome.
5. Se a classe for "Mago", o danoBase deve ser maior que 50.
6. Se a classe for "Tank", a vidaBase deve ser maior que 500.

---

## 🏛️ Estrutura Esperada (MVC)

O projeto deve conter separação clara de responsabilidades:
```
src/
├── model/
├── repository/
├── service/
├── controller/
├── view/
└── Main.java
```

---
## 💾 Persistência
Simular banco de dados utilizando:
- Um Map estático
- Armazenamento em memória
- Controle manual de ID auto incremental

Exemplo esperado:
```java
private static Map<Long, Champion> database = new HashMap<>();
```

---
## 🧪 Tomada de Decisão

Durante o desenvolvimento, considere:
- Onde devem ficar as regras de validação?
- Quem deve ser responsável por gerar ID?
- A Controller deve conhecer a estrutura do Map?
- O Service deve acessar o Map diretamente?
- Como evitar código duplicado?

---
## 🎮 Funcionalidade Extra (Opcional)

Implemente um método que calcule o "Power Score" do campeão:
```
PowerScore = (danoBase * 2) + vidaBase - (dificuldade * 10)
```

E permita listar campeões ordenados por PowerScore.

---
## 🪤 Observação Importante

O foco deste desafio é organização e raciocínio.
Soluções excessivamente complexas ou utilização de recursos não solicitados podem indicar fuga do escopo proposto.

---
## 📦 Entregáveis
O projeto deve conter:
- Código organizado em camadas
- Explicação sobre onde colocou as regras de negócio e por quê
- Explicação sobre possíveis melhorias futuras

---
## 🎓 O que será avaliado
- Clareza da modelagem
- Separação de responsabilidades
- Coesão e acoplamento
- Organização de pacotes
- Legibilidade
- Capacidade de justificar decisões técnicas