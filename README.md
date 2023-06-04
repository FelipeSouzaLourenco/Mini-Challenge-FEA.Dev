# Mini Challenge FEA.Dev
 import random

nomes = nomes = ["André", "Fernanda Mees", "Gabriel", "Henrique", "Ana", "Amanda", "Adriel", "Felipe", "Fernanda Mayumi", "Guilherme", "Kim", "Leticia", "Marcelo", "Mateus", "Milena", "Paulo", "Theo", "Vitor", "Maria"]
exclusivos = ['André', 'Fernanda Mees', 'Gabriel', 'Henrique']
random.shuffle(nomes)  # Embaralha a lista de nomes

grupo1 = random.sample([nome for nome in nomes if nome not in ['André', 'Fernanda Mees', 'Gabriel', 'Henrique']], 4) + random.sample(exclusivos, 1)
nomes = [nome for nome in nomes if nome not in grupo1]
exclusivos = [nome for nome in exclusivos if nome not in grupo1]
grupo2 = random.sample([nome for nome in nomes if nome not in ['André', 'Fernanda Mees', 'Gabriel', 'Henrique']], 4) + random.sample(exclusivos, 1)
nomes = [nome for nome in nomes if nome not in grupo2]
exclusivos = [nome for nome in exclusivos if nome not in grupo2]
grupo3 = random.sample([nome for nome in nomes if nome not in ['André', 'Fernanda Mees', 'Gabriel', 'Henrique']], 4) + random.sample(exclusivos, 1)
nomes = [nome for nome in nomes if nome not in grupo3]
exclusivos = [nome for nome in exclusivos if nome not in grupo3]
grupo4 = random.sample([nome for nome in nomes if nome not in ['André', 'Fernanda Mees', 'Gabriel', 'Henrique']], 3) + random.sample(exclusivos, 1)
nomes = [nome for nome in nomes if nome not in grupo4]
exclusivos = [nome for nome in exclusivos if nome not in grupo4]

print("Grupo 1:", grupo1)
print("Grupo 2:", grupo2)
print("Grupo 3:", grupo3)
print("Grupo 4:", grupo4)


