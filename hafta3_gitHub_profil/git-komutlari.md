 # 📌 Git Komutları - Türkçe | Almanca | İngilizce

 Aşağıda, yaygın olarak kullanılan Git komutlarının Türkçe, Almanca ve İngilizce karşılıklarının yer aldığı birkaç örnek bulabilirsiniz.

> **📝 Not:** Komutları terminalde kullanırken `<file>` veya `<branch>` gibi alanları kendi dosya/dal ismine göre değiştirmek gerekir.

---

## 📌 Temel Git Komutları
| Git Komutu          | Türkçe Açıklama                           | Almanca Açıklama                           | İngilizce Açıklama                      |
|---------------------|------------------------------------------|------------------------------------------|------------------------------------------|
| `git init`         | Yeni bir Git deposu başlatır.             | Ein neues Git-Repository initialisieren. | Initialize a new Git repository.         |
| `git clone <repo>` | Mevcut bir depoyu klonlar.                | Ein vorhandenes Repository klonen.       | Clone an existing repository.           |
| `git status`       | Çalışma alanının durumunu gösterir.       | Den Status des Arbeitsbereichs anzeigen. | Show the status of the working directory. |
| `git log`         | Commit geçmişini gösterir.                | Commit-Verlauf anzeigen.                 | Show commit history.                    |

---

## 📌 Dosya İşlemleri
| Git Komutu          | Türkçe Açıklama                           | Almanca Açıklama                           | İngilizce Açıklama                      |
|---------------------|------------------------------------------|------------------------------------------|------------------------------------------|
| `git add <file>`   | Değişiklikleri sahneye ekler.            | Änderungen zur Staging Area hinzufügen. | Add changes to the staging area.        |
| `git commit -m "mesaj"` | Değişiklikleri kaydeder.        | Änderungen festschreiben.                 | Save changes in the repository.         |
| `git rm <file>`    | Dosyayı Git’ten kaldırır.                | Datei aus Git entfernen.                  | Remove a file from Git.                 |

---

## 📌 Dallarla (Branches) Çalışma
| Git Komutu          | Türkçe Açıklama                           | Almanca Açıklama                           | İngilizce Açıklama                      |
|---------------------|------------------------------------------|------------------------------------------|------------------------------------------|
| `git branch`       | Mevcut dalları listeler.                 | Zeigt alle Branches an.                 | List all branches.                      |
| `git branch <isim>` | Yeni bir dal oluşturur.                 | Einen neuen Branch erstellen.            | Create a new branch.                    |
| `git checkout <dal>` | Belirtilen dala geçiş yapar.          | Zu einem bestimmten Branch wechseln.     | Switch to a specified branch.           |
| `git checkout -b <isim>` | Yeni bir dal oluştur ve geçiş yap. | Einen neuen Branch erstellen und wechseln. | Create and switch to a new branch.       |
| `git merge <dal>`  | Belirtilen dalı mevcut dala birleştirir. | Einen Branch mit dem aktuellen zusammenführen. | Merge the specified branch into the current branch. |

---

## 📌 Uzak Depo (Remote) İşlemleri
| Git Komutu          | Türkçe Açıklama                           | Almanca Açıklama                           | İngilizce Açıklama                      |
|---------------------|------------------------------------------|------------------------------------------|------------------------------------------|
| `git remote -v`    | Uzak bağlantıları listeler.               | Liste der Remote-Verbindungen anzeigen.  | List remote connections.                |
| `git remote add origin <url>` | Yeni uzak depo ekler. | Ein neues Remote-Repository hinzufügen. | Add a new remote repository.            |
| `git push`         | Değişiklikleri uzak depoya gönderir.      | Änderungen zum Remote-Repository hochladen. | Push changes to the remote repository. |
| `git pull`         | Güncellemeleri uzak depodan alır.         | Änderungen vom Remote-Repository abrufen. | Fetch and merge changes from the remote repository. |

---

## 📌 Geri Alma ve Reset İşlemleri
| Git Komutu                   | Türkçe Açıklama                                        | Almanca Açıklama                                        | İngilizce Açıklama                                        |
|------------------------------|-------------------------------------------------------|-------------------------------------------------------|-------------------------------------------------------|
| `git reset --hard HEAD~1`    | Son commit'i geri alır.                               | Den letzten Commit zurücksetzen.                     | Undo the last commit.                                 |
| `git revert <commit_id>`     | Belirli bir commit'i geri alır.                      | Einen bestimmten Commit rückgängig machen.           | Revert a specific commit.                            |
| `git stash`                  | Geçici olarak değişiklikleri saklar.                 | Änderungen vorübergehend speichern.                  | Temporarily stash changes.                           |
| `git stash pop`              | Saklanan değişiklikleri geri yükler.                 | Gespeicherte Änderungen wiederherstellen.            | Apply stashed changes.                               |

---

### 📌 Ek Bilgiler
- Daha fazla Git komutu için resmi Git dökümantasyonuna göz atabilirsiniz: [Git Documentation](https://git-scm.com/doc)
- Eğer GitHub kullanıyorsaniz, [GitHub Docs](https://docs.github.com/) üzerinden gelişmiş komutları öğrenebilirsiniz.

