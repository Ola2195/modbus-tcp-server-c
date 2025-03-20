# Modbus TCP Server

This is a simple implementation of a **Modbus TCP server** written in **C**. It supports basic Modbus communication with a single client. The server listens on a specified IP address and port, and handles Modbus requests such as reading and writing to registers.

## Features
- **Single Client Support**: The server can handle only one client connection at a time.
- **Modbus Register Mapping**: Supports mapping of registers to handle Modbus requests.
- **Debugging Output**: Debug information can be enabled to monitor requests and responses.
- **Command Line Options**: Configurable server settings such as IP address, port, and number of registers.

## Requirements
- **libmodbus**: A library for Modbus protocol support.
- **gcc** or any compatible C compiler.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/modbus-server.git
   ```

2. Install the required dependencies:
   - On Linux:
     ```bash
     sudo apt-get install libmodbus-dev
     ```

3. Compile the project:
   ```bash
   gcc modbus_server.c -o modbus_server -lmodbus
   ```

4. Run the server:
   ```bash
   ./modbus_server -i 192.168.1.100 -p 502 -r 10 --debug
   ```

## Command Line Options
- `-h, --help`: Show help message.
- `-v, --version`: Show version information.
- `-i IP`: Set the server IP address (default: `0.0.0.0`).
- `-p PORT`: Set the server port (default: `502`).
- `-r REG_COUNT`: Set the number of registers (default: `10`).
- `--debug`: Enable debug output (default: off).

## Example
```bash
./modbus_server -i 192.168.1.100 -p 502 -r 20 --debug
```
---
# Serwer Modbus TCP

Jest to prosta implementacja **serwera Modbus TCP** napisana w **C**. Obsługuje podstawową komunikację Modbus z jednym klientem. Serwer nasłuchuje na określonym adresie IP i porcie, oraz obsługuje zapytania Modbus, takie jak odczyt i zapis do rejestrów.

## Funkcje
- **Wsparcie dla jednego klienta**: Serwer może obsługiwać tylko jedno połączenie z klientem w tym samym czasie.
- **Mapowanie rejestrów Modbus**: Obsługuje mapowanie rejestrów w celu obsługi zapytań Modbus.
- **Wyniki debugowania**: Możliwość włączenia informacji debugujących w celu monitorowania zapytań i odpowiedzi.
- **Opcje wiersza poleceń**: Konfigurowalne ustawienia serwera, takie jak adres IP, port i liczba rejestrów.

## Wymagania
- **libmodbus**: Biblioteka do obsługi protokołu Modbus.
- **gcc** lub inny kompatybilny kompilator C.

## Instalacja

1. Sklonuj to repozytorium:
   ```bash
   git clone https://github.com/yourusername/modbus-server.git
   ```

2. Zainstaluj wymagane zależności:
   - Na systemach Linux:
     ```bash
     sudo apt-get install libmodbus-dev
     ```

3. Skompiluj projekt:
   ```bash
   gcc modbus_server.c -o modbus_server -lmodbus
   ```

4. Uruchom serwer:
   ```bash
   ./modbus_server -i 192.168.1.100 -p 502 -r 10 --debug
   ```

## Opcje wiersza poleceń
- `-h, --help`: Pokaż komunikat pomocy.
- `-v, --version`: Pokaż informacje o wersji.
- `-i IP`: Ustaw adres IP serwera (domyślnie: `0.0.0.0`).
- `-p PORT`: Ustaw port serwera (domyślnie: `502`).
- `-r REG_COUNT`: Ustaw liczbę rejestrów (domyślnie: `10`).
- `--debug`: Włącz tryb debugowania (domyślnie: wyłączony).

## Przykład
```bash
./modbus_server -i 192.168.1.100 -p 502 -r 20 --debug
```
