# atividade10-ex11
programa
{
	
	funcao inicio()
	{
		real populacaoA, populacaoB, porcentagemA, porcentagemB
		escreva ("Digite a população atual da População A: ")
		leia(populacaoA)

		escreva ("Digite a população atual da População B: ")
		leia(populacaoB)

		escreva ("Digite a taxa de crescimento anual da População A em porcentagem: ")
		leia(porcentagemA)

		escreva ("Digite a taxa de crescimento anual da População B em porcentagem: ")
		leia(porcentagemB)


		real crescimentoA = (populacaoA / 100) * porcentagemA
		real crescimentoB = (populacaoB / 100) * porcentagemB
		inteiro anos = 0

			se(crescimentoA<crescimentoB){
				para (crescimentoA ; populacaoA <= populacaoB ; populacaoA = ((populacaoA / 100) * porcentagemA) + populacaoA){
				populacaoB = ((populacaoB / 100) * porcentagemB) + populacaoB
				anos = anos +1
				escreva ("\nPopulação A = ", populacaoA ,"\nPopulação B = ", populacaoB,"\n\n")
			}
			}senao{
				para (crescimentoB ; populacaoB <= populacaoA ; populacaoB = ((populacaoB / 100) * porcentagemB) + populacaoB){
				populacaoA = ((populacaoA / 100) * porcentagemA) + populacaoA
				anos = anos +1
				escreva ("\nPopulação B = ", populacaoB ,"\nPopulação A = ", populacaoA,"\n\n")}
		
		escreva ("\nPopulação A = ", populacaoA ,"\nPopulação B = ", populacaoB,"\n\n")}
		escreva("Se passaram ",anos," anos para a População A se igualar ou ser maior que População B")
	}
}
