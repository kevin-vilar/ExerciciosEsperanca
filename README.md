# ExerciciosEsperanca

def divisores(n):
	a=2
	div=[]
	while n/2 >= a:
		if n%a == 0:
			div.append(a) 
		a = a+1
	return div

def consoantes(s):
	listconsoantes = []
	consoantes = ['b','c','d','f','g','h','j','k','l','m','n','p','q','r','s','t','v','w','y','x','z']
	for i in s:
		if i in consoantes:
			listconsoantes.append(i)
	return list(set(listconsoantes))

def comuns (a,b):
	lista=[]
	for i in a:
		if not i in lista:
			if a.count(i)>b.count(i):
				lista = lista + [i]*b.count(i)
			else:
				lista = lista + [i]*a.count(i)
	return lista

def naocomuns(a,b):
	lista = []
	for i in a :
		if not i in b:
			lista = lista + [i]
	for j in b :
		if not j in a:
			lista = lista + [j]
	return lista
