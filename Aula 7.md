AULA 7
1. def grava_nome_em_arquivo():
    nome = input("Por favor, insira seu nome: ")
    with open("nome_usuario.txt", "w") as arquivo:
        arquivo.write(nome)
    print("Nome gravado com sucesso!")

# Chamando a função
grava_nome_em_arquivo()

2) def imprime_conteudo_arquivo():
    nome_arquivo = input("Por favor, insira o nome do arquivo (com extensão): ")
    with open(nome_arquivo, "r") as arquivo:
        conteudo = arquivo.read()
    print("\nConteúdo do arquivo:")
    print(conteudo)

# Chamando a função
imprime_conteudo_arquivo()

3) def copia_conteudo_para_novo_arquivo():
    arquivo_origem = input("Por favor, insira o nome do arquivo de origem (com extensão): ")
    arquivo_destino = input("Por favor, insira o nome do novo arquivo (com extensão): ")

    with open(arquivo_origem, "r") as origem:
        conteudo = origem.read()

    with open(arquivo_destino, "w") as destino:
        destino.write(conteudo)
    
    print(f"Conteúdo copiado de {arquivo_origem} para {arquivo_destino} com sucesso!")

# Chamando a função
copia_conteudo_para_novo_arquivo()

4)def imprime_nome_por_numero():
    nome_arquivo = input("Por favor, insira o nome do arquivo (com extensão): ")
    numero = int(input("Insira um número: "))

    with open(nome_arquivo, "r") as arquivo:
        linhas = arquivo.readlines()

    # Verifica se o número está dentro do intervalo de linhas
    if 1 <= numero <= len(linhas):
        nome = linhas[numero - 1].strip()  # Subtrai 1 para ajustar ao índice 0 e remove espaços em branco
        print(f"O nome correspondente ao número {numero} é: {nome}")
    else:
        print(f"O número {numero} está fora do intervalo de linhas do arquivo.")

# Chamando a função
imprime_nome_por_numero()
