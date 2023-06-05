# Desafio-DIO

def soma_horas(hora1, hora2):
    # quebra as strings em horas e minutos
    h1, m1 = map(int, hora1.split(':')[:2])
    h2, m2 = map(int, hora2.split(':')[:2])

soma as horas e os minutos
    total_minutos = (h1 + h2) * 60 + m1 + m2

converte o total de minutos de volta para o formato "HH:MM"
    horas = total_minutos // 60
    minutos = total_minutos % 60

formata a hora com 2 dígitos para cada componente
    return f"{horas:02d}:{minutos:02d}"
hora1 = "02:30"
hora2 = "04:30"
resultado = soma_horas(hora1, hora2)
print(resultado)
