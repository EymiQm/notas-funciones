# notas-funciones

 cliente = {
        "id": id_cliente,
        "nombre": nombre,
        "edad": edad,
        "plan": plan,
        "estado": estado
    }

    clientes.append(cliente)
    guardar_clientes(clientes)
    print("Cliente creado")

except:
    print("Error en los datos")
    
    for c in clientes:
    print(c)
    
    for c in clientes:
    if str(c["id"]) == dato or c["nombre"].lower() == dato.lower():
        print("Encontrado:", c)
        return

print("Cliente no encontrado")

for c in clientes:
    if c["id"] == id_cliente:
        c["nombre"] = input("Nuevo nombre: ")
        c["edad"] = int(input("Nueva edad: "))
        c["plan"] = input("Nuevo plan: ")
        c["estado"] = input("Nuevo estado: ")

        guardar_clientes(clientes)
        print("Cliente actualizado")
        return

print("Cliente no encontrado")

for c in clientes:
    if c["id"] == id_cliente:
        clientes.remove(c)
        guardar_clientes(clientes)
        print("Cliente eliminado")
        return

print("Cliente no encontrado")

def menu(): clientes = cargar_clientes()

while True:
    print("\n--- MENÚ ---")
    print("1. Crear cliente")
    print("2. Listar clientes")
    print("3. Buscar cliente")
    print("4. Actualizar cliente")
    print("5. Eliminar cliente")
    print("6. Salir")

    opcion = input("Elige una opción: ")

    if opcion == "1":
        crear_cliente(clientes)
    elif opcion == "2":
        listar_clientes(clientes)
    elif opcion == "3":
        buscar_cliente(clientes)
    elif opcion == "4":
        actualizar_cliente(clientes)
    elif opcion == "5":
        eliminar_cliente(clientes)
    elif opcion == "6":
        print("Saliendo...")
        break
    else:
        print("Opción inválida")
        
        menu()

