
## 🠖 Simulador de Autômatos Finitos (AFD)
Este projeto da disciplina de Teoria da Computação implementa um simulador de autômatos finitos determinísticos (**AFD**) utilizando **HTML + JavaScript**, com entrada e saída via arquivos, conforme especificações da atividade.


## ⁇ Como usar
1. Acessar a página do simulador (https://whoisgege.github.io/simulador_automato/) ou abrir (`index.html`) localmente.
2. Enviar os dois arquivos:
   - `.aut` → contendo o autômato no formato JSON.
   - `.in` → contendo as palavras e os resultados esperados (formato CSV).
3. Clicar em **simular**.
4. Baixar o resultado como `saida.out`.


## ～ Formato dos Arquivos

### `.aut` (automato.aut)
```json
{
  "initial": 0,
  "final": [4,5],
  "transitions": [
    { "from": 0, "read": "a", "to": 1 },
    { "from": 1, "read": "b", "to": 2 },
    { "from": 2, "read": "a", "to": 3 },
    { "from": 3, "read": "b", "to": 4 },
    { "from": 4, "read": "a", "to": 5 },
    { "from": 5, "read": "c", "to": 5 }
  ]
}

