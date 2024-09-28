# Calculo-de-renda-em-C
programa
{
	
	funcao inicio()
	{
		real salarioBruto, salarioLiquido, salarioMenosINSS, descontos, inss
		cadeia usuario

		escreva("Olá, digite seu nome: ")
			leia(usuario)
		escreva("Olá ", usuario, ", agora digite seu salário bruto e os descontos respectivamente \nSALARIO BRUTO: ")
			leia(salarioBruto)
		escreva("\nDescontos: ")
			leia(descontos)

		se(salarioBruto <= 1302){
			salarioMenosINSS = salarioBruto * 0.925
				inss = salarioBruto - salarioMenosINSS
					salarioLiquido = salarioMenosINSS - descontos
						escreva("  Relação salarial de ", usuario, "\n")
						escreva("╔══════════════════════╦═══════════════════╗\n")
						escreva(" Salário Bruto         ║ R$", salarioBruto, " \n")
						escreva(" Descontos             ║ R$", descontos, "\n")
						escreva(" Desconto do INSS 7,5% ║ R$", inss, "\n")
						escreva(" Salário liquido       ║ R$", salarioLiquido, "\n")
           				escreva("╚══════════════════════╩═══════════════════╝\n")
		}
			se(salarioBruto > 1302 e salarioBruto <= 2571.29){
				salarioMenosINSS = salarioBruto * 0.91
					inss = salarioBruto - salarioMenosINSS	
						salarioLiquido = salarioMenosINSS - descontos
							escreva("  Relação salarial de ", usuario, "\n")	
           					escreva("╔════════════════════╦═══════════════════╗\n")
							escreva(" Salário Bruto       ║ R$", salarioBruto, " \n")
							escreva(" Descontos           ║ R$", descontos, "\n")
							escreva(" Desconto do INSS 9% ║ R$", inss, "\n")
							escreva(" Salário liquido     ║ R$", salarioLiquido, "\n")
           					escreva("╚════════════════════╩═══════════════════╝\n")
			}
				se(salarioBruto > 2571.29 e salarioBruto <= 3856.94){
					salarioMenosINSS = salarioBruto * 0.88
						inss = salarioBruto - salarioMenosINSS	
							salarioLiquido = salarioMenosINSS - descontos
								escreva("  Relação salarial de ", usuario, "\n")
								escreva("╔═════════════════════╦═══════════════════╗\n")
								escreva(" Salário Bruto        ║ R$", salarioBruto, " \n")
								escreva(" Descontos            ║ R$", descontos, "\n")
								escreva(" Desconto do INSS 12% ║ R$", inss, "\n")
								escreva(" Salário liquido      ║ R$", salarioLiquido, "\n")
           						escreva("╚═════════════════════╩═══════════════════╝\n")
				}				
					se(salarioBruto > 3856.94){
						salarioMenosINSS = salarioBruto * 0.86
							inss = salarioBruto - salarioMenosINSS
								salarioLiquido = salarioMenosINSS - descontos
									escreva("  Relação salarial de ", usuario, "\n")
									escreva("╔═════════════════════╦═══════════════════╗\n")
									escreva(" Salário Bruto        ║ R$", salarioBruto, " \n")
									escreva(" Descontos            ║ R$", descontos, "\n")
									escreva(" Desconto do INSS 14% ║ R$", inss, "\n")
									escreva(" Salário liquido      ║ R$", salarioLiquido, "\n")
           							escreva("╚═════════════════════╩═══════════════════╝\n")	
					}
						
		

						
		
		
	}
}
