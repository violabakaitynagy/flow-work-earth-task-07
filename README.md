# 7. feladat

> A feladatok megoldása során két fős csapatokban dolgozzatok! Jelöljetek ki egymás között egy csapatkapitányt. Az ő repoját fogjátok majd használni a feladat megoldása során.
>
> Fontos, hogy akkor is segítsétek egymást, amikor éppen csak az egyik csapattagnak vannak lépései! A csapat csak akkor tud sikeres lenni, ha mindenki érti, hogy mit csinál, és miért csinálja azt.

## Csapatkapitány feladatai

1. Hozz létre egy új repot ezt felhasználva template-ként.
2. Hívd meg a csapattársadat a repositoryhoz a GitHub-on a `Settings > Collaborators` menüpont alatt.
3. Klónozd le ezt a repositoryt a `~/flow/git` mappán belülre a `task-07` mappába. (`git clone https://github.com/[github-felhasznalo]/flow-work-earth-task-07 task-07`)

## A csapattárs feladatai

1. Fogadd el a meghívást a GitHub-on a csapatkapitányodtól a jobb felső sarokban megjelenő értesítésre kattintva. Kövesd a lépéseket, amiket a GitHub megjelenít neked.
2. Klónozd le a csapatkapitányod repositoryját a `~/flow/git` mappán belülre a `task-07` mappába. Fontos, hogy itt a repository nem a saját neved alatt lesz! (`git clone https://github.com/[csapatkapitany-github-felhasznaloja]/flow-work-earth-task-07 task-07`)

## Mindkét fél feladatai

1. Hozzatok létre egy-egy branchet a `main` branchből a saját **GitHub felhasználónevetekkel**. (`git branch <name>`)
2. Váltsatok át erre a branchre. (`git checkout <name>`)
3. Osszátok szét egymás között az alábbi feladatokat, majd mindenki a saját branchére dolgozzon:

> A `rendelesek.md` fájlban láttok egy szekciót, ahol az egyes termékek azonosítójának, nevének, illetve vásárolt mennyiségeknek kell szerepelnie.
>
> Az alábbi feladatokat osszátok ki egymás között:
>
> - A csapat egyik tagjának a feladata az, hogy az első és második termék azonosítóját a termék neve elé, a harmadik és negyedik termék mennyiségét pedig a termék neve mögé beírja.
> - A másik csapattagnak a feladata az, hogy a harmadik és negyedik termék azonosítóját a termék neve elé, az első és második termék mennyiségét pedig a termék neve mögé beírja.
>
> Használjátok a fájlban lévő táblázatot arra, hogy a megfelelő helyre beírjátok az adatokat!

4. Commitoljátok a változtatásaitokat. (`git add -A`, majd `git commit -m "<message>"`)
5. Hozzatok létre egy-egy pull requestet a saját branchetekből a `main` branchbe, és jelöljétek be egymást reviewernek.
6. Nézzétek meg egymás pull requestjét, és ha szükséges, akkor írjatok kommentet, vagy kérdezzetek rá a megoldásra a GitHubon keresztül.
7. Amennyiben valamelyik fél megoldásában hibát találtok, próbáljátok meg közösen kijavítani azt egymást segítve.
8. Ha mindent rendben találtok, akkor az első feladatért felelős személy mergelheti a saját pull requestjét a `main` branchbe.
9. ⚠️ Ezen a ponton a második feladat pull requestje conflictot fog generálni. Közösen javítsátok ki a problémát, és mergeljétek a második feladat pull requestjét is a `main` branchbe. Ezt a GitHub felületén keresztül is meg tudjátok akár tenni. Figyeljetek rá, hogy mindkettőtök változtatása bekerüljön a `main` branchbe!

## Segítség

### Példa az első feladat megoldására

```
| Rendelés azonosítója | Termék azonosítója | Mennyiség (kg) |
| -------------------- | ------------------ | -------------- |
| 1                    | 1                  | 15             |
| 2                    | 4                  | 5              |
| 3                    | 2                  | 20             |
| 4                    | 3                  | 10             |

## Vásárolt mennyiség

1 - Alma:
2 - Brokkoli:
Narancs: 10 kg
Paradicsom: 5 kg
```

### Példa a második feladat megoldására

```
| Rendelés azonosítója | Termék azonosítója | Mennyiség (kg) |
| -------------------- | ------------------ | -------------- |
| 1                    | 1                  | 15             |
| 2                    | 4                  | 5              |
| 3                    | 2                  | 20             |
| 4                    | 3                  | 10             |

## Vásárolt mennyiség

Alma: 15 kg
Brokkoli: 20 kg
3 - Narancs:
4 - Paradicsom:
```

### Példa a konfliktus feloldására

```
| Rendelés azonosítója | Termék azonosítója | Mennyiség (kg) |
| -------------------- | ------------------ | -------------- |
| 1                    | 1                  | 15             |
| 2                    | 4                  | 5              |
| 3                    | 2                  | 20             |
| 4                    | 3                  | 10             |

## Vásárolt mennyiség

1 - Alma: 15 kg
2 - Brokkoli: 20 kg
3 - Narancs: 10 kg
4 - Paradicsom: 5 kg
```
