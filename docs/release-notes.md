## v0.5.4 July 13, 2020
- Devices: (⚠️ Experimental) Support Bitcoin Core hot wallets (#210) (@ben-kaufman)
- Bugfix: Fix issues with Bitcoin Core calls timing out (#214) (@stepansnigirev)
- Bugfix: Fix issues with non standard keys (#209) (@stepansnigirev)
- Refactoring: Refactor HWI Javascript code (#213) (@stepansnigirev)
- UI: Add new exception handler page to give information about errors (#211) (@stepansnigirev)
- UI: Improve keys table (#218) (@stepansnigirev)

## v0.5.3 July 10, 2020
- Bugfix: Fix potential crashes and issues due to multi-threading race conditions (#205) (@stepansnigirev)
- Bugfix: Fix crash if current Specter version could not be obtained (#202) (@stepansnigirev)
- Bugfix: Fix potential issue with wallets not being properly loaded (#197) (@ben-kaufman)
- Feature: User management panel for admin to manage the list of existing users (in multi-user mode) (#194) (@ben-kaufman)
- UI: Fix notification UI in coin-selection and login screens (#192, #195) (@stepansnigirev)
- UI: Fix some notification messages showing up as error messages (#193) (@ben-kaufman)
- UI: List the devices used in a wallet and the wallets using a certain device (#196) (@ben-kaufman)
- UI: Allow changing device type and warn if non was selected on device setup (#201) (@ben-kaufman)
- UI: Clarify why funds are not available when already used in an unsigned transaction and how to free them (#204) (@ben-kaufman)
- UI: Indicate selected device on the sidebar (#206) (@stepansnigirev)

## v0.5.2 July 5, 2020
- Devices: [Cobo Valut](https://cobo.com/hardware-wallet/cobo-vault) single-sig support (#189) (@stepansnigirev)
- Devices: Support Specter-DIY [v1.2.0](https://github.com/cryptoadvance/specter-diy/releases/tag/v1.2.0) (#188) (@stepansnigirev)
- Bugfix: Fix issue with wallets and devices not being loaded properly (#190) (@ben-kaufman)
- Bugfix: Return button to display address on device for Ledger single-sig wallets (#187) (@stepansnigirev)
- Bugfix: Allow same origin requests to HWI Bridge by default (#185) (@stepansnigirev)
- Bugfix: Fix authentication and styles issues (#181) (@stepansnigirev)
- UI: Improve sidebar UI when Bitcoin Core is not connected or not configured (#184) (@stepansnigirev)

## v0.5.1 (v0.5.0 Hotfix) June 30, 2020
- Bugfix: Fix issue with running Specter after installing from pip (@stepansnigirev)

## v0.5.0 June 30, 2020
- Bugfix: Fix compatibility issue with latest Ledger and Trezor firmwares (addresses new BIP143 vulnerability), use HWI 1.1.2 (#178) (@stepansnigirev)
- Bugfix: Don't update explorer if chain is unknown (#174) (@stepansnigirev)
- Bugfix: Fix labels issue with Bitcoin Core v0.20.0 (#160) (@ben-kaufman)
- Feature: Multi-user support (#172) (@ben-kaufman)
- Feature: Import-export PSBT transactions (#175) (@stepansnigirev)
- Feature: Support HWI display multisig address on device (ColdCard, KeepKey, Trezor) (#179) (@ben-kaufman)
- UI: Show installed Specter version and notify on upgrades on the Setting page. (#158) (@k9ert)
- UI: Redesign and improve notifications and error messages (#177, #163) (@stepansnigirev)
- UI: Separate the different areas in the Settings screen into tabs. (#176) (@ben-kaufman)
- UI: Add copy button for QR codes (#173) (@stepansnigirev)
- UI: Change confusing “Pending PSBTs” terminology to “Unsigned PSBTs” (#171) (@ben-kaufman)
- UI: Improve signing UI (#175, #160) (@stepansnigirev, @ben-kaufman)
- UI: Add reject reason to the error on broadcast (#160) (@stepansnigirev)
- UI: New Trezor and Ledger icons (#160) (@stepansnigirev, @ben-kaufman)
- UI: Allow selecting device type manually (#160) (@ben-kaufman)
- Refactoring: Separate `logic.py` into multiple files (#160) (@ben-kaufman)
- Refactoring: Refactor Device, DeviceManager, Wallet, WalletManager classes (#160) (@ben-kaufman)
- Refactoring: Modularize supported device types (#160) (@ben-kaufman)
- Refactoring: Make devices and wallets accessible to each other (#160) (@ben-kaufman)
- Test: Improve test coverage for: Device, DeviceManager, Wallet, WalletManager classes (#160, #170) (@ben-kaufman)
- Test: Support multiple Bitcoin Core versions (#161) (@k9ert)
- Docs: Create FAQ doc (#151) (@kkdao)
- Docs: FAQ table of contents auto-generation (#165) (@k9ert)
- Docs: README updates (#164) (@moritzwietersheim)

## v0.4.0 May 31, 2020
- #112 - Mobile friendly UI (@stepansnigirev)
- #130 - Showing transacation details while sending (@ben-kaufman)
- #232 - Being able to copy transaction instead of sending via own node (@ben-kaufman)
- #139 - User feedback for proper connection to Core in settings menu (@k9ert)
- #140 - Bugfix which blocked the use of Coldcard under certain circumstances  (@ben-kaufman)
- #128 - Bugfix how funds get represented  (@ben-kaufman)

- A lot of refactorings (especially for template-logic) and tidyups. We also removed some dependencies (@ben-kaufman, @stepansnigirev)

## v0.3.0 May 11, 2020
- #104 - QR-Code animations enable to pass more information in smaller chunks (@gorazdko)
- #108 - Renaming and Deleting wallets (@ben-kaufman)
- #95 - addresses and utxo-view for better overview of your funds (@ben-kaufman)
- #100 - Pending PSBTS for partially sign and sign with others devices much later (@ben-kaufman)
- #101 - Support Device passphrases for HWI-wallets (@ben-kaufman)
- #40 - coin selection to control which utxo you want to spend (@k9ert)
- #120 - Display Addresses on device (@ben-kaufman)
- #127 - Windows support (@stepansnigirev)

## v0.2.0 Mar 27, 2020
- #94 - label addresses to get remember where coins are coming from (@ben-kaufman)
- #81 - Optional Authentication with RPC Password (@k9ert)
- Support custom block explorer for all networks (@ben-kaufman)

## v0.1.2 Mar 6, 2020
- bugfix-release (#84)

## v0.1.1 Feb 29, 2020
- #80 - Support for compressed PSBT in QR-codes (@stepansnigirev)
- #77 - Use specter-diy to sign via USB (@stepansnigirev)

## v0.1.0 Feb 27, 2020
- #73 - Rescan Blockchain to import older wallets easily (@stepansnigirev)
- Command-line options for server: daemon, ssl-certs and tor

## v0.0.2 Feb 20, 2020
- #69 - First PIP-Release available on [PyPi](https://pypi.org/project/cryptoadvance.specter/#history) (@k9ert)
- #23 - HWI support enables a whole bunch of hardwarewallets to work with specter (@kdmukai)
- #19 - Tor integration (@kdmukai)
- #56 - Support for coldcard (@kdmukai)
- #64 - https support (@stepansnigirev)

## v0.0.1-alpha Sep 28, 2019
Specter Desktop has been started by @stepansnigirev since Aug 30, 2019.
Thank you Stepan :-).
