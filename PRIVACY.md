# Privacy Policy – NN PowerTools

_Last updated: 8 October 2026_

NN PowerTools ("the app") is an unofficial, independent Windows client for the
My2N cloud. It is not affiliated with, endorsed by, or connected to
2N Telekomunikace a.s. The app is simply another view of the same My2N API that
the my2n.com web portal uses.

## Summary

**The developer does not collect, receive, store, sell, or share any of your data.**
The app has no developer-operated server and uses no analytics, telemetry,
advertising, or tracking.

## Your My2N sign-in

- You sign in with your existing My2N account. Your email and password are sent
  directly from your computer to My2N's own sign-in service (`auth.my2n.com`)
  over HTTPS, the same way as when you sign in on my2n.com.
- By default the app does **not** save your password. If you tick "Remember
  login", your email and password are saved in Windows Credential Manager
  (encrypted under your Windows account) so the app can sign you in on the next
  start. They never leave your computer except to sign in at `auth.my2n.com`.
  Unticking the box deletes them.
- The session token that My2N returns is kept in memory only while the app is
  running and is discarded when you close it.

## Data shown and edited in the app

Site users, their names and emails, apartments, RFID cards, licence plates,
and devices are loaded from and saved to your My2N account (`my2n.com`), and
only through your own signed-in session. The app only shows and changes what
your My2N account is already allowed to access on my2n.com. That data is
processed by 2N Telekomunikace a.s. under
[their privacy policy](https://www.2n.com), not by
this app's developer.

## Local network and devices

- **Device discovery:** the app uses mDNS/Bonjour to find 2N devices on your
  local network. This traffic stays on your local network.
- **Device access:** when you choose to connect to a 2N device, the app talks
  to that device directly (or through the My2N remote-access address) using the
  device credentials you enter. Those credentials are not saved.
- **Card reader:** when you use an Elatec TWN4 reader to encrypt MIFARE DESFire
  cards, the app talks only to the reader connected to your computer. The
  encryption keys are derived from a passphrase you type in. Neither the
  passphrase nor the keys are saved.

## What is stored on your computer

The app stores only these items, and only on your computer:

- `%LocalAppData%\NN PowerTools\config.json`: app settings (the DESFire
  application ID and which certificate authority is active). It contains no
  personal data or credentials.
- **Windows certificate store:** certificate authority certificates that you
  create or import in the app are saved in your Windows user certificate store.
- **Windows Credential Manager** (only if you tick "Remember login"): your My2N
  email and password, see above.
- **Optional debug log** (off by default, and turned off again every time the
  app starts): when you turn it on in Settings, the app writes its network
  requests and responses to a log file in the same folder so you can
  troubleshoot. Passwords, tokens, PINs, card codes, and keys are masked. The
  log can still contain names or emails returned by the API. If the app crashes,
  the error details (a technical stack trace) are written to the same file even
  when the log is off. It is never sent anywhere. You can clear it in Settings
  or delete the file.

Uninstalling the app and deleting the `%LocalAppData%\NN PowerTools` folder
removes everything listed above.

## Children

The app is a professional administration tool and is not directed at children.

## Changes

If this policy changes, the updated version will be published at this same
address with a new "Last updated" date.

## Contact

Please open an issue at https://github.com/kv-0000/nn-powertools-support/issues

---

# Zásady ochrany osobních údajů – NN PowerTools (česky)

**Vývojář nesbírá, nepřijímá, neukládá, neprodává ani nesdílí žádná vaše data.**
Aplikace nemá žádný vlastní server a nepoužívá žádnou analytiku, telemetrii,
reklamu ani sledování.

- **Přihlášení:** e-mail a heslo k My2N účtu se posílají přímo z vašeho počítače
  na přihlašovací službu My2N (`auth.my2n.com`) přes HTTPS, stejně jako při
  přihlášení na my2n.com. Heslo se ve výchozím stavu neukládá. Když zaškrtnete
  „Zapamatovat přihlášení“, uloží se e-mail a heslo do Správce přihlašovacích
  údajů Windows (šifrovaně pod vaším Windows účtem), aby se aplikace při dalším
  spuštění přihlásila sama. Odškrtnutím se smažou. Session
  token je jen v paměti a po zavření aplikace zanikne.
- **Data v aplikaci:** uživatelé, RFID karty, registrační značky a zařízení se
  načítají z vašeho My2N účtu (`my2n.com`) a ukládají se zpět do něj, vždy jen
  přes vaše přihlášení a jen v rozsahu, který má váš účet na my2n.com.
  Zpracovatelem těchto dat je 2N Telekomunikace a.s. podle
  [jejích zásad](https://www.2n.com).
- **Lokální síť a čtečka:** vyhledávání zařízení (mDNS) probíhá jen v lokální
  síti. Přihlašovací údaje k zařízením, fráze ani klíče karet DESFire se
  neukládají.
- **Uloženo jen ve vašem počítači:**
  - `%LocalAppData%\NN PowerTools\config.json`: nastavení, bez osobních údajů.
  - Certifikáty CA ve Windows úložišti certifikátů.
  - Jen se zaškrtnutým „Zapamatovat přihlášení“: e-mail a heslo k My2N ve
    Správci přihlašovacích údajů Windows.
  - Volitelný ladicí log: výchozí stav je vypnuto, citlivé hodnoty jsou
    maskované a nikam se neodesílá. Při pádu aplikace se do něj zapíše
    technický popis chyby i s vypnutým logem.

Aplikace je neoficiální nástroj nezávislého vývojáře a není spojena ani
přidružena k 2N Telekomunikace a.s.

Kontakt: založte issue na https://github.com/kv-0000/nn-powertools-support/issues
