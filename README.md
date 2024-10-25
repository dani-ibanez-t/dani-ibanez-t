import os 
os. system ("cls")
cant_tarta_de_manzana=0
cant_cheeseacake_de_frambuesa=0
cant_pastel_de_chocolate=0
cant_galletas_de_avena=0
cant_macarons_docena =0

while True : 
    print("====Dulces encantos====")
    print("tarta de manzana ")
    print("cheesecake de frambuesa ")
    print("pastel de chocolate ")
    print("galletas de avena ")
    print("macarons docena ")

    opcion = int (input ("seleciona una de las alternativas del menu" ))

    if opcion == 1 : 
        cant_tarta_de_manzana+= int (input("indica la cantidad de tarta de manzana que deseas" ))
    elif opcion ==2:
        cant_cheeseacake_de_frambuesa+= int (input("indica la cantidad de cheesecake de frambuesa que deseas" ))
    elif  opcion == 3:
        cant_pastel_de_chocolate+= int (input("indica la cantidad de pastel de chocolate que deseas" ))
    elif opcion== 4:
            cant_galletas_de_avena+= int (input("indica la cantidad de galletas de avena que deseas" ))
    elif opcion == 5:
            cant_macarons_docena+= int (input("indica la cantidad de macarons que deseas" ))

    else : 
        print ("opcion no valida ")

    continuar = int (input("desea algo mas ? 1: si 2 no : "))
    if continuar == 2:
        
     break
  

os.system ("cls")
print("== elige el descuento ==")
print("1.cliente premium 20%")
print("2.estudiante 15%")
print("3.no posee descuento 0%")
print("--------------------------------")
opcion_descuento = int(input("ingresa una opcion > "))
if opcion_descuento == 1 : 
    descuento = 0.20
elif opcion_descuento == 2: 
     descuento = 0.15
elif opcion_descuento == 3:
     descuento = 0 
else: 
     print("elija una opcion valida")
print("-----------------------------------")
os.system("cls")
print("====== dulces encantos ======")
print (cant_tarta_de_manzana,"tarta de manzana$" ,cant_tarta_de_manzana *8000 )
print (cant_cheeseacake_de_frambuesa ,"cheeseacake de frambuesa $" ,cant_cheeseacake_de_frambuesa*9000 )
print (cant_pastel_de_chocolate,"pastel de chocolate $" ,cant_pastel_de_chocolate *7500 )
print (cant_galletas_de_avena,"galletas de avena$" ,cant_galletas_de_avena *5000 )
print (cant_macarons_docena,"macarons docena  $" ,cant_macarons_docena *12000 )
print("------------------------------------------------")
subtotal = cant_tarta_de_manzana*8000 + cant_cheeseacake_de_frambuesa*9000 + cant_pastel_de_chocolate*7500 + cant_galletas_de_avena*5000 * cant_macarons_docena*12000
print("subtotal: $" , subtotal)
print("descuento: $" , subtotal*descuento)
total = subtotal-(subtotal*descuento)
print("--------------------------------------------------")
print("total: $" , total)

print("======== ¡gracias por su compra! :D ========")



