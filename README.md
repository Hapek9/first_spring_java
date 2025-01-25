# First-Project-Java-Spring

Prosty projekt stworzony w oparciu o **Spring Boot**, prezentujący podstawy wzorca **MVC** (Model-View-Controller).  
Aplikacja uruchamia serwer HTTP (port domyślny: `8080`) i udostępnia dwa endpointy:
- `/` – zwraca prosty tekst w przeglądarce,  
- `/greeting` – renderuje widok Thymeleaf (plik `greeting.html`) z parametrem `name`.  

## Wymagania
- Java w wersji zgodnej z projektem (np. 17 lub 19)  
- Maven (do pobrania zależności, budowania oraz uruchamiania projektu)  

## Uruchomienie aplikacji

1. **Klonowanie/rozpakowanie** projektu:
   - Jeśli pobierasz z [start.spring.io](https://start.spring.io/), rozpakuj wygenerowane archiwum `.zip`.
   - Jeśli pobierasz z repozytorium, sklonuj je do lokalnego folderu.
2. **Import** projektu do IDE (np. IntelliJ, Eclipse, VS Code) lub przejdź do głównego folderu projektu w terminalu.
3. **Budowanie i uruchamianie**:
   - W IDE: uruchom metodę `main()` w klasie `FirstProjectJavaSpringApplication`.
   - W terminalu:  
     ```bash
     mvn spring-boot:run
     ```
4. Po pomyślnym starcie aplikacja nasłuchuje na adresie:
http://localhost:8080

markdown
Kopiuj
Edytuj

## Korzystanie z aplikacji

- **Endpoint główny**:  
http://localhost:8080/

yaml
Kopiuj
Edytuj
Wyświetla w przeglądarce tekst:  
Hello Vistula, in my first Spring controller.

markdown
Kopiuj
Edytuj
- **Endpoint z widokiem**:  
http://localhost:8080/greeting?name=Vistula

java
Kopiuj
Edytuj
Renderuje plik `greeting.html` (z użyciem Thymeleaf).  
- W widoku pojawi się komunikat „Hello, Vistula!” oraz przykładowy obrazek (jeśli został dodany do folderu `static/images/`).
