#  Pilha - ED 🔋
ㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤ
## Introdução
A pilha armazena apenas a posição de uma de suas extremidades (chamada topo), que é o único local onde são realizadas todas as operações de entrada e saída. A operação de entrada de dados (sempre no topo da pilha ) é chamada push e a retirada (também sempre do topo) é chamada pop.

## Definição 

É uma estrutura de dados de tamanho variável, sendo que elementos são incluídos (empilhados) e/ou removidos (desempilhados) apenas pela extremidade topo.

## FILO (first-in, last-out)

Pilhas são listas lineares com disciplina de acesso FILO (first-in, last-out, ou, o primeiro a entrar é o último a sair).

## Alocação de Memória

- Alocação Estática: Em geral através de arranjo ou
vetor;
- Alocação Dinâmica: Utilizando ponteiro.

## Operações Básicas:

Teste de pilha vazia;
- Criação da pilha;
- Empilhamento;
- Desempilhamento;
- Acesso aos elementos da pilha;
- ✓ Topo
- ✓ Tamanho

## Pilha: Alocação Dinâmica

Considere a definição do tipo Pilha abaixo:
```
class No {
   Tipo dado;
   No próximo; //Ponteiro
}
```

## Teste de Pilha Vazia

```
No topo;
   booleano pilhaVazia() {
       se (topo == nulo) {
          retorne verdadeiro;
       } senão {
  retorne falso;
  }
}
```

## Empilhando um elemento (push)

```
No topo;
   void push (tipo e) {
      No elemento = new No();
      elemento.dado = e;
          se (pilhaVazia() == verdadeiro) {
             topo = elemento;
          } senão {
          elemento.proximo = topo;
          topo = elemento;
          } 
   }
```

## Desempilhando um elemento (pop)

```
No topo;
   tipo pop() {
      se (pilhaVazia() == verdadeiro) {
          exceção(“Não há elementos para desempilhar”);
      }
      tipo valor = topo.dado;
      topo = topo.proximo;
      retorne valor;
   }
```

## Acessando elementos da pilha

Como estamos usando uma lista simplesmente encadeada podemos acessar todos os elementos da pilha, a partir do topo, sem ter a necessidade de desempilhá-los.

### Verificar o topo da pilha

```
No topo;
   tipo topo() {
      se (pilhaVazia() == verdadeiro) {
          exceção(“Não há elementos na pilha”);
      }
      tipo valor = topo.dado;
      retorne valor;
}
```

## Verificar o tamanho da pilha:

```
No topo;
   tipo tamanho() {
   int cont = 0;
      se (pilhaVazia() == falso) {
         No auxiliar = topo;
         cont = 1;
         enquanto (auxiliar.proximo != null) {
             cont = cont + 1;
         auxiliar = auxiliar.proximo;
   }
}
 retorne cont;
}
```

## Verificar o tamanho da pilha:

```
No topo;
   tipo tamanho() {
   int cont = 0;
      se (pilhaVazia() == falso) {
         No auxiliar = topo;
         cont = 1;
         enquanto (auxiliar.proximo != null) {
             cont = cont + 1;
             auxiliar = auxiliar.proximo;
         }
      } 
 retorne cont;
}
```


## Exemplo (pilha de inteiros):

```
class exemplo {
   void main(String[] args) {
        Pilha p = new Pilha();
        p.push(5);
        p.push(4);
        p.push(3);
        inteiro topo = p.topo();
             escreva(“Topo:”+topo);
             inteiro tamanho = p.tamanho();
                  escreva(“Tamanho da Pilha:”+tamanho);
                  ...
  }
}
```


# 📝 Exercícios de Pilha com Java

- [x] Implemente uma função que imprima os elementos de uma Pilha.
- [x] Faça uma função que inverta a ordem dos elementos da Pilha.
- [x] Faça uma função para retornar o número de elementos da Pilha que possuem valor ímpar.
- [x] Faça uma função para retornar o número de elementos da Pilha que possuem valor par.
ㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤㅤ
<div align="center">
    © Material fornecido por <a href="[https://www.homehost.com.br/](https://br.linkedin.com/in/icarofreitas)">Prof° Ícaro de Paula Freitas</a></p>
</div>
