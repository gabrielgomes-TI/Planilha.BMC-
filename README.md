import pandas as pd

# As regras de tipos continuam aqui:
# Nomes e e-mails usam aspas ("String"). Idades e Alturas são números puros (int ou float).
dados_dos_leads = {
    "Nome": ["Gabriel", "Jude Bellingham", "Lucas"],
    "E-mail": ["gabriel@email.com", "bellingham@real.com", "lucas@email.com"],
    "Idade": [24, 23, 19],  # Números matemáticos inteiros (int)
    "Altura": [1.87, 1.86, 1.74]  # Números decimais (float)
}

# O Python organiza tudo em formato de tabelas (DataFrame)
tabela = pd.DataFrame(dados_dos_leads)

# E exporta direto para um arquivo do Excel!
tabela.to_excel("leads_desenvolvimento_negocios.xlsx", index=False)
print("Planilha criada com sucesso!")
