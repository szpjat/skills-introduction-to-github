# Inicjalizacja nowego repozytorium / Initialize a New Repository

## Polski / Polish

### Jak utworzyć i zainicjalizować nowe repozytorium na GitHub

Ten przewodnik pokazuje, jak utworzyć nowe repozytorium na GitHub i przesłać do niego swój kod.

#### Krok 1: Utwórz nowe repozytorium na GitHub

1. Przejdź do [GitHub.com](https://github.com) i kliknij ikonę **+** w prawym górnym rogu
2. Wybierz **New repository**
3. Wprowadź nazwę repozytorium (np. `ProjektFinal`)
4. Wybierz, czy repozytorium ma być publiczne czy prywatne
5. **Nie** inicjalizuj z README, .gitignore ani licencją (ponieważ będziesz przesyłać istniejący kod)
6. Kliknij **Create repository**

#### Krok 2: Połącz lokalne repozytorium z GitHub

W terminalu, w katalogu Twojego projektu, wykonaj następujące polecenia:

```bash
# Dodaj zdalny adres URL repozytorium
git remote add origin https://github.com/TWOJA-NAZWA-UŻYTKOWNIKA/ProjektFinal.git

# Zmień nazwę gałęzi na main (jeśli jeszcze tak nie jest)
git branch -M main

# Wypchnij swój kod na GitHub
git push -u origin main
```

> **Ważne:** Zamień `TWOJA-NAZWA-UŻYTKOWNIKA` na swoją rzeczywistą nazwę użytkownika GitHub w powyższych poleceniach.

#### Co robią te polecenia?

- **`git remote add origin [URL]`**: Łączy Twoje lokalne repozytorium ze zdalnym repozytorium na GitHub. Nazwa "origin" jest domyślną nazwą dla głównego zdalnego repozytorium.
  
- **`git branch -M main`**: Zmienia nazwę bieżącej gałęzi na `main`. Flaga `-M` wymusza zmianę nazwy, nawet jeśli gałąź o nazwie `main` już istnieje.

- **`git push -u origin main`**: Wypycha Twój kod do zdalnego repozytorium. Flaga `-u` ustawia śledzenie, dzięki czemu przyszłe wypychanie i pobieranie będzie łatwiejsze (możesz po prostu użyć `git push` lub `git pull`).

#### Przydatne dodatkowe polecenia

```bash
# Wyświetl wszystkie skonfigurowane zdalne repozytoria
git remote -v

# Wypchnij zmiany do zdalnego repozytorium
git push

# Pobierz najnowsze zmiany ze zdalnego repozytorium
git pull

# Sprawdź stan swojego repozytorium
git status
```

---

## English

### How to Create and Initialize a New Repository on GitHub

This guide shows you how to create a new repository on GitHub and push your code to it.

#### Step 1: Create a New Repository on GitHub

1. Go to [GitHub.com](https://github.com) and click the **+** icon in the top right corner
2. Select **New repository**
3. Enter a repository name (for example: `ProjektFinal`)
4. Choose whether to make it public or private
5. **Do not** initialize with a README, .gitignore, or license (since you'll push existing code)
6. Click **Create repository**

#### Step 2: Connect Your Local Repository to GitHub

In your terminal, navigate to your project directory and run these commands:

```bash
# Add the remote repository URL
git remote add origin https://github.com/YOUR-USERNAME/ProjektFinal.git

# Rename your branch to main (if it's not already)
git branch -M main

# Push your code to GitHub
git push -u origin main
```

> **Important:** Replace `YOUR-USERNAME` with your actual GitHub username in the commands above.

#### What Do These Commands Do?

- **`git remote add origin [URL]`**: Connects your local repository to the remote repository on GitHub. The name "origin" is the default name for the primary remote repository.
  
- **`git branch -M main`**: Renames your current branch to `main`. The `-M` flag forces the rename even if a branch named `main` already exists.

- **`git push -u origin main`**: Pushes your code to the remote repository. The `-u` flag sets up tracking, so future pushes and pulls are easier (you can just use `git push` or `git pull`).

#### Additional Useful Commands

```bash
# View all configured remotes
git remote -v

# Push changes to the remote repository
git push

# Pull the latest changes from the remote repository
git pull

# Check the status of your repository
git status
```

---

## Additional Resources / Dodatkowe zasoby

- [About remote repositories](https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories) - GitHub Docs
- [Creating a new repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository) - GitHub Docs
- [Adding a remote](https://docs.github.com/en/get-started/getting-started-with-git/managing-remote-repositories) - GitHub Docs
