programa
{
	caracter confirm
	inteiro op=0,ladoB[5] = {0,0,0,0,0}
	cadeia item[5] = {"","(1 - Camponês)"," (2 - Lobo)", " (3 - Ovelha)"," (4 - Couve)"}
	
	funcao inicio()
	{
		escreva("Olá! Vamos resolver um problema de lógica, vou lhe passar a situação...")
		escreva("\n\nUm camponês precisa atravessar um riacho, de um lado (A) para o outro (B), e ele deve levar: Uma ovelha, um lobo e um maço de couve")
		escreva("\n\nAí está o problema: Ele so pode levar um de cada vez. Portanto, Se ele deixar o lobo junto com a ovelha, ela vira banquete")
		escreva("\n\nE se ele deixar a ovelha unto com o maço de couve, ja era!")
		escreva(" Está preparado? digite (s) para Sim: ")
		leia(confirm)
		se(confirm=='s' ou confirm =='S')
		{	limpa()		
			escreva("Vamos lá! \n\nNo lado (A) estão: ",item[1-ladoB[1]],item[2-ladoB[2]],item[3-ladoB[3]],item[4-ladoB[4]],"\n\n")	
			
			enquanto(op>=0 e op<=3)
			{	escreva("Digite o número correspondente ao item que você quer passar para o lado (B): ")
				leia (op)
				ladoB[op]=op
				se(op!=1) ladoB[1]=1
				se(ladoB[1]!=0 e ladoB[2]==0 e ladoB[3]==0 e ladoB[4]==0)//Lobo devora ovelha no lado A
				{	limpa()
					escreva("Que pena! Você deixou a ovelha sozinha com o lobo e ele a devorou. Tente novamente!\n")
					pare
				}
				se(ladoB[1]!=0 e ladoB[2]!=0 e ladoB[3]==0 e ladoB[4]==0)//Ovelha com e a couve no lado A
				{	limpa()
					escreva("Que pena! Você deixou a ovelha sozinha com a couve e ela comeu. Tente novamente!\n")
					pare
				}
				se(ladoB[1]!=0 e ladoB[2]==0 e ladoB[3]==0 e ladoB[4]!=0)//Lobo devora ovelha no lado A
				{	limpa()
					escreva("Que pena! Você deixou a ovelha sozinha com o lobo e ele a devorou. Tente novamente!\n")
					pare
				}
				se(ladoB[1]!=0 e ladoB[2]!=0 e ladoB[3]!=0 e ladoB[4]!=0)//Parabéns!
				{	limpa()
                			escreva("Meus Parabéns! Você conseguiu!!!\n\n")
					pare
				}

				limpa()
				escreva("No lado (B) estão:",item[ladoB[1]],item[ladoB[2]],item[ladoB[3]],item[ladoB[4]],"\n")
				escreva("\nDigite o número correspondente ao que você deseja trazer para o lado (A): ")
				leia(op)
				ladoB[op]=0
				se(op!=1) ladoB[1]=0
				se(ladoB[1]==0 e ladoB[2]!=0 e ladoB[3]!=0 e ladoB[4]==0)//Lobo devora ovelha no lado B
				{	limpa()
					escreva("Que pena! Você deixou a ovelha sozinha com o lobo e ele a devorou. Tente novamente!\n")
		     			pare
				}
			
				se(ladoB[1]==0 e ladoB[2]==0 e ladoB[3]!=0 e ladoB[4]!=0)//Ovelha come a couve no lado B
				{	limpa() 
					escreva("Que pena! Você deixou a ovelha sozinha com a couve e ela almoçou. Tente novamente!\n")
					pare
				}
				limpa()
				escreva("Agora no lado (A) nós temos:", item[1-ladoB[1]],item[2-ladoB[2]],item[3-ladoB[3]],item[4-ladoB[4]], "\n\n")
			}	
		}
		senao
			escreva("\nVocê digitou (não) ou um caracter inválido, Tente novamente!\n")
	}
}
