# FUNDAMENTOS-DE-PROGRAMACION-
ITS A DEMO! :)
hola como esta!!
Viva la maracuya
ahora si nos pusimos serios, intento de intercambio de moneda de soles a dolares, o al reves nose


# Sistema simple de cambio de soles a dólares

def convertir_soles_a_dolares(soles, tipo_cambio):
    dolares = soles / tipo_cambio
    return dolares

def main():
    print("=== Conversor de Soles a Dólares ===")
    
    try:
        soles = float(input("Ingresa la cantidad en soles (PEN): "))
        tipo_cambio = float(input("Ingresa el tipo de cambio (PEN a USD): "))
        
        dolares = convertir_soles_a_dolares(soles, tipo_cambio)
        
        print(f"\nEquivalente en dólares: ${dolares:.2f} USD")
    
    except ValueError:
        print("Error: Ingresa valores numéricos válidos.")

if __name__ == "__main__":
    main()
