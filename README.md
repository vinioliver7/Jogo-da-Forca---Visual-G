# Jogo-da-Forca---Visual-G
Este Código foi escrito em Portugol em aula no meu segundo mês de curso


Algoritmo "Jogo de Forca"
// Disciplina   : [Algoritimos]
// Professor   : Roger Santos
// Autor(a)    : Vinícius Valério
// Data atual  : 28/11/2022
Var
   //variáveis
   palavra,dica,chute:caractere
   nLetras:inteiro

Inicio
   // Seção de Comandos, procedimento, funções, operadores, etc...
   escreval("                                ")
   escreval("                                ")
   escreval("                                ")
   escreval("                                ")
   escreval("                   Digite a palavra secreta ")
   escreva("                    ->")
   LEIA(palavra)
   nLetras<- Compr(palavra)
   escreval("                   Digite a dica ")
   escreva("                    ->")
   leia(dica)
   escreval("                                     ")
   escreval("                                     ")
   escreval("               -------------------------------- ")
   escreval("              |  [P] Prosseguir    [V] Voltar  |")
   escreval("               -------------------------------- ")

   chute<-("n")
   enquanto (chute<>"p")faça
      limpatela

      escreval("                                ")
      escreval("             A Palavra secreta tem",(nLetras)," letras")
      escreval("                A dica é: ",(dica))
      escreval("                                ")
      escreval("          /-----\                      ")
      escreval("          |     |                 ")
      escreval("          |                      ")
      escreval("          |                     ")
      escreval("          |                       ")
      escreva("         ---   ")
      escreva("")
      leia(chute)

      se(chute=palavra)entao
         chute<-("p")
      fimse
   fimenquanto
   
   limpatela
   escreval("                                ")
   escreval("                                ")
   escreval("         parabéns você acertou a resposta")
   escreval("                   '",(palavra),"'")
