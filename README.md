
caja = 0
                                                                  #UPGRADE!!
print ("\n Juego de dados")
caja = int ( input ('\n Cuantas fichas queres? '))
usuario = input ("Nombre del jugador: ")
print ('Hola',usuario)                    #INICIO DEL JUEGO DE 
apuesta = int ( input  ('Cuanto queres apostar?: '))
while  apuesta >caja:
      print ('No tienes esa cantidad de fichas.')
      input ()
      caja = int ( input ('\n Cuantas fichas queres? '))
      apuesta = int ( input  ('Cuanto queres apostar?: '))
if apuesta <caja:
      print ('Apostaste', apuesta )

elif apuesta ==caja:
      print ('Apostaste', apuesta  )    

eleccion = str (input ('Par o impar?'))
print ("Pesiona ENTER para jugar.")
input () 

import random
dado1 = random.randint (1,6)
dado2 = random.randint (1,6)               
print ("Tirando dados..")                 #TIRADERA DE DADOS
print ("Han salido ",dado1,'y',dado2)
total = dado1 + dado2
resto = total%2
print (total)

if total % 2 == 0 and eleccion.upper() == "PAR":
      print("Tu eleccion fue certera")
      caja = apuesta * 2 
      print ('Te quedan ',caja,'fichas en la caja')

elif total % 2 != 0 and eleccion.upper() == "IMPAR":    #CONDICIONES
      print("Tu eleccion fue certera")                      #VERIFICACION CON LA ELECCION DEL USUARIO 
      caja = apuesta * 2
      print ('Te quedan ',caja,'fichas en la caja')
else:
      print("Tu eleccion NO fue la correcta")
      caja - apuesta
      print ('Te quedan ',apuesta,'fichas en la caja')
      


