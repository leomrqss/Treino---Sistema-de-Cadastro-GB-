# Treino---Sistema-de-Cadastro-GB-
// Treinando um sistema de cadastro de alunos em uma academia de jiu-jitsu.
// Lógica de Programação em Portugol (Desenvolvedor JAVA - Senai)

programa {
  funcao inicio() {
  
    // Variáveis de texto (cadeia) e número (inteiro) para armazenar os dados.
    cadeia nome, email, endereco, contato_responsavel, info_medica
    inteiro idade

    // Váriaveis para receber a escolha dos menus.
    inteiro opcao_plano, opcao_pagamento, opcao_horario

    // Variáveis para guardar o resultado das escolhas.
    cadeia plano = "", pagamento = "", horario = ""

    // Cabeçalho
    escreva("========================================\n")
    escreva("   SISTEMA DE CADASTRO - GRACIE BARRA   \n")
    escreva("========================================\n\n") 

    // 1. ENTRADA DOS DADOS PESSOAIS
    escreva("--- Dados Pessoais ---\n")
    escreva("Nome completo: ")
    leia(nome)

    escreva("Idade: ")
    leia(idade)

    escreva("E-mail: ")
    leia(email)

    escreva("Endereço: ")
    leia(endereco)

    escreva("Contato de emergência / Responsável: ")
    leia(contato_responsavel)

    // 2. INFORMAÇÕES MÉDICAS
    escreva("\n--- Informações Médicas ---\n")
    escreva("Possui doenças, alergias ou lesões? (Descreva ou digite 'Nenhuma'): ")
    leia(info_medica)

    // 3. MENU DE PLANOS
    escreva("\n--- Plano de Treino ---\n")
    escreva("1 - Mensal\n")
    escreva("2 - Trimestral\n")
    escreva("3 - Semestral\n")
    escreva("4 - Anual\n")
    escreva("Escolha o plano (1 a 4): ")
    leia(opcao_plano)
    
    // A estrutura 'escolha' traduz o número digitado para o nome do plano.
    escolha(opcao_plano){
      caso 1: plano = "Mensal" pare
      caso 2: plano = "Trimestral" pare
      caso 3: plano = "Semestral" pare
      caso 4: plano = "Anual" pare
      caso contrario: plano = "Não definido (Opção inválida)"
    }

    // 4. MENU DE PAGAMENTO
    escreva("\n--- Forma de Pagamento ---\n")
    escreva("1 - PIX\n")
    escreva("2 - Dinheiro\n")
    escreva("3 - Cartão de Crédito\n")
    escreva("Escolha o pagamento (1 a 3): ")
    leia(opcao_pagamento)

    escolha(opcao_pagamento) {
      caso 1: pagamento = "PIX" pare
      caso 2: pagamento = "Dinheiro" pare
      caso 3: pagamento = "Cartão de crédito" pare
      caso contrario: pagamento = "Não definido (Opção inválida)"
    }

    // 5. MENU DA GRADE HORÁRIA
    escreva("\n--- Grade Horária ---\n")
    escreva("1 - Seg, Qua e Sex às 08h\n") 
    escreva("2 - Seg, Qua e Sex às 12h\n") 
    escreva("3 - Seg, Qua e Sex às 20h\n") 
    escreva("4 - Ter e Qui -  12h\n")
    escreva("5 - Ter e Qui - 20h30\n")
    escreva("Escolha o horário (1 a 5): ")
    leia(opcao_horario)

    escolha(opcao_horario) {
    caso 1: horario = "Seg, Qua e Sex - 08h" pare
    caso 2: horario = "Seg, Qua e Sex - 12h" pare
    caso 3: horario = "Seg, Qua e Sex - 20h" pare
    caso 4: horario = "Ter e Qui - 12h" pare
    caso 5: horario = "Ter e Qui - 20h30" pare
    caso contrario: horario = "Não definido (Opção inválida)" 
    }

    // 6. IMPRESSÃO DO RESUMO DO CADASTRO
    escreva("\n===================================\n")
    escreva("   CADASTRO REALIZADO COM SUCESSO!   \n")
    escreva("\n===================================\n")
    escreva("Aluno: ", nome, "| Idade: ", idade, "anos\n")
    escreva("E-mail: ",email, "\n")
    escreva("Contato de Emergência: ", contato_responsavel, "\n")
    escreva("Informações Médicas: ", info_medica, "\n")
    escreva("---------------------------------------------------\n")
    escreva("Plano escolhido: ", plano, "\n")
    escreva("Forma de pagamento: ", pagamento, "\n")
    escreva("Horário dos Treinos: ", horario,"\n")
    escreva("===================================================\n")
    escreva("Bem vindo(a) à Gracie Barra! Oss!\n")
  }
}
