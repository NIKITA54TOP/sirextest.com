<div align="center">

# SportaKlubs

**Sporta kluba klientu sistēma**

![Java](https://img.shields.io/badge/Java-21-orange?style=for-the-badge&logo=openjdk&logoColor=white)
![NetBeans](https://img.shields.io/badge/NetBeans-GUI_Builder-1B6AC6?style=for-the-badge&logo=apachenetbeanside&logoColor=white)
![Derby](https://img.shields.io/badge/Apache_Derby-DB-blue?style=for-the-badge&logo=apache&logoColor=white)
![JUnit](https://img.shields.io/badge/JUnit-4-25A162?style=for-the-badge&logo=junit5&logoColor=white)

*2. projekta darbs · 8. tēma · DTTT · PR-32 · 2026./2027.*

</div>

---

### 👥 Autori

<table>
  <tr>
    <td align="center"><a href="https://github.com/NIKITA54TOP"><img src="https://github.com/NIKITA54TOP.png" width="80"><br><b>Nikita Novikovs</b></a><br><sub>@NIKITA54TOP</sub></td>
    <td align="center"><a href="https://github.com/volconokbeta-cell"><img src="https://github.com/volconokbeta-cell.png" width="80"><br><b>Vadims Kožuhovskis</b></a><br><sub>@volconokbeta-cell</sub></td>
  </tr>
</table>

---

### 🔐 Pieslēgšanās

<table>
  <tr>
    <th>👑 Administrators</th>
    <th>🙋 Testa klienti</th>
  </tr>
  <tr>
    <td>

| Lietotājvārds | Parole |
|---|---|
| `admin` | `admin123` |

Pilnas tiesības: klienti, treneri,<br>abonementi, grafiks, maksājumi.

</td>
    <td>

| Lietotājvārds | Parole |
|---|---|
| `janis` | `janis123` |
| `anna` | `anna123` |
| `peteris` | `peteris123` |

</td>
  </tr>
</table>

---

### 🚀 Ātrā palaišana

```text
1. NetBeans → File → Open Project → SportaKlubs
2. Run Project (F6)
3. Pieslēdzieties ar admin / admin123
```

> [!TIP]
> Nekas papildus nav jāinstalē – bibliotēkas ir mapē `lib`, datu bāze ar testa datiem – mapē `database`.

---

<details>
<summary><b>🗄️ Datu bāze</b></summary>
<br>

| | |
|---|---|
| DBVS | Apache Derby (Embedded) |
| Atrašanās vieta | `database/sportaklubsDB` (glabājas repozitorijā) |
| Tabulas | USERS, CLIENTS, TRAINERS, MEMBERSHIPS, TRAININGS, BOOKINGS, PAYMENTS |
| Teksta eksports | `database/eksports/*.csv` – atjaunojas, aizverot programmu |
| SQL skripts | `sql/sportaklubs.sql` |

</details>

<details>
<summary><b>📁 Projekta struktūra</b></summary>
<br>

```
src/lv/sportaklubs/
├── gui/     MainFrame, Ui, HelpText
├── dao/     ClientDAO, TrainerDAO, MembershipDAO, ...
├── model/   Client, Trainer, Membership, ...
├── db/      DBConnection, TestData, DataExport
└── util/    Session, Validator, PasswordUtil
```

</details>
