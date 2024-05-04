# calculadora-descuentos
nombre = input("Ingrese su nombre: ")
edad = int(input("Ingrese su edad: "))
trabajador_estudiante = input("¿Es usted trabajador o estudiante?: ")

precio_pasaje = 860

trabajador_estudiante = trabajador_estudiante.lower()



if edad >= 65:
    descuento = 0.6  
elif trabajador_estudiante == "estudiante":
    descuento = 0.5 
elif trabajador_estudiante == "trabajador":
    descuento = 0.15  
else:
    descuento = 0   


precio_final = precio_pasaje * (1 - descuento)


print("Hola {}, el precio final de su pasaje es: ${:.2f}".format(nombre, precio_final))

